## Event Manager

### Links to Closed Issues
Below are the links to the closed issues for this project:

[Issue #1](https://github.com/dhanesh-kh/event_manager/issues/1)

[Issue #2](https://github.com/dhanesh-kh/event_manager/issues/3)

[Issue #3](https://github.com/dhanesh-kh/event_manager/issues/5)

[Issue #4](https://github.com/dhanesh-kh/event_manager/issues/7)

[Issue #5](https://github.com/dhanesh-kh/event_manager/issues/9)
### Docker Image
The project image has been deployed to Docker Hub. You can find it at the following link:

[Event Manager Docker Image](https://hub.docker.com/layers/kdhanesh/event_manager/tagname/images/sha256-8bbf798771f5d9d35a692aac761a6f664964fe6c9381127757d93623f4e26c65?context=repo)

Reflecting on the work done to resolve the issues, I learned a lot about the importance of aligning test data with expectations. For example, the failure of the UserResponse test due to a missing nickname field shows the importance of test data mirroring the model schema. By adding the nickname field to the user_response_data, I not only fixed the test but also saw the importance cross-checking test fixtures against models, ensuring the test was reliable and accurate.

Another valuable lesson was learned from addressing the test failure related to updating user names. The test was initially failing because it was only checking the first_name field instead of the full name. By updating the user_update_data to include both first_name and last_name fields, and adjusting the test to reflect this change, I learned how to see the intended functionality. This experience showed the significance of precise test conditions and the need for test cases to reflect the actual behavior of the application.

Lastly, resolving the issue with JWT tokens and user information updates taught me about the complexities of authentication and authorization in tests. The tests were failing due to missing or incorrect tokens, which were necessary for verifying user roles and permissions. By implementing fixtures to generate these tokens and updating the tests accordingly, I ensured that each test ran with the appropriate permissions. This highlighted the importance of testing for different user roles and the need to simulate the permissions in order to catch any potential issues from wrong permissions in testing. Overall, I'd say the assignment gave me a more comprehensive understanding of test-driven development and the importance of test data management.
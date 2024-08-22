
# Description

•In this application 2 databases are used. MySQL is used for running the application and H2 database is used for unit testing repository layer.

•h2 database is configured in src/test/resources/application-test.properties and @ActiveProfiles annotation is used.

•@DataJpaTest provides a minimal Spring context for testing the persistence layer. It is limited to the JPA repository layer of the application. It doesn’t load the entire application context. It clean up the record after each test to the database doent remain populated.

•@Spy annotation is used to implement real modelMapper object properties in test cases.

![Screenshot 2024-08-22 124357](https://github.com/user-attachments/assets/fda8e791-0461-44b8-b527-107868dc9d6d)

![Screenshot 2024-08-22 124727](https://github.com/user-attachments/assets/33f193a9-1b8f-4e0c-b346-3ef30780572d)

![Screenshot 2024-08-22 124757](https://github.com/user-attachments/assets/a59b93ca-c896-408a-8e95-6b166adb892e)

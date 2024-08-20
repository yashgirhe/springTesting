
# Description

•In this application 2 databases are used. MySQL is used for running the application and H2 database is used for unit testing repository layer.

•h2 database is configured in src/test/resources/application-test.properties and @ActiveProfiles annotation is used.

•@DataJpaTest provides a minimal Spring context for testing the persistence layer. It is limited to the JPA repository layer of the application. It doesn’t load the entire application context. It clean up the record after each test to the database doent remain populated.

•@Spy annotation is used to implement real modelMapper object properties in test cases.
Introduction:
Briefly explain the current implementation of your ASP.NET web app for calculating bank guarantees and liabilities using a nightly SQL job and custom waits for 24 hours.
Highlight the need for real-time processing and faster data updates to improve the responsiveness of your web app.
Proposal:
Present your proposal to implement real-time processing using Kafka Streams and CQRS pattern for accepting and processing client and liability data in real-time.
Mention the use of Kafka Connect for syncing data to downstream systems or Oracle DB for seamless data integration.
Highlight the addition of a circuit breaker to handle transient failures during data push to Kafka, improving the resiliency of your system.
Mention the use of a schema registry to ensure data integrity and compatibility between producers and consumers, enhancing data validation and serialization/deserialization.
Benefits:
Explain the advantages of the proposed approach, including:
Real-time processing: Data updates are processed in real-time, reducing the delay and providing up-to-date information to users.
Improved responsiveness: Users can get immediate feedback on bank guarantees and liabilities, enhancing the user experience.
Scalability: Kafka Streams provides horizontal scalability for handling high volumes of data.
Resiliency: The circuit breaker helps to handle transient failures, preventing cascading failures and improving system stability.
Data integrity: Schema registry ensures data compatibility and validation, reducing data-related errors.
Seamless integration: Kafka Connect simplifies data synchronization with downstream systems or Oracle DB, enhancing data integration capabilities.

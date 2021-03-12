# Section 4: Integrating Google Cloud services

## 4.1 Integrating an application with data and storage services.

Considerations include:

* Read/write data to/from various databases (e.g., SQL)
* Connecting to a data store (e.g., Cloud SQL, Cloud Spanner, Firestore, Cloud Bigtable)
* Writing an application that publishes/consumes data asynchronously (e.g., from Pub/Sub)
* Storing and retrieving objects from Cloud Storage

## 4.2 Integrating an application with compute services.

Considerations include:

* Implementing service discovery in GKE and Compute Engine
* Reading instance metadata to obtain application configuration
* Authenticating users by using OAuth2.0 Web Flow and Identity-Aware Proxy
* Authenticating to Cloud APIs with Workload Identity

## 4.3 Integrating Cloud APIs with applications.

Considerations include:

* Enabling a Cloud API
* Making API calls using supported options (e.g., Cloud Client Library, REST API or gRPC, APIs Explorer) taking into consideration:
   * Batching requests
   * Restricting return data
   * Paginating results
   * Caching results
   * Error handling (e.g., exponential backoff)
* Using service accounts to make Cloud API calls

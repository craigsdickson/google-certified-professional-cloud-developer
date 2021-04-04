# Section 1: Designing highly scalable, available, and reliable cloud-native applications

## 1.1 Designing high-performing applications and APIs.

Considerations include:

* Microservices
   * Reading
      * [Microservices Architecture on Google App Engine (Java)](https://cloud.google.com/appengine/docs/standard/java/microservices-on-app-engine) - other language examples available from same page
      * [Solution - Migrating a monolithic application to microservices on Google Kubernetes Engine](https://cloud.google.com/solutions/migrating-a-monolithic-app-to-microservices-gke)
      * [Solution - Architecture: Scalable commerce workloads using microservices](https://cloud.google.com/solutions/architecture/scaling-commerce-workloads-architecture)
      * [Operations Suite - Microservices](https://cloud.google.com/stackdriver/docs/solutions/slo-monitoring/microservices)
      * [Serve dynamic content and host microservices using Firebase Hosting](https://firebase.google.com/docs/hosting/serverless-overview)
   * Code Examples
      * [GitHub - microservices demo](https://github.com/GoogleCloudPlatform/microservices-demo)
   * Labs
      * [Codelab - Migrating a Monolithic Website to Microservices on Google Kubernetes Engine](https://codelabs.developers.google.com/codelabs/cloud-monolith-to-microservices-gke#0)
* Scaling velocity characteristics/tradeoffs of IaaS (infrastructure as a service) vs. CaaS (container as a service) vs. PaaS (platform as a service)
* Geographic distribution of Google Cloud services (e.g., latency, regional services, zonal services)
   * Reading
      * [Geography and regions](https://cloud.google.com/docs/geography-and-regions#:~:text=Google%20Cloud%20services%20are%20available,%2C%20availability%2C%20and%20durability%20requirements.)
      * [Cloud locations](https://cloud.google.com/about/locations)
      * [Regions and zones](https://cloud.google.com/compute/docs/regions-zones)
      * [Compute Engine - Global, regional, and zonal resources](https://cloud.google.com/compute/docs/regions-zones/global-regional-zonal-resources)
* Defining a key structure for high-write applications using Cloud Storage, Cloud Bigtable, Cloud Spanner, or Cloud SQL
   * Reading
      * [Big Table - Designing Your Schema](https://cloud.google.com/bigtable/docs/schema-design)
      * [Cloud Storage - Naming Best Practices](https://cloud.google.com/storage/docs/best-practices#naming)
      * [Cloud Spanner - Schema design best practices](https://cloud.google.com/spanner/docs/schema-design)
      * [Cloud SQL - Data Architecture](https://cloud.google.com/sql/docs/mysql/best-practices#data-arch)
* User session management
   * Tutorial
      * [AppEngine - Handling sessions with Firestore](https://cloud.google.com/go/getting-started/session-handling-with-firestore)
   * Open Questions
      * Is IAP in scope for the exam?
* Caching solutions
   * App Layer Caching
      * Reading
         * [AppEngine - Caching data with Memorystore](https://cloud.google.com/appengine/docs/standard/go111/using-memorystore)
         * [MemoryStore for Redis](https://cloud.google.com/memorystore/docs/memcached)
   * Content Caching (CDN)
      * Reading
         * [Cloud CDN - Caching Overview]()https://cloud.google.com/cdn/docs/caching
         * [Cloud Storage - Caching](https://cloud.google.com/storage/docs/caching)
* Deploying and securing API services
   * Reading
      * [API Gateway service docs](https://cloud.google.com/api-gateway/docs)
      * [Cloud Endpoints services docs](https://cloud.google.com/endpoints)
   * Open questions
      * Does the exam cover API Gateway and/or Cloud Endpoints?
* Loosely coupled asynchronous applications (e.g., Apache Kafka, Pub/Sub)
   * Reading
      * [Solutions - DevOps tech: Architecture](https://cloud.google.com/solutions/devops/devops-tech-architecture)
      * [Patterns for scalable and resilient apps](https://cloud.google.com/solutions/scalable-and-resilient-apps)
      * [Choosing the right architecture for global data distribution](https://cloud.google.com/solutions/architecture/global-data-distribution)
      * [Apache Kafka for GCP users: connectors for Pub/Sub, Dataflow and BigQuery](https://cloud.google.com/blog/products/data-analytics/apache-kafka-for-gcp-users-connectors-for-pubsub-dataflow-and-bigquery)
      * [Emulating Google’s Cloud Pub/Sub on Apache Kafka](https://medium.com/appscale/emulating-googles-cloud-pub-sub-on-apache-kafka-74084222c9db)
* Graceful shutdown on platform termination
   * Reading
      * [Graceful shutdowns on Cloud Run: Deep dive](https://cloud.google.com/blog/topics/developers-practitioners/graceful-shutdowns-cloud-run-deep-dive)
      * [Kubernetes best practices: terminating with grace](https://cloud.google.com/blog/products/containers-kubernetes/kubernetes-best-practices-terminating-with-grace)
   * Code Examples
      * [k8s-node-termination-handler](https://github.com/GoogleCloudPlatform/k8s-node-termination-handler)
* Google-recommended practices and documentation
   * Reading
      * [Cloud-native application development](https://cloud.google.com/solutions/cloud-native-app-development)
      * [5 principles for cloud-native architecture](https://cloud.google.com/blog/products/application-development/5-principles-for-cloud-native-architecture-what-it-is-and-how-to-master-it)
      * [Whitepaper: Re-architecting to cloud native](https://services.google.com/fh/files/misc/re_architecting_to_cloud_native_whitepaper2.pdf)
   * Videos
      * [Building a Cloud Native Application from Scratch (Cloud Next '19)](https://www.youtube.com/watch?v=8ieMU_evObc)
      * [Cloud Native Application Development, Delivery and Persistent Storage (Cloud Next '19)](https://www.youtube.com/watch?v=cVDg7tgzIQc)

## 1.2 Designing secure applications.

Considerations include:

* Implementing requirements that are relevant for applicable regulations (e.g., data wipeout)
   * Reading
      * [Google Cloud & the General Data Protection Regulation (GDPR)](https://cloud.google.com/security/gdpr)
      * [Compliance resource center](https://cloud.google.com/security/compliance)
      * [Data deletion on Google Cloud Platform](https://cloud.google.com/security/deletion)
      * [Deleting your data in Google Cloud Platform](https://cloud.google.com/blog/products/storage-data-transfer/deleting-your-data-in-google-cloud-platform)
* Security mechanisms that protect services and resources
   * Reading
      * [Google Cloud Security Whitepapers](https://services.google.com/fh/files/misc/security_whitepapers_march2018.pdf)
      * [Google Cloud’s Approach to Security](https://services.google.com/fh/files/misc/csuite_security_ebook.pdf)
      * [Cloud Security FAQ](https://support.google.com/cloud/answer/6262505?hl=en)
* Security mechanisms that secure/scan application binaries and manifests
   * Reading
      * [Implementing Binary Authorization using Cloud Build and GKE](https://cloud.google.com/solutions/binary-auth-with-cloud-build-and-gke)
* Storing and rotating application secrets and keys (e.g., Cloud KMS, HashiCorp Vault)
   * Reading
      * [Secret Manager conceptual overview](https://cloud.google.com/secret-manager/docs/overview)
      * [Cloud KMS - Overview](https://cloud.google.com/kms/docs/quickstart)
* Authenticating to Google services (e.g., application default credentials, JSON Web Token (JWT), OAuth 2.0)
   * Reading
      * [Authentication overview](https://cloud.google.com/docs/authentication)
      * [Authenticating as a service account](https://cloud.google.com/docs/authentication/production)
      * [Authentication between services](https://cloud.google.com/endpoints/docs/openapi/service-account-authentication)
   * How-to / Tutorial
      * [Understanding OAuth2 and deploying a basic authorization service to Cloud Functions](https://cloud.google.com/community/tutorials/understanding-oauth2-and-deploy-a-basic-auth-srv-to-cloud-functions)
* IAM roles for users/groups/service accounts
   * Reading
      * [Granting, changing, and revoking access to resources](https://cloud.google.com/iam/docs/granting-changing-revoking-access)
* Securing service-to-service communications (e.g., service mesh, Kubernetes Network Policies, and Kubernetes namespaces)
   * Reading
      * [Anthos Service Mesh - security overview](https://cloud.google.com/service-mesh/docs/security/security-overview)
      * [Kubernetes best practices: Organizing with Namespaces](https://cloud.google.com/blog/products/containers-kubernetes/kubernetes-best-practices-organizing-with-namespaces)
      * [CloudRun - Authenticating service-to-service](https://cloud.google.com/run/docs/authenticating/service-to-service)
   * How-to / Tutorial
      * [GKE - Configuring network policies for applications](https://cloud.google.com/kubernetes-engine/docs/tutorials/network-policy)
* Running services with least privileged access (e.g., Workload Identity)
   * How-to / Tutorial
      * [GKE - Using Workload Identity](https://cloud.google.com/kubernetes-engine/docs/how-to/workload-identity)
* Certificate-based authentication (e.g., SSL, mTLS)
   * Reading
      * [SSL certificates overview](https://cloud.google.com/load-balancing/docs/ssl-certificates)
      * [Solution - Using mutual TLS to obtain short-lived credentials](https://cloud.google.com/solutions/using-mutual-tls-to-obtain-short-lived-credentials)
* Google-recommended practices and documentation

## 1.3 Managing application data.

Considerations include:

* Defining database schemas for Google-managed databases (e.g., Firestore, Cloud Spanner, Cloud Bigtable, Cloud SQL)
   * Reading
      * [Google Cloud databases](https://cloud.google.com/products/databases)
      * [Cloud Firestore Data model](https://firebase.google.com/docs/firestore/data-model)
      * [Spanner - Schema and data model](https://cloud.google.com/spanner/docs/schema-and-data-model)
      * [Bigtable - Designing your schema](https://cloud.google.com/bigtable/docs/schema-design)
      * [CloudSQL - MySQL - Best practices](https://cloud.google.com/sql/docs/mysql/best-practices)
      * [CloudSQL - PostgreSQL - Best practices](https://cloud.google.com/sql/docs/postgres/best-practices)
* Choosing data storage options based on use case considerations, such as:
   * Time-limited access to objects
   * Data retention requirements
   * Structured vs. unstructured data
   * Strong vs. eventual consistency
   * Data volume
   * Frequency of data access in Cloud Storage
   * Reading
      * [Cloud Storage - Signed URLs](https://cloud.google.com/storage/docs/access-control/signed-urls)
         * Signed URLs have limited time validity
      * [IAM - Resource attributes for IAM Conditions](https://cloud.google.com/iam/docs/conditions-resource-attributes)
         * Can use IAM Conditions to limit times when objects can be accessed (e.g. only during business hours)
      * [Cloud Storage - Retention policies and retention policy locks](https://cloud.google.com/storage/docs/bucket-lock)
      * [Google Cloud online storage products](https://cloud.google.com/products/storage)
         * Overview of storage products
      * [Cloud Storage - Storage Classes](https://cloud.google.com/storage/docs/storage-classes)
* Google-recommended practices and documentation

## 1.4 Application modernization.

Considerations include:

* Using managed services
* Refactoring a monolith to microservices
   * Reading
      * [Migrating a monolithic application to microservices on Google Kubernetes Engine](https://cloud.google.com/solutions/migrating-a-monolithic-app-to-microservices-gke)
* Designing stateless, horizontally scalable services
   * Reading
      * [Solutions - Patterns for scalable and resilient apps](https://cloud.google.com/solutions/scalable-and-resilient-apps)
* Google-recommended practices and documentation
   * Reading
      * [Solutions - Application modernization](https://cloud.google.com/solutions/application-modernization)
      * [Solutions - Modernize existing applications with Anthos](https://cloud.google.com/solutions/modernize-apps-with-anthos)
      * [Modernizing Your .NET Application for Google Cloud Platform](https://cloud.google.com/files/maximizing-cloud-computing-through-application-modernization.pdf)
      * [CIO Guide to Application Modernization](https://inthecloud.withgoogle.com/cio-guide-app-mod/cio_guide_app_modernization.pdf)
      * [Application modernization and the decoupling of infrastructure services and teams](https://services.google.com/fh/files/blogs/anthos_white_paper.pdf)


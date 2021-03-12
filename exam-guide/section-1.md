# Section 1: Designing highly scalable, available, and reliable cloud-native applications

## 1.1 Designing high-performing applications and APIs.

Considerations include:

* Microservices
   * Reading
      * [Microservices Architecture on Google App Engine](https://cloud.google.com/appengine/docs/standard/java/microservices-on-app-engine)
      * [Migrating a monolithic application to microservices on Google Kubernetes Engine](https://cloud.google.com/solutions/migrating-a-monolithic-app-to-microservices-gke)
      * [Scalable commerce workloads using microservices](https://cloud.google.com/solutions/architecture/scaling-commerce-workloads-architecture)
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
      * [DevOps tech: Architecture](https://cloud.google.com/solutions/devops/devops-tech-architecture)
      * [Patterns for scalable and resilient apps](https://cloud.google.com/solutions/scalable-and-resilient-apps)
      * [Choosing the right architecture for global data distribution](https://cloud.google.com/solutions/architecture/global-data-distribution)
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
* Security mechanisms that protect services and resources
* Security mechanisms that secure/scan application binaries and manifests
* Storing and rotating application secrets and keys (e.g., Cloud KMS, HashiCorp Vault)
* Authenticating to Google services (e.g., application default credentials, JSON Web Token (JWT), OAuth 2.0)
* IAM roles for users/groups/service accounts
* Securing service-to-service communications (e.g., service mesh, Kubernetes Network Policies, and Kubernetes namespaces)
* Running services with least privileged access (e.g., Workload Identity)
* Certificate-based authentication (e.g., SSL, mTLS)
* Google-recommended practices and documentation

## 1.3 Managing application data.

Considerations include:

* Defining database schemas for Google-managed databases (e.g., Firestore, Cloud Spanner, Cloud Bigtable, Cloud SQL)
* Choosing data storage options based on use case considerations, such as:
   * Time-limited access to objects
   * Data retention requirements
   * Structured vs. unstructured data
   * Strong vs. eventual consistency
   * Data volume
   * Frequency of data access in Cloud Storage
* Google-recommended practices and documentation

## 1.4 Application modernization.

Considerations include:

* Using managed services
* Refactoring a monolith to microservices
* Designing stateless, horizontally scalable services
* Google-recommended practices and documentation

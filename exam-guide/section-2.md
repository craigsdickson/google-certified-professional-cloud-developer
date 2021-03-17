# Section 2: Building and testing applications

## 2.1 Setting up your local development environment.

Considerations include:

* Emulating Google Cloud services for local application development
    * Reading
        * [App Engine - Using the Local Development Server](https://cloud.google.com/appengine/docs/standard/python/tools/using-local-server)
        * [Pub/Sub - Testing apps locally with the emulator](https://cloud.google.com/pubsub/docs/emulator)
        * [Running the Datastore Emulator](https://cloud.google.com/datastore/docs/tools/datastore-emulator)
        * [Introduction to Firebase Local Emulator Suite](https://firebase.google.com/docs/emulator-suite)
        * [Using the Cloud Spanner Emulator](https://cloud.google.com/spanner/docs/emulator)
    * Creating Google Cloud projects
        * [Creating and managing projects](https://cloud.google.com/resource-manager/docs/creating-managing-projects)
    * Using the command-line interface (CLI), Google Cloud Console, and Cloud Shell tools
        * [Cloud SDK](https://cloud.google.com/sdk)
        * [Cloud Console](https://console.cloud.google.com/)
        * [Cloud Shell](https://cloud.google.com/shell)
    * Using developer tooling (e.g., Cloud Code, Skaffold)
        * [Cloud Code](https://cloud.google.com/code)
        * [Skaffold](https://skaffold.dev/)
        * [Kubernetes development, simplified — Skaffold](https://cloud.google.com/blog/products/application-development/kubernetes-development-simplified-skaffold-is-now-ga)

## 2.2 Writing efficient code.

Considerations include:

* Algorithm design
* Modern application patterns
    * Reading
        * [Solutions - Patterns for scalable and resilient apps](https://cloud.google.com/solutions/scalable-and-resilient-apps)
        * [Cloud-native application development](https://cloud.google.com/solutions/cloud-native-app-development)
        * [5 principles for cloud-native architecture](https://cloud.google.com/blog/products/application-development/5-principles-for-cloud-native-architecture-what-it-is-and-how-to-master-it)
    * Videos
        * [Building a Cloud Native Application from Scratch (Cloud Next '19)](https://www.youtube.com/watch?v=8ieMU_evObc)
        * [Effective Cloud-Native Java on GCP (Cloud Next '19)](https://www.youtube.com/watch?v=g9qqEnhU_uU)
* Software development methodologies
    * Reading
        * [Twelve-factor app development on Google Cloud](https://cloud.google.com/solutions/twelve-factor-app-development-on-gcp)
        * [DevOps](https://cloud.google.com/devops)
* Debugging and profiling code
    * Reading
        * [Cloud Debugger](https://cloud.google.com/debugger)
        * [Cloud Profiler](https://cloud.google.com/profiler)
    * Tutorial/Lab
        * [Analyze production performance with Cloud Profiler](https://codelabs.developers.google.com/codelabs/cloud-profiler#0)

## 2.3 Testing.

Considerations include:

* Unit testing
* Integration testing
* Performance testing
* Load testing
    * Reading
        * [Cloud Functions - Testing HTTP Functions](https://cloud.google.com/functions/docs/testing/test-http)
        * [Cloud Functions - Testing Event-Driven Functions](https://cloud.google.com/functions/docs/testing/test-event)
        * [App Engine - Local Unit Testing for Java 8](https://cloud.google.com/appengine/docs/standard/java/tools/localunittesting)
    * Videos
        * [Shift Left: Continuous Integration Testing with Cloud Build (Cloud Next '19)](https://www.youtube.com/watch?v=pqCq24aEka4)
        * [Accelerate your Build and Test with Google Cloud Platform (Cloud Next '18)](https://www.youtube.com/watch?v=NcShWeGgWd0)

## 2.4 Building.

Considerations include:

* Source control management
    * Reading
        * [Cloud Source Repositories](https://cloud.google.com/source-repositories)
        * [DevOps tech: Version control](https://cloud.google.com/source-repositories)
* Creating secure container images from code
    * Reading
        * [Best practices for building containers](https://cloud.google.com/solutions/best-practices-for-building-containers)
        * [Binary Authorization](https://cloud.google.com/binary-authorization)
* Developing a continuous integration pipeline using services (e.g., Cloud Build, Container Registry) that construct deployment artifacts
    * Reading
        * [CI/CD on Google Cloud](https://cloud.google.com/docs/ci-cd)
        * [Set Up CI/CD With Firebase on Google Cloud Platform and GitHub in 10 Minutes](https://betterprogramming.pub/set-up-ci-cd-with-firebase-gcp-and-github-in-10-minutes-be76bee4579e)
    * Tutorial/Lab
        * [Continuous deployment to Google Kubernetes Engine (GKE) with Cloud Build](https://codelabs.developers.google.com/codelabs/cloud-builder-gke-continuous-deploy/index.html#0)
* Reviewing and improving continuous integration pipeline efficiency
    * Reading
        * [DevOps tech: Continuous integration](https://cloud.google.com/solutions/devops/devops-tech-continuous-integration)

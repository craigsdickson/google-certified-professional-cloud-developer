# Section 3: Deploying applications

## 3.1 Recommend appropriate deployment strategies using the appropriate tools (e.g., Cloud Build, Spinnaker, Tekton, Anthos Configuration Manager) for the target compute environment (e.g., Compute Engine, Google Kubernetes Engine).

Considerations include:

* Blue/green deployments
* Traffic-splitting deployments
* Rolling deployments
* Canary deployments

## 3.2 Deploying applications and services on Compute Engine.

Considerations include:

* Installing an application into a virtual machine (VM)
* Managing service accounts for VMs
* Bootstrapping applications
* Exporting application logs and metrics
* Managing Compute Engine VM images and binaries

## 3.3 Deploying applications and services to Google Kubernetes Engine (GKE).

Considerations include:

* Deploying a containerized application to GKE
* Managing Kubernetes RBAC and Google Cloud IAM relationships
* Configuring Kubernetes namespaces
* Defining workload specifications (e.g., resource requirements)
* Building a container image using Cloud Build
* Configuring application accessibility to user traffic and other services
* Managing container lifecycle
* Define Kubernetes resources and configurations

## 3.4 Deploying a Cloud Function.

Considerations include:

* Cloud Functions that are triggered via an event from Google Cloud services (e.g., Pub/Sub, Cloud Storage objects)
* Cloud Functions that are invoked via HTTP
* Securing Cloud Functions

## 3.5 Using service accounts.

Considerations include:

* Creating a service account according to the principle of least privilege
* Downloading and using a service account private key file

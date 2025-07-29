## Installing Authorino Operator with Argo CD on OpenShift
This README.md provides instructions for installing the Authorino Operator on an OpenShift cluster using oc CLI commands and leveraging Argo CD for GitOps-driven deployment.

### What is Authorino?
Authorino is a Kubernetes-native authorization service that helps protect your APIs with tailor-made Zero Trust security. It integrates with API gateways and proxies (like Envoy) to provide authentication and authorization capabilities.

### Prerequisites
Before you begin, ensure you have the following:

* An OpenShift 4.x cluster with administrative access.

* The oc CLI installed and configured to connect to your OpenShift cluster.

* An Argo CD instance deployed on your OpenShift cluster (e.g., via the Red Hat OpenShift GitOps Operator).

* A Git repository to store your Kubernetes manifests.

### Installation
~~~
oc apply -f app.yaml -n openshift-gitops # Or the namespace where your Argo CD instance is installed
~~~

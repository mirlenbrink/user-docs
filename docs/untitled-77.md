# Kubernetes integration overview

* [ Kubernetes integration overview](/hc/en-us/articles/360003916138-Kubernetes-integration-overview)
* [ Install the Snyk controller with Helm](/hc/en-us/articles/360003916158-Install-the-Snyk-controller-with-Helm)
* [ Automatic import/deletion of Kubernetes workloads projects](/hc/en-us/articles/360020835037-Automatic-import-deletion-of-Kubernetes-workloads-projects)
* [ Install the Snyk controller with OpenShift 4 and OperatorHub](/hc/en-us/articles/360006548317-Install-the-Snyk-controller-with-OpenShift-4-and-OperatorHub)
* [ Install the Snyk controller on Amazon Elastic Kubernetes Service \(Amazon EKS\)](/hc/en-us/articles/360011128137-Install-the-Snyk-controller-on-Amazon-Elastic-Kubernetes-Service-Amazon-EKS-)
* [ Adding Kubernetes workloads for security scanning](/hc/en-us/articles/360003947117-Adding-Kubernetes-workloads-for-security-scanning)
* [ Viewing project details and test results](/hc/en-us/articles/360003916178-Viewing-project-details-and-test-results)
* [ Snyk Priority Score and Kubernetes](/hc/en-us/articles/360010906897-Snyk-Priority-Score-and-Kubernetes)
* [ Viewing your Kubernetes integration settings](/hc/en-us/articles/360006368657-Viewing-your-Kubernetes-integration-settings)
* [ Disable the Kubernetes integration](/hc/en-us/articles/360003947137-Disable-the-Kubernetes-integration)

##  Kubernetes integration overview

Snyk integrates with Kubernetes, enabling you to import and test your running workloads and identify vulnerabilities in their associated images and configurations that might make those workloads less secure. Once imported, Snyk continues to monitor those workloads, identifying additional security issues as new images are deployed and the workload configuration changes.

**Feature availability**  
This feature is available in Business and Enterprise plans and is also supported by our on-prem offering. See [pricing plans](https://snyk.io/plans/) for more details.

**How it works**

1. Your administrator installs a controller on your cluster, authenticating the integration with a unique ID generated from the Snyk account. Install the controller with either of these options:
2. The controller communicates with the Kubernetes API to determine which workloads \(for instance the Deployment, ReplicationController, CronJob, etc.\) are running on the cluster, find their associated images, and scan them directly on the cluster for vulnerabilities.
3. From Snyk, collaborators select which workloads to import, or workloads can be imported automatically using annotations. These options are as described in [Adding Kubernetes workloads for security scanning](/hc/articles/360003947117#UUID-a0526554-0943-3363-6977-7a11f766ede2).
4. For each workload that your collaborators import, Snyk displays the vulnerabilities found in each image as well as a summary of configuration issues identified with the workload.
5. Snyk monitors your imported workloads on an ongoing basis, reporting on new vulnerabilities as they are disclosed whenever they affect your projects.
6. Based on your configurations, if vulnerabilities are found, Snyk notifies you via email or Slack so that you can take immediate action.

**Terms and conditions**

_The Snyk Container Kubernetes integration uses Red Hat UBI \(Universal Base Image\)._

_Before downloading or using this application, you must agree to the Red Hat subscription agreement located at redhat.com/licenses. If you do not agree with these terms, do not download or use the application. If you have an existing Red Hat Enterprise Agreement \(or other negotiated agreement with Red Hat\) with terms that govern subscription services associated with Containers, then your existing agreement will control._

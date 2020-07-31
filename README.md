# Installing TAS for K8s 0.3 beta

This is a collection of jupyter notebooks to perform the steps of installing TAS4K8s on either minikube or TKG. Then, connect to TAS with the cf cli and push a sample application.

Tested on Ubuntu 20.04, TKG 1.1.2 on vSphere 6.7U3 or Minikube

Prereqs

* Tested on Ubuntu 20.04
* TAS for K8s v0.3 downloaded from Tanzu Network
* Minikube or TKG with deployed guest cluster (5 nodes, 8GBx2vCPU)
* jupyter notebook or lab with bash kernel
* cf cli, bosh cli, k14 tools
* kubectl and context pointed to proper cluster. Modify notebooks as needed for local environment.
* helm client
* k9s optional for inspecting cluster
* DNS zone to set wildcard domain
* An application to push to TAS (Sample go app: https://github.com/cloudfoundry-samples/test-app.git)

To start, run from repository root:

```jupyter notebook```

Use either notebook depending on minikube or TKG preference. The tas4k8s app demo works with both once TAS is deployed.

Note the environment variables at the top to adjust for your own environment. 
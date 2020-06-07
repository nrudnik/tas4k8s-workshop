# Installing TAS for K8s 0.1 beta

This is a collection of jupyter notebooks to perform the steps of installing TAS4K8s on either minikube or TKG. Then, connect to TAS with the cf cli and push a sample application.

Tested on Ubuntu 20.04, TKG 1.1 on vSphere 6.7U3 or Minikube

Prereqs

* Tested on Ubuntu 20.04, should be adaptable to MacOS
* TAS for K8s downloaded from Pivnet
* Minikube or TKG with deployed guest cluster (3 nodes, medium)
* jupyter notebook or lab with bash kernel
* cf cli, bosh cli, k14 tools
* kubectl and context pointed to proper cluster. Modify notebooks as needed for local environment.
* helm client
* k9s optional for inspecting cluster
* DNS zone to set wildcard domain
* Your own application to push to TAS (TODO: add link to working test app)

To start, run from repository root:

```jupyter notebook```

Use either notebook depending on minikube or TKG preference. The tas4k8s app demo works with both once TAS is deployed.

Note the environment variables at the top to adjust for your own environment. 
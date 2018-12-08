# Workshop Tooling

In this page we list a few useful commands that we will use along the workshop to interact with our environment.

## Interacting with Vagrant

To interact with Vagrant, you should use the following commands:  
- `vagrant up`, start the Vagrant machine (will provision at first boot only)
- `vagrant provision`, force provisioning on an already existing machine
- `vagrant ssh`, ssh inside the newly created vagrant machine
- `vagrant destroy`, destroy the provisioned machine

## Kubernetes and MicroK8s
Inside the `vagrant` machine we have automatically provisioned a single-node Kubernetes cluster thanks to `microk8s`. [Microk8s](https://microk8s.io/) is a local Kubernetes distribution maintained by Canonical. Another alternative would have been to use Minikube. Microk8s has the benefit of being blazing fast and updated to Kubernetes 1.13.  

Interacting with Kubernetes:  
- `vagrant ssh` to enter the Vagrant machine
- `microk8s.status` will returnt the status of the cluster
- `kubectl get nodes` will interact with the API Server of Kubernetes and will return the single node description of the cluster

# Kubernetes: from DevOps practices to the Cloud-Native stack

Welcome to the "Kubernetes: from DevOps practices to the Cloud-Native stack" setup repo. This workshop is organized by [SIGHUP](https://sighup.io) and [Avanscoperta](https://www.avanscoperta.it). If you want to know more about the workshop [here you can find full abstract and detailed program](https://www.avanscoperta.it/it/training/kubernetes-from-devops-practices-to-the-cloud-native-stack/) and future programmer dates.

### About [SIGHUP](https://sighup.io)

We are a software and open source company specialized on infrastructural automation for public and private cloud. Our mission is to engineer, deliver and maintain battle tested automated infrastructures based on Kubernetes and the Cloud Native stack.

You can contact us by email at [hello@sighup.io](mailto:hello@sighup.io)

## Environment Setup

### Basic requirements  
#### Laptop

Each participant should bring his/her own laptop (Mac or Linux recommended, Windows is supported but expect to tweak around settings), 8GB of RAM recommended

#### Cloud Account

An active account with a Cloud Provider (AWS, GCP, Azure, DigitalOcean, Scaleway). Your account should be able to create, destory and play around with object storage, compute and networking resources. 

If your employer does not provide an account with a cloud provider (or in case you risk to destroy your actual production environment), you can get an account with GCP or Azure, both these providers have free credits that will allow you to follow the workshop without paying for cloud resources.

#### Clone this repo

Make sure to clone this repo.

#### Hypervisor

You should have an hypervisor installed on your machine and it should be compatible with `Vagrant`. All major OS (Mac, Linux, Windows) should be supported as well free (Virtualbox) and supported (VMWare/Parallels) virtualization solutions.

If you are not sure where to start, make sure to install [Virtualbox](https://www.virtualbox.org/).

Make sure to have the API Key and API Secret at hand the day of the workshop.

### Vagrant Machine

You will also need to setup a few different software pieces. We have bundled them all together in a Vagrant machine.

#### Vagrant setup

- [Install Vagrant](https://www.vagrantup.com/downloads.html) for your system  
- Inside the repo folder, issue a `vagrant up`  

You should be good to go!
If you have any issue, we highly recommend get in touch by email at [training@sighup.io](mailto:training@sighup.io).

## Check again before the workshop

Right before your workshop, make sure to pull any change to this repository and run `vagrant up && vagrant provision`. This will apply last minute changes to the workshop material.

#### LICENCE

This material is under copyright from SIGHUP s.r.l.
You are free to use this repository for personal use. Commercial use is forbidden unless authorized by written permission.

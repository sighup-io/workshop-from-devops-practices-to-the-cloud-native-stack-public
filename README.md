# Kubernetes: from DevOps practices to the Cloud-Native stack

Welcome to the "Kubernetes: from DevOps practices to the Cloud-Native stack" setup repo. This workshop is organized by [SIGHUP](https://sighup.io) and [Avanscoperta](https://www.avanscoperta.it). If you want to know more about the workshop [here you can find full abstract and detailed program](https://www.avanscoperta.it/it/training/kubernetes-from-devops-practices-to-the-cloud-native-stack/) and future programmer dates.

### About SIGHUP

[SIGHUP](https://sighup.io) is a software and open source company specialized on infrastructural automation for public and private cloud. Our mission is to engineer, deliver and maintain battle tested automated infrastructures based on Kubernetes and the Cloud Native stack.

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

If you are not sure where to start, install [Virtualbox](https://www.virtualbox.org/). At the time of writing, latest stable release is `Virtualbox 5.2.22`.

Make sure to have the API Key and API Secret at hand the day of the workshop.

##### Achtung!

If virtualbox is returning `VERR_CFGM_NOT_ENOUGH_SPACE`, simply rename the repo with a shorter name.

### Vagrant Machine

You will also need to setup a few different software pieces. We have bundled them all together in a Vagrant machine.

#### Vagrant setup

- [Install Vagrant](https://www.vagrantup.com/downloads.html) for your system  
- Inside the repo folder, issue a `vagrant up`  

You should be good to go!
If you have any issue, we highly recommend get in touch by email at [training@sighup.io](mailto:training@sighup.io).

#### Tooling
If you want to know a bit more about the tools we will use and how to start interacting with them, [check the tooling page](TOOLING.md).

## Pull updates

Right before your workshop, make sure to pull any change to this repository and run `vagrant up && vagrant provision`. This will apply last minute changes to the workshop material.

#### LICENCE

This material is authored and copyrighted from [SIGHUP s.r.l.](https://sighup.io)

It is forbidden to reproduce, copy and redistribute partially on entirely the material inside this repository for commercial use. You are free to use this repository for personal learning purposes.

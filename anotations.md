# OPENSHIFT - INSTALLATION

**MY ANOTATIONS ABOUT OPENSHIFT**


### Installer provisioned
> Suport AWS, AZURE GCP, OPENSTACK RHSP, AND RHEV, 
### User provisioned
> Suport AWS, AZURE GCP, OPENSTACK, VMware,VSphere, IBM Z, IBM POWER, and  bare metal


## Installation and configuration

### **HARDWARE REQUIREMENTS**
- vCPUS = 4 
- MEMORY = 9GB of free memory
- SOTARAGE SPACE = 35 GB of free storage space 


### **OPERATING SYSTEM REQUIREMENTS**
- WINDOWS
-  - WINDOWS 10 PRO FALL CREATORS UPDATE OR NEWER


- macOS
- - macOS 10.12 Sierra or newer


- LINUX
- - SUPPORTED: 
- - - RHEL/CENTOS 7.5 OR NEWEWR , FEDORA - 2 LATEST STABLE RELEASES


> [!IMPORTANT]
> ### UNSUPORTED
- UBUNTU 18.04 LTS OR NEWER
- DEBIAN 10 OR NEWER


## REQUIRE SOFTWARES PACKAGES
|        |     |         |
|------|---------|-------|
|LINUX DISTRIBUTIONS| INSTALLATION COMMANDS|
Fedora|sudo dnf install NetworkManager|
|RHEL/CentOS| su -c 'yum install NetworkManager'|
Debian/Ubuntu| sudo apt install qemu-kvm libvirt-daemon libvirt-daemon-system network-manager|


##  Installation and Upgrade

[Cloud REDHAT INSTALLATION](https://cloud.redhat.com/openshift/install)


https://cloud.redhat.com/openshift/install/crc/installer-provisioned

https://mirror.openshift.com/pub/openshift-v4/clients/crc/latest/crc-linux-amd64.tar.xz


### Follow the documentation to install CodeReady containers
Run the crc setup command to set up your host operating system for the CodeReady Containers virtual machine.

Then, the crc start will create a minimal OpenShift 4 cluster on your laptop or desktop computer.


```bash
$ crc setup
$ crc start
```

## Access OpenShift the CLI

```bash
$ crc oc-env
$ crc console --credentials
$ oc login -u user -p pass https://api.crc.testing:6443
$ oc new-project <projectname>

$ crc console
$ oc get co
```

## Login to the cluster
```bash
$ oc login
```
## Createing a project 
```bash
 $ oc new-project  my-project 
```
 ## View status of current project
 ```bash
 $ oc status
```

## Create a new app 

```bash
oc new-app https://github.com/sclorg/cakephp-example
```

## View pods

```bash
$ oc get pods -o wide
```

## View pod logs

```bash
$ oc logs cakephp-ex-1-deploy
```

## List supported APIs

```bash
$ oc api-reources
```

- ##  Helpful Links

[OpenShift 4.2 Documentation: Web Console](https://docs.openshift.com/container-platform/4.2/web_console/web-console.html)

[OpenShift 4.2 Documentation: CLI](https://docs.openshift.com/container-platform/4.2/cli_reference/openshift_cli/getting-started-cli.html)


# Create and delee a project 

### Create a project 

```bash
$ oc new-project 
```
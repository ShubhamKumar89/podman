# podman

 Installation of Podman on Ubuntu 20.04 LTS.
 
 ## Prerequisites
 
 1. `apt-get`, `curl`, and `apt-key` are installed.
 
 2. Superuser access.
 
 ## Procedure
 
 ### Source OS Release
```bash
source /etc/os-release
```
### Add Repository

```bash
echo "deb https://download.opensuse.org/repositories/devel:/kubic:/libcontainers:/stable/xUbuntu_${VERSION_ID}/ /" | sudo tee /etc/apt/sources.list.d/devel:kubic:libcontainers:stable.list
```

###  Add GPG Key

```bash
curl -L https://download.opensuse.org/repositories/devel:/kubic:/libcontainers:/stable/xUbuntu_${VERSION_ID}/Release.key | sudo apt-key add -
```

### Install Podman

```bash
sudo apt-get update
sudo apt-get -y upgrade
sudo apt-get -y install podman
```

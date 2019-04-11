Install RedHat OKD 4.0 on your own server.  For a local only install, it is suggested that you use CDK or MiniShift instead of this repo.

This install method is targeted for 3 node worker, 1 node master that has a long life.

**Please do use a clean CentOS system, the script installs all necesary tools and packages including Ansible, container runtime, etc.**

## Installation

1. ssh-keygen and ssh-copy-id for each node and cluster

3. Download & unzip

```
curl -LOk https://github.com/vatoio/openshift-centos/archive/master.zip
yum install -y unzip
unzip master.zip
```

3. execute `01-config-update.sh` for all worker and master

4. execute the installation `20-install-openshift-run-in-master.sh` script on guest machine

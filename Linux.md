# Linux

## Types

### Red Hat

* Fedora, CentOS, Oracle Enterprise
* Uses .rpm packages.
* dependencies are important and they are bundled with yum(CentOS)

#### Commands

* [Build a rpm package](https://www.thegeekstuff.com/2015/02/rpm-build-package-example/) : `yum install rpm-build`
* [Custom repo](https://www.digitalocean.com/community/tutorials/how-to-set-up-and-use-yum-repositories-on-a-centos-6-vps) : /etc/yum.repos.d 에 파일 생성
```
[examplerepo]
name=Example Repository
baseurl=http://mirror.cisp.com/CentOS/6/os/i386
enabled=1
gpgcheck=1
gpgkey=http://mirror.cisp.com/CentOS/6/os/i386/RPM-GPG-KEY-CentOS-6
```

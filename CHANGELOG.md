# Ansible Role for Docker

## 2.1.0 - TBC

## 2.0.0 - 2018-10-25

### Major Changes

  - Upgrade Ansible support to 2.6 or higher
  - Support both Ubuntu 16.04/18.04 and RHEL/CentOS 6/7
  - Remove support for optional `docker_image` and `docker_container`
  - Keep APT/YUM cache as-is
  - Update Travis CI test plan

## 1.1.0 - 2017-11-23

### Major Changes

  - Install Docker CE on Ubuntu 16.04/14.04 from official repository
  - Install Docker CE on CentOS 7 from official repository
  - Install Docker IO on CentOS 6 from stock package
  - Ensure docker-compose install with correct version
  - Update test cases

## 1.0.0 - 2017-09-25

  - Ininitial release for Ansible 2.4
  - Support both Ubuntu 16.04/14.04 or RHEL/CentOS 7/6

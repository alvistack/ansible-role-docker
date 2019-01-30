# Ansible Role for Docker

## 2.4.0 - TBC

### Major Changes

## 2.3.0 - 2019-01-30

### Major Changes

  - Porting test to Molecule based

## 2.2.0 - 2019-01-25

### Major Changes

  - Bugfix /lib/systemd/system/containerd.service with template
  - Use handler for `systemctl daemon-reload`
  - Rollback to default `native.cgroupdriver=cgroupfs`

## 2.1.0 - 2018-12-06

### Major Changes

  - CI with yamllint, ansible-lint and ansible-playbook --syntax-check
  - CI with LXD, improve systemd support
  - Use shell only when shell functionality is required
  - Ignore modprobe failures in ExecStartPre (systemd unit) (<https://github.com/containerd/containerd/pull/2776>)
  - Template `/etc/docker/daemon.json` for Kubernetes

### CentOS 6

  - Drop support

### CentOS 7

  - Enable repo with official procedure

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

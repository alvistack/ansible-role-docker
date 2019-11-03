# Ansible Role for Docker

## 3.6.0 - TBC

### Major Changes

  - Upgrade minimal Ansible support to 2.9.0

## 3.5.0 - 2019-10-06

### Major Changes

  - Support openSUSE Leap 15.1
  - Default with Python 3
  - Revamp molecule test with vagrant

## 3.4.0 - 2019-09-18

### Major Changes

  - Run molecule test manually on Travis CI
  - Apply sysctl entries in individual file
  - Apply modprobe entries in individual file

## 3.3.0 - 2019-08-27

### Major Changes

  - Update for RHEL 7
  - Add Vagrant test for RHEL 7
  - Restart service serially
  - Debug `WARNING: bridge-nf-call-iptables is disabled`

## 3.2.0 - 2019-07-08

### Major Changes

  - Update LXD test profile for Kubernetes v1.15.0 support
  - Fix molecule `group_vars` with links
  - Replace `with_items` with `loop`
  - Replace `with_dict` with `var`
  - Replace `with_first_found` with `lookup('first_found')`

## 3.1.0 - 2019-06-13

### Major Changes

  - Always include default variables from `vars/main.yml`
  - Always use `become: true` with molecule, especially for vagrant

## 3.0.0 - 2019-05-20

### Major Changes

  - Upgrade minimal Ansible support to 2.8.0
  - Improve handlers implementation
  - Restart service if templates changed

## 2.6.0 - 2019-05-04

### Major Changes

  - Test with `docker run hello-world`
  - Rollback to `native.cgroupdriver=systemd` for Kubernetes
  - Remove patch for /lib/systemd/system/containerd.service
  - Refine Travis CI Molecue test cases

## 2.5.0 - 2019-04-17

### Major Changes

  - Run test with `travis_wait 120`

## 2.4.0 - 2019-03-03

### Major Changes

  - Add openSUSE Leap 15 support

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

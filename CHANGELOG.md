# Ansible Role for Docker

## 5.2.0 - TBC

### Major Changes

  - Remove Ubuntu 20.10 support
  - Support Fedora 35
  - Support Ubuntu 21.10
  - Upgrade minimal Ansible community package support to 4.6.0
  - Install dependencies with package manager

## 5.1.0 - 2021-07-18

### Major Changes

  - Upgrade minimal Ansible community package support to 4.2.0
  - Support Debian 11
  - Support openSUSE Leap 15.3

## 5.0.0 - 2021-06-02

### Major Changes

  - Upgrade minimal Ansible support to 4.0.0
  - Support Fedora 34
  - Support Ubuntu 21.04

## 4.7.0 - 2021-03-13

### Major Changes

  - Bugfix [ansible-lint `namespace`](https://github.com/ansible-community/ansible-lint/pull/1451)
  - Bugfix [ansible-lint `no-handler`](https://github.com/ansible-community/ansible-lint/pull/1402)
  - Bugfix [ansible-lint `unnamed-task`](https://github.com/ansible-community/ansible-lint/pull/1413)
  - Simplify Python dependency with system packages
  - Support RHEL 8 with Molecule
  - Support RHEL 7 with Molecule
  - Remove CentOS 8 support
  - Improve HTTP transparent proxy support
  - Support CentOS 8 Stream
  - Support openSUSE Tumbleweed
  - Migrate base Vagrant box from `generic/*` to `alvistack/*`

## 4.6.0 - 2020-12-28

### Major Changes

  - Simplify Molecule scenario for vagrant-libvirt
  - Migrate from Travis CI to GitLab CI
  - Support Fedora 33
  - Remove Fedora 32 support
  - Support Ubuntu 20.10
  - Remove redundant tags from tasks

## 4.5.0 - 2020-08-26

### Major Changes

  - Upgrade minimal Ansible Lint support to 4.3.2

## 4.4.0 - 2020-08-19

### Major Changes

  - Upgrade Travis CI test as Ubuntu Focal based
  - Upgrade minimal Ansible support to 2.10.0
  - Support openSUSE Leap 15.2
  - Remove Ubuntu 19.10 support
  - Remove Ubuntu 16.04 support
  - Support Fedora 32
  - Support Debian 10
  - Support CentOS/RHEL 8
  - Support Ubuntu 20.04
  - Migrate role name to lowercase or underline
  - Migrate group name to lowercase or underline
  - Migrate molecule `group_vars` to file
  - Consolidate molecule tests into `default` (noop)

## 4.2.0 - 2020-02-13

### Major Changes

  - Migrate molecule driver to Libvirt
  - Migrate molecule verifier to Ansible
  - Support Ubuntu 19.10
  - Tweak `/etc/sysctl.conf` in Ansible style

## 4.1.0 - 2020-01-16

### Major Changes

  - Default `interpreter_python` with `python3`
  - Bugfix `python3-xml` not exists for openSUSE Leap 15.1

## 4.0.0 - 2019-11-05

### Major Changes

  - Upgrade minimal Ansible support to 2.9.0
  - Upgrade Travis CI test as Ubuntu Bionic based

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

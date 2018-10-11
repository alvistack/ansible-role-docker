Ansible Role for Docker
=======================

1.2.0 - TBC
-----------

### Major Changes

-   Upgrade Ansible support to 2.6 or higher
-   Remove Ubuntu 14.04 support
-   Add Ubuntu 18.04 support
-   Keep APT/YUM cache as-is
-   Simplify role duty to just handling installation

1.1.0 - 2017-11-23
------------------

### Major Changes

-   Install Docker CE on Ubuntu 16.04/14.04 from official repository
-   Install Docker CE on CentOS 7 from official repository
-   Install Docker IO on CentOS 6 from stock package
-   Ensure docker-compose install with correct version
-   Update test cases

1.0.0 - 2017-09-25
------------------

-   Ininitial release for Ansible 2.4
-   Support both Ubuntu 16.04/14.04 or RHEL/CentOS 7/6
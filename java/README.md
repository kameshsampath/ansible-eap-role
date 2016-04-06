Java
=========

A role to install OpenJDK as JDK or JRE

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

* `openjdk_version` - The JDK version to install, defaults to 1.8.0
* `openjdk_package` - The rhel7 java package name, defaults to `java-1.8.0-openjdk-headless`


Example Playbook
----------------

When you want to install OpenJDK 1.8 as part of your playbook, include this role like, 

    - hosts: eap
      roles:
         - { role: java, openjdk_version: '1.8.0'  openjdk_package: "java-{{openjdk_version}}-openjdk-headless"}

License
-------

[LICENSE](../LICENSE)

Authors Information
------------------

* [Andrew Block] (mailto:andy.block@gmail.com)
* [Albert Wong] (mailto:atwong@alumni.uci.edu)
* [Justin Holmes] (mailto:justinmichaelholmes@gmail.com)
* [Kamesh Sampath] (mailto:kamesh.sampath@hotmail.com)


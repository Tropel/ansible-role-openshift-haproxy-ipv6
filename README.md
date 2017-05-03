OpenShift HAProxy IPv6 Role
===========================

This Ansible role enables IPv6 on OpenShift HAProxy frontends.

Requirements
------------

One of:

* OpenShift Enterprise 3.2
* OpenShift Container Platform 3.3 or later
* OpenShift Origin M5 1.3 or later.

IPv6 configured on OpenShift nodes running routers.

Role Variables
--------------

| Name     | Default value    | Description                                    |
|----------|------------------|------------------------------------------------|
| routers  | None (Required)  | List of router DeploymentConfigs to configure  |

Dependencies
------------

* <https://github.com/appuio/ansible-role-openshift-haproxy>

Example Usage
-------------

`playbook.yml`:

    roles:
    - role: ../ansible-role-openshift-haproxy-ipv6
      routers:
      - ha-router-ex1

License
-------

Apache License Version 2.0

Author Information
------------------

APPUiO Team <info@appuio.ch>

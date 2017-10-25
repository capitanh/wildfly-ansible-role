Role Name
=========

This role install wildfly 10.1.0.Final application server

Requirements
------------

This role requires ansible 2.4.0.0 or higher, and Oracle JDK 8. You can find a role to install it at https://github.com/capitanh/oraclejdk-ansible-role. platform requirements are listed
in the metadata file.

Role Variables
--------------

The variables that can be passed to this role and a brief description about
them are as follows:

      wildfly_user:       wildfly       # OS User to run the server
      wildfly_basedir:    /opt          # Directory to install the server
      wildfly_home:       /opt/wildfly  # Wildfly home dir
      wildfly_version:    10.1.0.Final  # Software version

Dependencies
------------

None

Example Playbook
----------------

Register the role in requirements.yml:

    ```yaml
    - src: capitanh.wildfly-ansible-role
      name: wildfly

Include it in your playbooks:

    ```yaml
    - hosts: servers
      roles:
      - wildfly
    ```

License
-------

BSD


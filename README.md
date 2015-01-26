mapr-springxd
=========

A simple role to ensure compatibility between MapR's HDFS implementation and SpringXD. The role simply copies the `.jar` files containing MapR's HDFS implementation code to where SpringXD can find them. 

Requirements
------------

Install this on either a cluster node or a client node. The node must have either `mapr-core` or `mapr-client` installed.

Role Variables
--------------

This role has been tested with spring-xd 1.1.0.M2.

`spring_home: "spring-xd-1.1.0.M2"`

Dependencies
------------

None

Example Playbook
----------------

	- hosts: localhost
	  roles:
	    - { role: mapr-springxd,  spring_home: "spring-xd-1.1.0.M2" }

License
-------

BSD

Author Information
------------------

vgonzalez at mapr dot com

Role Name
=========

Vector

Requirements
------------
Create config for Vector
Example

````
[sources.inp]
type = "internal_logs"

[sinks.pes-sink]
type = "vector"
inputs = [ "inp" ]
address = "51.250.90.50:6000"
version = "1"

````


Role Variables
--------------
Variables in catalog defaults/vars  
1. vector_version  
2. vector_home


Dependencies
------------
---



Example Playbook
----------------
````yaml
- name: install vector
  hosts: vector
  roles:
    - vector-role
````
License
-------

BSD

Author Information
------------------

Lebedev Igor

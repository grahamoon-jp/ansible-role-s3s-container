Ansible Role: s3s container
=========

Build [s3s](https://github.com/frozenpandaman/s3s) container for podman environment.

Requirements
------------

This requires podman installed on target system.

Role Variables
--------------

|Name|Comment|
|----|----|
|s3s_config||List of s3s config. Parameter details are below. (Default: [])|

|Parameter|Comment|
|----|----|
|name|Name of config. *Required*|
|api_key|API key for stat.ink|
|acc_loc|Language|
|gtoken|Token for accessing splatnet|
|bullettoken|Token for accessing splatnet|
|session_token|Token for accessing nintendo|
|f_gen|Endpoint for generating f. (Default: `https://api.imink.app/f`|
|salmon|Get salmon run data. (Default: `no`)|
|timer_delay|Checking for new results every this configuration. (Default: `5min`)|

Dependencies
------------

None.

Example Playbook
----------------

```
- hosts: localhost
  roles:
   - grahamoon.s3s-container
```

License
-------

Apache

Author Information
------------------

Grahamoon


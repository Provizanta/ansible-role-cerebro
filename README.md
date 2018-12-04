Cerebro
=========

Cerebro productivity tool with plugins.

Requirements
------------

None

Role 
--------------

A list of plugins that should be installed.

    settings: <list of Cerebro settings>
    plugins: <list of plugins>
      - ...

Dependencies
------------

None

Example Playbook
----------------

    - hosts: localhost
      roles:
        - role: keepass
          vars:
            settings:
              hotkey: "Control+Shift+Space"
            plugins:
              - basic-apps 

License
-------

MIT

Author Information
------------------

Tibor Csoka

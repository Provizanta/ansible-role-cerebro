Ansible role: Cerebro
=========

Install and setup the Cerebro productivity tool with plugins.

Requirements
------------

None

Role
--------------

These defaults are set in defaults/main.yml:

    configuration:
      locale: en-US
      lang: en
      country: US
      theme: "../dist/main/css/themes/dark.css"
      hotkey: "Control+Space"
      showInTray: true
      firstStart: false
      developerMode: true
      cleanOnHide: true
      skipDonateDialog: true
      isMigratedPlugins: false
      trackingEnabled: false
      crashreportingEnabled: true
      openAtLogin: true

    plugins: []   # without the 'cerebro-' prefix

Dependencies
------------

None

Example Playbook
----------------

    - hosts: localhost
      roles:
        - role: cerebro
          vars:
            configuration:
              hotkey: "Control+Shift+Space"
            plugins:
              - basic-apps

License
-------

MIT

Author Information
------------------

Tibor Csóka

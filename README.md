Ansible role: Cerebro
=========

[![Build Status](https://travis-ci.com/Provizanta/ansible-role-cerebro.svg?branch=master)](https://travis-ci.com/Provizanta/ansible-role-cerebro)

Install and setup the Cerebro productivity tool with plugins.

Requirements
------------

None

Role
--------------

These defaults are set in [defaults/main.yml](./defaults/main.yml):

    cerebro_configuration:
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

    cerebro_plugins: []   # without the 'cerebro-' prefix

Dependencies
------------

None

Example Playbook
----------------

    - name: Converge
      hosts: all
      roles:
        - role: cerebro
          vars:
            cerebro_configuration:
              hotkey: "Control+Shift+Space"
            cerebro_plugins:
              - basic-apps

License
-------

MIT

Author Information
------------------

Tibor Csóka

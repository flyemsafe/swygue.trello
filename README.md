Role Name
=========

Installs Trello Desktop on Fedora

Requirements
------------

none

Role Variables
--------------

|                            | required | optional | default value                                                            | description                 |
|----------------------------|----------|----------|--------------------------------------------------------------------------|-----------------------------|
| trello_desktop             | X        |          | true                                                                     | true/false                  |
| trello_desktop_url         | X        |          | https://github.com/danielchatfield/trello-desktop/releases               | trello install url          |
| trello_desktop_user        | X        |          |                                                                          | your user name              |
| trello_desktop_group       | X        |          |                                                                          | your user group             |
| trello_desktop_install_dir | X        |          |                                                                          | where to install trello     |
| trello_desktop_launcher    | X        |          | /home/{{ trello_desktop_user }}/.local/share/applications/trello.desktop | where to place the launcher |

Dependencies
------------

none

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      vars_files:
        - "{{ playbook_dir }}/trello_vars.yml"
  
      roles:
        - role: swygue.trello
        tags: trello


License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).

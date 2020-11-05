Deploy_nginx
=========
A brief description of the role goes here.
### Task folder
- there is a task for installing nginx and python for different OS
### Hadlers
- reload nginx
### Templates
- ansible.srwx.net.conf.j2 config for nginx.
 - index.html web pages for testing with {% For item %} create Menus

# Requirements
------------
Debian or CentOS

# Role Variables
--------------
Variables for creating menus and submenus.
Links to install and copy paths

Example Playbook
----------------
-- defaults
   - main.yml

-- files

-- handlers
  - main.yml
-- README.md

-- tasks
  - main.yml

-- templates
   - ansible.srwx.net.conf.j2
   - index.html

 -- vars
    - main.yml


  ---
  - hosts: dev
      gather_facts: yes
      roles:
        - { role: deploy_nginx, when: ansible_system == "Debian" }

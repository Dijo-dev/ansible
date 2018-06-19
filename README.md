## Web Server setup.

### Requirements:
* Sudo rights
* ansible 2.5
* ssh client
* At least one web server :smile:

### Purpose

This setup install some tools to facilitate the use and navigation in
your web-server as :
* Vim-nox to edit files.
* Git to handle repos.
* zsh to propose friendly bash.
* fonts-powerline to use the zsh agnoster theme.
* htop to manage process.

And the least applications for a web-server arbitrarily chosen by your
servant as :
* php7
* Apache2
* postgreSQL

### Customisation.
* Change *hosts* file content :
  - With your serverName/Ip lists.

        [webServer]
        serverName.com
        192.168.0.0/16
        [...]

  - With your server Vars

        [web:vars]
        user: your_user_name

### Installation :
* To launch server(s) setup launch :
      `ansible-playbook -i hostFile playbookFile.yml`

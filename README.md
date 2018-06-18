## Web Server setup.

### Requirements:
* Sudo rights
* ansible 2.5
* ssh client
* At least one web server :smile:

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

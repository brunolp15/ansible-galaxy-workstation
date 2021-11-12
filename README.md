# Workstation
=========

Esse projeto instala e configura todas as ferramentas e configurações básicas para um notebook de trabalho com DevOps/SRE.

## Dependecies ##
- ansible >= v2.11.6
- ansible-galaxy >= v2.11.6


## Goals ##

Running the Code
--------------

     * Para instalar as roles externas execute o script role_update.sh que irá realizar o download de todas as role via Ansible Galaxy.
     ```
     ./extensions/setup/role_update.sh
      
     ```
     * Insira os hosts que deseja rodar no playbook de acordo com a plataforma de cloud utilizada pela aplicação.
     ```
     ../inventory/hosts_aws ou ./inventory/hosts_gcp

     ```
     * Para rodar o playbook do init_server execute o seguinte commando.
     ```
     ansible-playbook -i inventory/hosts_aws plays/playbook-init-host.yml
 
Dependencies
------------

Nenhuma.

License
-------

BSD

Author Information
------------------

   Bruno Lopes.

   bruno.llopes@b2wdigital.com

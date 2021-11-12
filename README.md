Init\_server
=========

Esse projeto prepara o ambiente inicial para suportar todos os serviços em produção no Labs, configurando e instalando dependências.

Requirements
------------

Esse projeto requer a instalação do Ansible 2.5.5 ou superior

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

### ansible-vsftp
*ansible-vsftp*

Dans ce playbook nous avons essayé de lancer notre playbook vers une machine distante.
Notre fichier hosts contient les configuration de nos machines sur lesquelles nous voulons faire nos installations. L'essentiel des paramètres sont commenté ci-dessous:
  - other_host (remote machine ip)
  - ansible_connection=ssh (not necessary by default ansible use ssh)
  - ansible_user=user (user login on remote desktop)
  - ansible_become_pass=pa$$w0rd (password)
  - ansible_become_user=root 
  - ansible_become_method=su (when user have sudoers priviligies ansible_becom_user=root becomes optional)

### How to playbooks
ansible-playbooks your-playbook.yml -u[optional] username -b[optional] -k[optional] -i[optional] ipaddress,

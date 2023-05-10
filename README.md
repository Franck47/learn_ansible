# learn_ansible

#changer en user admin

su - admin 

##Creer les clé ssh sur la machine node, et voir le contenu du id_rsa.pub puis copier
ssh-keygen
cat .ssh/id_rsa.pub

## Coller le contenu du  id_rsa.pub la sur le repo github 
Profil -> Settings -> SSH and GPG Keys -> New ssh-key


###installer ansible-lint sur le node
sudo pip install ansible-lint

#Check de l'indentation du playbook
ansible-lint deploy.yml

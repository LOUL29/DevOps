Lab 5 Vagrant :

Connexion SSH sur notre serveur centOS :

![unknown](https://user-images.githubusercontent.com/93076379/206893010-39eca991-43c5-472b-ba4b-f2236b62b12d.png)

![unknown (1)](https://user-images.githubusercontent.com/93076379/206892996-eff3d759-d83d-4595-9c23-eac8c0e8c345.png)

Accès au serveur en localhost :

![unknown (2)](https://user-images.githubusercontent.com/93076379/206892999-580d251e-de05-434a-b412-8a820ab21c6c.png)

Récupération du mot de passe :

![unknown (3)](https://user-images.githubusercontent.com/93076379/206893001-1442074e-16bc-49d6-b46e-febb77d177bf.png)

Connexion au projet :

![unknown (4)](https://user-images.githubusercontent.com/93076379/206893004-d6dd189f-014c-4f54-8378-baba9df1a6e4.png)

Test de health OK :

![unknown (5)](https://user-images.githubusercontent.com/93076379/206893101-afc0d03c-e336-4654-9ddb-f998d1a7c8d5.png)

Analyse de stasks lors du lancement du playbook :

![unknown (6)](https://user-images.githubusercontent.com/93076379/206893111-468024ea-d9a6-4823-bc94-cfe2e0d086f2.png)

On modifie le fichier main.yml sur le serveur centos en ssh pour faire les checks sur readiness et liveness :

![unknown (8)](https://user-images.githubusercontent.com/93076379/206893146-357321c3-3d20-4e49-bdbc-7b21409fe10e.png)

On a bien les checks qui sont effectués via la commande ansible-playbook /vagrant/playbooks/run.yml --tags check -i /tmp/vagrant-ansible/inventory/vagrant_ansible_local_inventory

![unknown (9)](https://user-images.githubusercontent.com/93076379/206893177-343c8be2-c47c-44d3-8086-4d87b55bd7e8.png)

![unknown (7)](https://user-images.githubusercontent.com/93076379/206893122-99f33379-d695-48aa-9f17-1fd3b7736902.png)

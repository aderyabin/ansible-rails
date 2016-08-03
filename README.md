Ping All servers
```
ansible all -i hosts -m ping -u root
```

Connect to Vagrant
```
ssh -p 2222 -i .vagrant/machines/default/virtualbox/private_key  -o IdentitiesOnly=yes -o StrictHostKeyChecking=no -o PasswordAuthentication=no vagrant@127.0.0.1
```

Connect to Vagrant using deploy
```
ssh -p 2222 -i ~/.ssh/digitalocean deploy@127.0.0.1
```

Run commands on HOST
```
sudo apt-get update
sudo apt-get install software-properties-common
sudo apt-get -y install ansible aptitude
```

Deploy to vagrant
```
ansible-playbook -i hosts playbook.yml
```
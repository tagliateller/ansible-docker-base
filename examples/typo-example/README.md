# Manuelle Provision
export ANSIBLE_HOST_KEY_CHECKING=False
ansible-playbook --private-key=.vagrant/machines/default/virtualbox/private_key -u vagrant -s -i .vagrant/provisioners/ansible/inventory/vagrant_ansible_inventory ansible/site.yml

# Automatische Provision
vagrant up

# Docker
docker build -t typo3 .
docker run -d -p 8081:80 typo3

# TODO

Auftrennen Apache / MySQL


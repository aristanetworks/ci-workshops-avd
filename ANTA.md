
pip install --upgrade anta

anta get from-ansible --ansible-inventory sites/site_1/inventory.yml -o anta-inventory.yml -g SITE1_FABRIC

anta psirt -i anta-inventory.yml md-report --md-output sa-report.md
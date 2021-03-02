# ec2_inventory_patch

Patch to respect `all_instances: true` option in the Tower inventory source vars

Instructions:

  - sudo -i
  - ansible-tower-service stop
  - cd /var/lib/awx/venv/awx/lib/python3.6/site-packages/awx/main/models/
  - mv inventory.py inventory.bak
  - wget https://raw.githubusercontent.com/benjdudas/ec2_inventory_patch/main/inventory.py
  - chmod 644 inventory.py
  - ansible-tower-service start



# ec2_inventory_patch

Patch to respect `all_instances: true` option in source vars

Instructions:
  On all Tower instances
    - su - root
    - ansible-tower-service stop
    - cd /var/lib/awx/venv/awx/lib/python3.6/site-packages/awx/main/models/
    - mv inventory.py inventory.bak
    - wget <add_raw_link>
    - chmod 644 inventory.py
    - ansible-tower-service start



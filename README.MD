# Ansible playbooks using DSV plugin to retrieve secrets

### NOTE: requires installation of python-dsv-sdk module

## Use-cases:
- **dsv-test_client_creds.yaml:** Hard coding DSV client creds in playbook
- **dsv-test_client_url.yaml:** Pass the one-time-use client cred retrieval URL while executing the playbook (note: alternatively you could uncomment the _clienturl_ var in the file and add URL there
Example: 
  
  ```python3.9 /usr/bin/ansible-playbook dsv-test-client-url.yaml -i inventory.txt --extra-vars "clienturl=https://mydsvtenant.secretsvaultcloud.com/v1/clients/bootstrap/234234234234234234"```
  
  

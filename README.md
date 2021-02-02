# Fast solution for manage Filebeat on all server 


## How to use 

1) Set envitonemnt for exvution into `filebeat-instalation.yml`
```
---
- hosts: sbx [ SBX | DEV | PRD] or Cluster name [sbx_1 | sbx_2 | dev_3 ]
  gather_facts: no
  ...
```
2) Run Playbook
```
ansible-playbook -i $(find ../../ -name Sample_Inventory.yml)  beats-instalation.yml  -vv

1 plays in beats-instalation.yml
Enter Coollector name [filebeat | metricbeat ]: metricbeat  
```  
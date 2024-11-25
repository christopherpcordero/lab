# Virtual Lab Environment 

-------------------

Using Azure resources created virtual lab environment. Lab environment is used for pentesting and incident response practice. 

## Resources
--- 
| Resource Type | Name |
|---------------|-------|
| Virtual Network | vnet |
| Network Security Group | public_nsg |
| Network Security Group | private_nsg |
| Public IP | kali_ip |
| Public IP | siem_ip |
| Virtual Machine | kali |
| Virtual Machine | siem |
| Virtual Machine | vuln |

-------
### Virtual Network
#### vnet 
- IP Range
  - 10.0.0.0/16
  - Subnets
    - public
      - 10.0.0.0/24
    - private
      - 10.0.1.0/24
#### Network Security Group
- public_nsg
  - only internal traffic
- private_nsg
  - public facing subnet to allow outside traffic

### Topology 
![image](https://github.com/user-attachments/assets/dc47b9d8-4a99-471d-ac53-2a2d12096776)







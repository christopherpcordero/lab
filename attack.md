# Red Team Lab
---
## Description 
Using the already established virtual lab used the kali vm to simulate red team tasks such as network reconnacense, vulnerability exploitation, and penetration testing. 



## Resources 
|Resource Type | Resource Name |
|------------|-----------------|
|Virtual Machine | kali |
| Public IP | kali_ip |

## Tools
- kali linux
- nmap
- ssh


## Attacks
### Network Recon & Enumeration
1. ssh into kali vm from local pc using username & pw combination
2. locate kali internal IP
   - run ifconfig 
3. Recon network
    - using found ip run nmap to scan network
    - nmap 10.0.0.0/16 -T4 
    - Use -T4 flag to run quick scan to see hosts that are up
    - Found 2 hosts up
4. Enumerate network
     - to see what vms we found ran nmap using -A flag and used -sS to do a stealth scan
     - sudo nmap 10.0.0.4 -A -sS -Pn
     - found host with vulnerable ports open maybe http or ssh server since port 80 and port 22 are open
### Vulnerability Exploitation
1. host found at 10.0.0.4 has following open ports
     - 21 : ftp
     - 22 : ssh
     - 80 : http
2. 
    

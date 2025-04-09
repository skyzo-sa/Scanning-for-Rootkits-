# Linux Lab – Scanning for Rootkits 
## Objective

The objective of this script is to block incoming network traffic from a list of specified IP addresses using the iptables firewall in Linux. It automates the process of applying IP-based traffic restrictions for network security purposes.

### Job Skills Learned

- Linux System Administration
- Managing firewall rules using iptables.
- Bash Shell Scripting
- Using loops and conditional commands.
- Network Security and Access Control
- Automation and Efficiency


### Tools Used

- Linux Terminal Command Line Interface (CLI)
- Bash Shell
- iptables (Firewall)
- Networking Commands: ping, ifconfig
- VMware Tools: Linux VM


### STEPS



# installing rkhunter
`apt update && apt install rkhunter`
 ![image](https://github.com/user-attachments/assets/a5bb2b91-e611-4cc6-a247-843ed316a3f0)

 
# updating its data file of stored values with the current values
`rkhunter –propupd`
![image](https://github.com/user-attachments/assets/f4c5fc9e-cf32-4326-9343-9cc56bc69e66)
 
 
# running a full system check

`rkhunter --check # => /var/log/rkhunter.log`
![image](https://github.com/user-attachments/assets/2ad358f1-d2f2-4b15-842b-e7937c5cb28d)
![image](https://github.com/user-attachments/assets/888a0055-f00e-401e-a484-287e75b8600b)
  
`rkhunter --check --report-warnings-only`
 
 
# installing chkrootkit
`apt install chkrootkit`
![image](https://github.com/user-attachments/assets/1a7fff0c-4951-4293-8b80-051f3fb0d4cb)
 
 
# running a scan
`chkrootkit`
![image](https://github.com/user-attachments/assets/ed5f182c-eaba-4f80-8fa6-2905dd361d62)
 
`chkrootkit -q`
![image](https://github.com/user-attachments/assets/b1ac39e4-bb2a-4ba8-a303-9e9403b76829)
 
 

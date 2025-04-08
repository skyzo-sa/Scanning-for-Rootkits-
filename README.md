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
apt update && apt install rkhunter
 
 
# updating its data file of stored values with the current values
rkhunter –propupd
 
 
# running a full system check

rkhunter --check # => /var/log/rkhunter.log
 
 
rkhunter --check --report-warnings-only
 
 
# installing chkrootkit
apt install chkrootkit
 
 
# running a scan
Chkrootkit
 
chkrootkit -q
 
 

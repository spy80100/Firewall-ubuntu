# Firewall-ubuntu
Features
Block IP addresses
Block access to certain ports
Block specifed prefixes of IP address (to block networks)
Block too many requests made by the same IP in a short period of time (user can specify threshold and time)
Steps to Run
Type the following terminal command:
iptables -I INPUT -d 192.168.0.0/24 -j NFQUEUE --queue-num 1
Fill out the rules in the JSON file as follows:
Execute firewall.py using python3
Requirements
netfilterqueue
scapy

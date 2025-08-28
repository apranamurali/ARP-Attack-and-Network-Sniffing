# ARP-Attack-and-Network-Sniffing
# Explore Network Sniffing and ARP Attacks
#### NAME:APARNA.M
#### REGISTER NUMBER:212223220008
# AIM:

To explore network sniffing and ARP Attacks

## STEPS:

- `Step 1:` Install kali linux either in partition or virtual box or in live mode
- `Step 2:` Investigate on the various categories of tools as follows.
-  `Step 3:` Open terminal and try execute some kali linux commands

## ARP Attacks:  
ARP spoofing: A hacker sends fake ARP packets that link an attacker's MAC address with an IP of a computer already on the LAN. 

```
arpspoof -i eth0 -t <victim_IP> <gateway_IP>
```
## Tools Commonly Used:

**ARP Spoofing:** arpspoof, ettercap, bettercap

**Sniffing:** wireshark, tcpdump, dsniff
## Architecture Diagram
```
                     +-------------------+
                     |   Attacker (Kali) |
                     |  [ARP Spoof Tool] |
                     +---------+---------+
                               |
               +---------------+----------------+
               |                                |
       +-------v-------+              +---------v--------+
       | Victim Device |              | Gateway/Router   |
       | (e.g., Laptop)|              | (Default Gateway)|
       +---------------+              +------------------+
               |                                |
       ====== Normal ARP Traffic ===============|
               |                                |
               +---------> Internet             |
                         (DNS, HTTP, etc.)      |
                                                |
                  [Start ARP Spoofing/Poisoning]
                               |
                               v
               +-------------------------------+
               |  Attacker becomes MITM        |
               | (Man-in-the-Middle via ARP)   |
               +-------------------------------+
                               |
                     [Sniff Packets Using]
                 e.g., Wireshark, tcpdump, Ettercap

         +----------------------------------------------+
         | Captured Info:                               |
         |  - IP Addresses                              |
         |  - DNS Requests                              |
         |  - HTTP/HTTPS Data (if not encrypted)        |
         |  - Credentials (if sent in plain text)       |
         +----------------------------------------------+

```
## OUTPUT:
<img width="1010" height="806" alt="image" src="https://github.com/user-attachments/assets/7245ea96-2ba8-4e2c-9c60-15f36c61cc7e" />
<img width="1257" height="902" alt="image" src="https://github.com/user-attachments/assets/0dcb688a-d9ae-4d77-a558-60c1ab4ce6d4" />
<img width="812" height="140" alt="image" src="https://github.com/user-attachments/assets/35532824-278c-4c6e-a3df-0aa520a70a7b" />


## RESULT:
The kali linux tools for ARP Attack and Network Sniffing were identified successfully

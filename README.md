# SDN-testing
This repository provides an overview of technologies and tools used for setting up and testing various security and high availability requirements for Software-Defined Networking (SDN) elements.
## Description of Tasks and Responsibilities

### Requirement A.1: Message Integrity Using Message Bus

**Task:** Ensure message integrity between 'publisher' and 'producer' using RSA and TLS.

**Steps Taken:**
1. Set up Mininet to create a network topology.
2. Generated RSA key pairs on host h1.
3. Signed messages and transferred them to host h2.
4. Verified message integrity on h2 using the public key.
5. Implemented TLS for secure message transmission.

**Outcome:** Established a secure communication channel ensuring message integrity.

### Requirement A.2: Authentication of Users

**Task:** Ensure no messages are accepted from unknown or unauthenticated users.

**Steps Taken:**
1. Set up Mininet for testing.
2. Generated and used RSA key pairs for message signing and verification.
3. Tested with valid and invalid messages.
4. Implemented mutual TLS (mTLS) for client-server authentication.

**Outcome:** Successfully blocked messages from unauthenticated users.

### Requirement A.3: Securing Communications Using TLS

**Task:** Secure communications using TLS 1.2 and above.

**Steps Taken:**
1. Installed and started Wireshark for packet analysis.
2. Sent HTTPS requests using curl.
3. Monitored traffic to ensure TLS encryption.

**Outcome:** Verified secure TLS communication for message bus.

### Requirement A.4: Monitoring for Unauthenticated Messages

**Task:** Monitor message bus for unauthenticated or suspicious messages.

**Steps Taken:**
1. Set up Mininet and generated RSA key pairs.
2. Signed and verified messages.
3. Implemented a script to send email alerts on verification failure.

**Outcome:** Implemented real-time monitoring and alert system for unauthenticated messages.

### Requirement B: Identifying and Mitigating Potential Attacks

**Task:** Deploy security functionality to identify and mitigate attacks on SDN elements.

**Steps Taken:**
1. Created Docker containers for SDN elements and attacker.
2. Simulated SYN flood attack on SDN element.
3. Implemented monitoring script to detect and block attack.

**Outcome:** Successfully detected and mitigated SYN flood attack.

### Requirement C: High Availability for SDN Components

**Task:** Implement high availability architecture for SDN controllers.

**Steps Taken:**
1. Installed Docker and network tools.
2. Created Docker containers for primary and secondary SDN controllers.
3. Configured VRRP using Keepalived for failover.
4. Monitored traffic flow using tcpdump and Wireshark.

**Outcome:** Ensured high availability with successful failover between SDN controllers.

**Technical Skills:** Computer Networks, NFV, SDN, RSA encryption, TLS/SSL, Wireshark, Mininet, Docker, Keepalived.  
**Soft Skills:** Problem-solving, teamwork, effective communication.

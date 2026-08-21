---
tags: [path, cybersecurity, roadmap]
difficulty: 3
---

# Cybersecurity Path

Protect systems and data from attackers. Ethical hacking and defense.

## What You Will Do

- Monitor networks for suspicious activity.
- Perform penetration testing (ethical hacking).
- Investigate security breaches.
- Implement security policies and tools.

## Roadmap

### Phase 1: The Basics (Months 1-3)
- **Networking**: OSI model, TCP/IP, ports, protocols.
- **Linux**: Command line, file permissions, users.
- **Security Concepts**: CIA triad, encryption, hashing.
- **Scripting**: Basic Python or Bash.

### Phase 2: Offensive Security (Months 4-6)
- **Reconnaissance**: OSINT, scanning (Nmap).
- **Exploitation**: Metasploit, Burp Suite.
- **Web Vulnerabilities**: OWASP Top 10 (SQLi, XSS).
- **Password Cracking**: Hashcat, John the Ripper.

### Phase 3: Defensive Security (Months 7-9)
- **SIEM Tools**: Splunk, ELK Stack.
- **Incident Response**: Forensics, malware analysis.
- **Compliance**: GDPR, HIPAA, PCI-DSS basics.

## Domain Goodies

- **OverTheWire Bandit**: Linux security game.
- **TryHackMe**: Guided hacking rooms.
- **HackTheBox**: Advanced penetration testing labs.
- **PicoCTF**: Capture the Flag for beginners.
- **Practical Networking**: Deep dive into networking.

## Ebooks

See [[ebooks/README|Cybersecurity Ebooks]] for detailed book lists.

## Communities

See [[communities/README|Cybersecurity Communities]] for forums and Discords.

## Practice Projects

Build these projects to solidify your skills and create a portfolio:

### Project 1: Home Security Lab (Weeks 1-3)
**Goal**: Create a safe environment for security testing.
- Set up VirtualBox with isolated network (Host-only adapter)
- Install Kali Linux VM (attacker machine)
- Install Metasploitable2 or OWASP Broken Web Apps VM (victim machines)
- Configure network segmentation to prevent accidental exposure
- Document your lab topology using the [[../../00-TEMPLATES/Project-Tracker|Project Tracker Template]]

### Project 2: Network Vulnerability Assessment (Weeks 4-6)
**Goal**: Master reconnaissance and scanning.
- Use Nmap to scan your lab network
- Identify open ports, services, and OS versions
- Run vulnerability scans with Nessus Essentials (free) or OpenVAS
- Write a professional report with findings and remediation recommendations
- Practice on TryHackMe "Complete Beginner" path rooms

### Project 3: Web Application Penetration Test (Weeks 7-9)
**Goal**: Exploit common web vulnerabilities.
- Set up OWASP Juice Shop or DVWA (Damn Vulnerable Web App)
- Complete all OWASP Top 10 vulnerabilities:
  - SQL Injection (extract database contents)
  - Cross-Site Scripting (XSS) - steal fake cookies
  - Broken Authentication (bypass login)
  - Sensitive Data Exposure
  - More...
- Document each exploit with screenshots and write-ups

### Project 4: Blue Team Defense Lab (Weeks 10-12)
**Goal**: Learn defensive security operations.
- Set up ELK Stack (Elasticsearch, Logstash, Kibana) or Splunk Free
- Configure Windows/Linux VMs to forward logs
- Simulate attacks and detect them in SIEM
- Create alert rules for suspicious activity
- Practice incident response procedures

### Project 5: Capture The Flag (CTF) Challenge Series (Weeks 13-16)
**Goal**: Apply skills in realistic scenarios.
- Complete 5+ beginner CTF challenges on HackTheBox or TryHackMe
- For each challenge:
  - Document your methodology
  - Note tools used and commands run
  - Explain how you exploited vulnerabilities
  - Suggest how to prevent the attack
- Build a public write-up portfolio on GitHub or blog

## Challenge

Complete these quick tasks to test your knowledge:

- [ ] Complete the first 5 levels of OverTheWire Bandit.
- [ ] Install Kali Linux in a VM.
- [ ] Scan your own home network with Nmap.
- [ ] Document one vulnerability finding using the [[../../00-TEMPLATES/Troubleshooting-Log|Troubleshooting Log Template]].

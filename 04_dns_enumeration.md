# DNS Enumeration

## What is DNS?
- DNS stands for Domain Name System
- It is like a phonebook of the internet
- Converts human readable domain names into IP addresses
- Without DNS you would need to remember IP addresses of every website
- Example: google.com → 142.250.190.46

---

## What is DNS Enumeration?
- DNS Enumeration is the process of finding all DNS records of a target domain
- It helps discover subdomains, mail servers, IP addresses, and more
- It is one of the first steps in reconnaissance phase of ethical hacking
- Helps build a map of the target infrastructure
- Can reveal hidden or forgotten subdomains that may be vulnerable

---

## Why DNS Enumeration is Important in OSINT?
- Discovers all subdomains of a target
- Finds mail servers which can be used for email spoofing research
- Reveals hosting providers and IP ranges
- Finds internal infrastructure accidentally exposed
- Helps in finding old or forgotten subdomains with vulnerabilities

---

## DNS Record Types

### A Record
- Maps domain name to IPv4 address
- Example: example.com → 93.184.216.34

### AAAA Record
- Maps domain name to IPv6 address
- Example: example.com → 2606:2800:220:1:248:1893:25c8:1946

### MX Record
- Mail Exchange record
- Points to mail servers responsible for receiving emails
- Example: mail.example.com

### NS Record
- Name Server record
- Shows which DNS servers are authoritative for the domain
- Example: ns1.example.com

### CNAME Record
- Canonical Name record
- It is an alias pointing to another domain
- Example: www.example.com → example.com

### TXT Record
- Text record
- Used for verification, SPF, DKIM, DMARC records
- Can contain sensitive information sometimes

### PTR Record
- Pointer record
- Used for reverse DNS lookup
- Converts IP address back to domain name

### SOA Record
- Start of Authority record
- Contains administrative information about the domain
- Shows primary name server and admin email

### SRV Record
- Service record
- Defines location of specific services like VoIP, messaging
- Example: _sip._tcp.example.com

---

## DNS Enumeration Techniques

### Forward DNS Lookup
- Resolving domain name to IP address
- Most basic and common technique

### Reverse DNS Lookup
- Resolving IP address back to domain name
- Useful for finding other domains hosted on same IP

### Zone Transfer Attack
- DNS zone transfer is meant for syncing DNS records between servers
- If misconfigured, anyone can request a full copy of DNS records
- This reveals all subdomains and internal infrastructure
- Command: dig axfr @nameserver domain.com

### Subdomain Brute Force
- Trying common subdomain names against a target domain
- Uses wordlists like admin, mail, ftp, dev, test, staging etc
- Example: admin.target.com, dev.target.com, mail.target.com

### DNS Cache Snooping
- Checking what domains a DNS server has recently cached
- Reveals what websites users of that DNS server visited

### DNSSEC Walking
- DNSSEC is a security extension for DNS
- DNSSEC walking can enumerate all records if NSEC is used instead of NSEC3

---

## Common Subdomains to Look For
- mail.target.com
- admin.target.com
- ftp.target.com
- dev.target.com
- staging.target.com
- test.target.com
- api.target.com
- vpn.target.com
- portal.target.com
- remote.target.com
- webmail.target.com

---

## DNS Enumeration Tools

### nslookup
- Built in tool in Windows and Linux
- Used for basic DNS queries
```bash
nslookup example.com
nslookup -type=MX example.com
nslookup -type=NS example.com
```

### dig
- Domain Information Groper
- More powerful than nslookup
- Available on Linux
```bash
dig example.com
dig example.com MX
dig example.com NS
dig example.com TXT
dig example.com ANY
dig axfr @ns1.example.com example.com
```

### dnsenum
- Automated DNS enumeration tool
- Finds subdomains, MX records, NS records
- Attempts zone transfer automatically
```bash
dnsenum example.com
```

### dnsrecon
- Advanced DNS enumeration tool
- Supports multiple techniques
```bash
dnsrecon -d example.com
dnsrecon -d example.com -t axfr
dnsrecon -d example.com -t brt
```

### Sublist3r
- Python tool for subdomain enumeration
- Uses search engines like Google, Bing, Yahoo
```bash
sublist3r -d example.com
```

### Amass
- Most powerful subdomain enumeration tool
- Uses many data sources and techniques
```bash
amass enum -d example.com
```

### theHarvester
- Collects subdomains, emails, IPs from public sources
```bash
theHarvester -d example.com -b google
```

---

## Online DNS Enumeration Tools
- dnsdumpster.com
- securitytrails.com
- viewdns.info
- shodan.io
- censys.io
- virustotal.com (relations tab)
- crt.sh (certificate transparency logs)

---


## DNS Enumeration in Cybersecurity Use Cases
- Finding forgotten dev or staging subdomains with vulnerabilities
- Discovering internal portals exposed to internet
- Mapping full attack surface of a target
- Finding mail servers for email security testing
- Identifying hosting providers and CDN used by target

---

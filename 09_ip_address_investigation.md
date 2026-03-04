# IP Address Investigation

## What is IP Address Investigation?
- IP Address Investigation is the process of gathering information
  linked to an IP address
- IP stands for Internet Protocol
- Every device connected to internet has an IP address
- IP address investigation helps trace location, owner, and activity
- It is a core technique in network OSINT and cybersecurity investigations
- Used by ethical hackers, investigators, and security researchers

---

## What is an IP Address?
- IP address is a unique numerical label assigned to every device on a network
- It works like a home address for devices on the internet
- Two versions exist:
  - IPv4 → 32 bit address → Example: 192.168.1.1
  - IPv6 → 128 bit address → Example: 2001:0db8:85a3:0000:0000:8a2e:0370:7334
- Two types of IP addresses:
  - Public IP → visible on internet
  - Private IP → used inside local network

---

## Types of IP Addresses

### Static IP Address
- Permanently assigned to a device
- Does not change over time
- Easier to trace and investigate
- Used by servers and businesses

### Dynamic IP Address
- Changes periodically assigned by ISP
- Harder to trace over long period
- Used by most home internet connections

### Dedicated IP Address
- Single IP assigned to one user or website
- Common in web hosting

### Shared IP Address
- Multiple users or websites share same IP
- Common in shared web hosting

---

## Why IP Address Investigation is Important in OSINT?
- Traces location of attacker or target
- Identifies hosting provider of malicious website
- Finds open ports and running services
- Checks if IP is blacklisted or flagged for malicious activity
- Reveals ISP and organization behind IP
- Finds other domains hosted on same IP
- Helps in incident response and threat intelligence
- Identifies VPN, proxy, or Tor exit node usage

---

## What Can Be Found From an IP Address?
- Country and city of IP address
- ISP (Internet Service Provider) name
- Organization or company name
- ASN (Autonomous System Number)
- Hostname linked to IP
- Open ports and running services
- Operating system fingerprint
- Web technologies in use
- SSL certificates
- Domains hosted on same IP
- Blacklist status
- Abuse reports
- Whether IP belongs to VPN or proxy
- Whether IP is Tor exit node
- Geolocation coordinates (approximate)
- Timezone of IP location

---

## IP Address Investigation Techniques

### IP Geolocation
- Finding approximate physical location of IP address
- Provides country, city, region, and coordinates
- Not always 100% accurate
- VPN and proxy can show wrong location
- Accuracy varies by ISP and region

### Reverse DNS Lookup
- Finding hostname linked to an IP address
- Converts IP address back to domain name
- Reveals server name and organization
- Command: nslookup IP or dig -x IP

### WHOIS for IP Address
- Finding owner information of IP address range
- Reveals organization, ISP, and abuse contact
- Shows IP range allocated to organization
- Command: whois IP

### Port Scanning
- Finding open ports on target IP address
- Reveals services running on the server
- Helps identify attack surface
- Common ports:
  - 21 → FTP
  - 22 → SSH
  - 23 → Telnet
  - 25 → SMTP
  - 53 → DNS
  - 80 → HTTP
  - 443 → HTTPS
  - 3306 → MySQL
  - 3389 → RDP
  - 8080 → HTTP Alternate

### Banner Grabbing
- Collecting information from service banners
- Reveals software version and server type
- Example: Apache 2.4.49, OpenSSH 7.4

### ASN Lookup
- ASN stands for Autonomous System Number
- Every ISP and large organization has an ASN
- Finding ASN reveals IP ranges owned by organization
- Useful for finding all IP addresses of a target organization

### Passive DNS Analysis
- Finding all domains that have pointed to an IP address historically
- Reveals related infrastructure
- Shows domains even if they no longer point to that IP

### SSL Certificate Analysis
- SSL certificates contain domain names
- One IP can serve certificates for multiple domains
- Reveals all websites hosted on same server

---

## IP Address Investigation Tools

### Shodan
- Most powerful tool for IP and device investigation
- Indexes internet connected devices
- Shows open ports, services, banners, vulnerabilities
- Finds cameras, routers, servers, industrial systems
- Website: shodan.io
```bash
shodan host IP_ADDRESS
shodan search apache
shodan search "default password"
```

### Censys
- Similar to Shodan
- Scans entire internet for devices and services
- Shows certificates, ports, protocols
- Website: censys.io

### ipinfo.io
- Provides geolocation, ISP, ASN information
- Simple and fast API
- Website: ipinfo.io/IP_ADDRESS
```bash
curl ipinfo.io/8.8.8.8
```

### AbuseIPDB
- Database of IPs reported for malicious activity
- Check if IP has been flagged for abuse
- Shows abuse categories and reports
- Website: abuseipdb.com

### VirusTotal
- Checks IP against multiple threat intelligence sources
- Shows related domains and files
- Reveals malicious activity linked to IP
- Website: virustotal.com

### MXToolbox
- Checks if IP is on email blacklists
- Useful for investigating spam sources
- Website: mxtoolbox.com/blacklists

### Nmap
- Most popular port scanner
- Discovers open ports and services
- Performs OS detection
- Performs version detection
```bash
nmap IP_ADDRESS
nmap -sV IP_ADDRESS
nmap -O IP_ADDRESS
nmap -A IP_ADDRESS
nmap -p 1-65535 IP_ADDRESS
nmap -sn 192.168.1.0/24
```

### Traceroute
- Traces path packets take to reach IP address
- Shows all hops between source and destination
- Reveals intermediate routers and their locations
```bash
traceroute IP_ADDRESS
tracepath IP_ADDRESS
```

### Ping
- Checks if IP address is reachable
- Measures response time
```bash
ping IP_ADDRESS
ping -c 4 IP_ADDRESS
```

### dig and nslookup
- Perform reverse DNS lookup
- Find hostname linked to IP
```bash
dig -x IP_ADDRESS
nslookup IP_ADDRESS
```

### BGP Tools
- bgp.he.net → Hurricane Electric BGP toolkit
- Find ASN and IP ranges of organizations
- Trace routing paths

---

## Online IP Investigation Tools
- ipinfo.io
- whatismyipaddress.com
- ip2location.com
- maxmind.com
- abuseipdb.com
- shodan.io
- censys.io
- virustotal.com
- bgp.he.net
- dnsdumpster.com
- threatintelligenceplatform.com
- greynoise.io
- ipvoid.com

---

## VPN and Proxy Detection

### Why It Matters
- Attackers use VPN and proxy to hide real location
- Knowing if IP is VPN changes investigation approach
- Real location is hidden behind VPN server

### How to Detect VPN and Proxy
- Check if IP belongs to known VPN provider
- Check if IP is datacenter IP instead of residential
- Check ASN for VPN company names
- Use dedicated VPN detection tools

### VPN Detection Tools
- ipinfo.io/IP → shows if IP is VPN or proxy
- ipqualityscore.com
- proxycheck.io
- iphub.info

---

## Tor Exit Node Detection
- Tor network anonymizes internet traffic
- Last node in Tor circuit is called exit node
- Exit node IP is visible to destination server
- Can check if IP is known Tor exit node

### Tor Detection Tools
- check.torproject.org
- dan.me.uk/torlist
- ipinfo.io → shows Tor flag

---

## How to Find IP Address of a Target

### From Email Headers
- Email headers contain originating IP of sender
- Analyze Received headers from bottom to top
- X-Originating-IP field shows sender IP

### From Website
- Use ping or nslookup to find IP of website
- Website may be behind CDN like Cloudflare

### From Social Media
- Direct messages sometimes reveal IP in server logs
- Not directly accessible by regular users

### By Sending a Tracking Link
- Create a link that logs visitor IP when clicked
- Tools: grabify.link, iplogger.org, canarytokens.org
- Use only with permission and for ethical purposes

---

## CDN and IP Investigation Challenges

### What is CDN?
- CDN stands for Content Delivery Network
- Cloudflare, Akamai, Fastly are popular CDNs
- CDN hides real server IP behind CDN IP
- Target IP resolves to CDN IP not real server

### Finding Real IP Behind CDN
- Check historical DNS records for IP before CDN was used
- Check SSL certificate for alternate domains
- Check subdomains that may not use CDN
- Tools: securitytrails.com, censys.io
- Check MX records which often point to real IP

---

## IP Address Ranges of Major Cloud Providers
- AWS IP ranges: ip-ranges.amazonaws.com/ip-ranges.json
- Google Cloud IP ranges: cloud.google.com/compute/docs/faq
- Azure IP ranges: Microsoft download center
- Knowing cloud provider helps identify hosting infrastructure

---

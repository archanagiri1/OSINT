# WHOIS Lookup

## What is WHOIS?
- WHOIS is a query and response protocol
- It is used to find information about a registered domain name
- It queries databases that store information about domain owners
- Originally created in the early 1980s for internet management
- Managed by ICANN (Internet Corporation for Assigned Names and Numbers)

---

## Why WHOIS is Important in OSINT?
- Reveals identity of domain owner
- Helps trace malicious websites
- Used in phishing investigation
- Helps find linked domains of a target
- Useful in bug bounty reconnaissance phase

---

## What Information WHOIS Reveals?
- Registrant name (owner name)
- Registrant organization
- Registrant email address
- Registrant phone number
- Registrant country and address
- Domain registrar name
- Domain creation date
- Domain expiry date
- Last updated date
- Name servers (NS records)
- Domain status (active, locked, expired)

---

## Types of WHOIS
- **Thin WHOIS** → only stores basic info like registrar and name servers
- **Thick WHOIS** → stores complete registrant details

---

## WHOIS Privacy Protection
- Many domain owners use WHOIS privacy protection
- It hides personal details and replaces with proxy information
- Also called Domain Privacy or WHOIS Guard
- Even with privacy protection, registrar info and name servers are still visible

---

## How to Use WHOIS on Linux
```bash
whois google.com
whois facebook.com
whois <target-domain>
```

---

## How to Read WHOIS Output
- Domain Name → the registered domain
- Registrar → company where domain was purchased (GoDaddy, Namecheap etc)
- Creation Date → when domain was first registered
- Expiry Date → when domain will expire
- Name Servers → DNS servers handling the domain
- Status → current status of the domain

---

## WHOIS Online Tools
- who.is
- whois.domaintools.com
- icann.org/whois
- whois.net
- centralops.net

---

## Historical WHOIS
- Normal WHOIS shows current information only
- Historical WHOIS shows past owner details even if changed
- Useful when attacker changes ownership to hide identity

### Historical WHOIS Tools
- whoisology.com
- domaintools.com
- whoishistory.com

---

## WHOIS in Cybersecurity Use Cases
- Investigating phishing domains
- Finding linked domains of a threat actor
- Checking if a domain is recently registered (suspicious)
- Finding email address of domain owner for further OSINT
- Verifying legitimacy of a website

---

## Important Points
- Newly registered domains are often used for phishing
- Expired domains can be bought by attackers to reuse reputation
- Same registrant email found on multiple domains means same owner
- Name servers can link multiple domains to same infrastructure
```


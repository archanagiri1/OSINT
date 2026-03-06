# Dark Web OSINT

## What is the Dark Web?
- The dark web is a part of the internet not indexed by normal search engines
- It requires special software to access like Tor Browser
- It is a subset of the deep web
- Deep web includes all pages not indexed by search engines
- Dark web is intentionally hidden and requires special tools to access
- It uses onion routing to anonymize traffic
- Websites on dark web have .onion domain extensions

---

## Three Layers of the Internet

### Surface Web
- Publicly accessible part of internet
- Indexed by search engines like Google and Bing
- Examples: news websites, social media, blogs
- Estimated to be only 4% of total internet

### Deep Web
- Part of internet not indexed by search engines
- Requires login or direct URL to access
- Examples: email inboxes, banking portals, private databases
- Estimated to be 96% of total internet
- Not illegal to access

### Dark Web
- Small portion of deep web
- Requires special software like Tor to access
- Intentionally hidden from normal internet
- Contains both legal and illegal content
- Estimated to be a tiny fraction of deep web

---

## What is Tor?
- Tor stands for The Onion Router
- Originally developed by US Navy for secure communications
- Now maintained by Tor Project nonprofit organization
- Routes internet traffic through multiple relays worldwide
- Each relay only knows previous and next hop
- Traffic is encrypted in multiple layers like an onion
- Exit node is final relay that connects to destination
- Provides anonymity but not 100% guarantee

### How Tor Works
- User connects to Tor network via Tor Browser
- Traffic is encrypted three times
- Passes through three relays: Guard, Middle, Exit
- Each relay decrypts one layer of encryption
- Destination only sees exit node IP not real IP
- .onion sites are only accessible within Tor network

---

## Why Dark Web OSINT is Important?
- Threat intelligence gathering
- Finding leaked credentials and data
- Monitoring cybercriminal activity
- Tracking threat actor conversations
- Finding stolen corporate data
- Identifying emerging cyber threats
- Monitoring brand and organization mentions
- Finding leaked documents and databases
- Tracking malware and exploit sales
- Understanding attacker tools and techniques

---

## What Can Be Found on Dark Web?

### Leaked Data
- Stolen credentials from data breaches
- Credit card numbers and financial data
- Personal identity information
- Corporate email and password dumps
- Government and military documents
- Medical records

### Cybercriminal Activity
- Malware and ransomware for sale
- Exploit kits and zero day vulnerabilities
- Hacking services for hire
- DDoS attack services
- Phishing kits and tools
- Botnet rentals

### Forums and Communities
- Hacking forums and discussions
- Cybercriminal marketplaces
- Extremist communities
- Whistleblower platforms
- Privacy focused communities
- Journalism and free speech platforms

### Threat Intelligence
- Threat actor profiles and activities
- New attack techniques being discussed
- Targeted attack planning
- Vulnerability discussions before public disclosure
- Stolen data being sold or shared

---

## Dark Web OSINT Techniques

### Passive Monitoring
- Monitoring dark web forums and marketplaces
- Searching for specific keywords or organization names
- Using automated tools and services
- Not interacting with any dark web entities
- Collecting intelligence without exposing identity

### Keyword and Brand Monitoring
- Searching for company name on dark web
- Finding mentions of employee emails
- Finding leaked credentials from organization
- Monitoring for stolen data being sold

### Threat Actor Profiling
- Collecting posts and messages from threat actors
- Analyzing writing style and patterns
- Finding connections between different aliases
- Tracking threat actor across multiple forums

### Leaked Data Analysis
- Analyzing leaked credential databases
- Identifying affected users and organizations
- Checking password patterns and reuse
- Correlating leaked data with other intelligence

### Forum and Marketplace Analysis
- Analyzing dark web forum structure and members
- Finding administrator and moderator identities
- Tracking marketplace listings over time
- Identifying vendors and their activity patterns

---

## Dark Web Search Engines

### Ahmia
- Most popular dark web search engine
- Indexes .onion sites
- Accessible on surface web and Tor
- Website: ahmia.fi
- Filters out illegal content

### Torch
- One of oldest dark web search engines
- Large index of .onion sites
- Available only on Tor network
- Onion: xmh57jrknzkhv6y3ls3ubitzfqnkrwxhopf5aygthi7d6rplyvk3noyd.onion

### DuckDuckGo on Tor
- Privacy focused search engine
- Accessible via Tor Browser
- Does not track searches
- Can find some dark web content

### Haystak
- Large dark web search engine
- Indexes millions of .onion pages
- Available only on Tor

### Not Evil
- Dark web search engine
- Focuses on legitimate content
- Available only on Tor

---

## Dark Web OSINT Tools

### OnionSearch
- Python tool for searching dark web search engines
- Automates searching across multiple dark web engines
- Does not require Tor Browser for some features

### Intelligence X (IntelX)
- Powerful OSINT tool with dark web indexing
- Searches Tor, I2P, paste sites, and more
- Stores historical data even after original is deleted
- Website: intelx.io
- Has free and paid tiers

### Ahmia Search API
- Programmatic access to Ahmia search
- Can automate dark web keyword monitoring

### DarkSearch
- Dark web search engine with API
- Website: darksearch.io
- Allows automated searching

### Mitaka
- Browser extension for OSINT
- Searches multiple sources including dark web indexes

---

## Dark Web Monitoring Services
- These services monitor dark web on your behalf
- Alert when specific keywords or data appear
- Used by organizations to detect data breaches

### Popular Services
- Recorded Future
- Digital Shadows
- Flashpoint
- DarkOwl
- Terbium Labs
- SpyCloud
- Have I Been Pwned (haveibeenpwned.com)
- IntelX (intelx.io)
- Dehashed (dehashed.com)

---

## Paste Sites Monitoring
- Paste sites are used to share text anonymously
- Frequently used to dump leaked data
- Important to monitor for leaked credentials

### Popular Paste Sites
- pastebin.com
- ghostbin.com
- hastebin.com
- paste.ee
- dpaste.com
- privatebin.net

### Paste Site Monitoring Tools
- psbdmp.ws (Pastebin dump search)
- Google dorking: site:pastebin.com "company name"
- IntelX indexes paste sites

---

## I2P Network
- I2P stands for Invisible Internet Project
- Alternative anonymity network to Tor
- Used for internal darknet services
- Less popular than Tor but used by some threat actors
- Has its own .i2p domain system

---

## Freenet
- Decentralized censorship resistant network
- Used for anonymous file sharing and communication
- Less common for criminal activity than Tor
- Used by journalists and privacy advocates

---

## Dark Web Forums for Threat Intelligence
- RaidForums (seized by law enforcement)
- BreachForums
- XSS Forum
- Exploit.in
- Nulled
- Hackforums
- Note: Accessing these requires caution and is for research only

---

## Safe Dark Web OSINT Practices

### Technical Safety
- Always use Tor Browser for accessing dark web
- Never use personal device for dark web research
- Use dedicated virtual machine for investigations
- Keep Tor Browser updated to latest version
- Never maximize Tor Browser window
- Disable JavaScript in Tor Browser for safety
- Never login to personal accounts on Tor
- Use VPN before connecting to Tor for extra layer

### Operational Security (OPSEC)
- Never reveal real identity on dark web
- Create separate investigative identity
- Never reuse usernames from surface web
- Use separate email for dark web research
- Never share investigation details publicly
- Document findings securely and privately
- Assume you are being monitored at all times

### Legal Considerations
- Viewing freely available dark web content is generally legal
- Purchasing illegal goods or services is illegal
- Downloading illegal content is illegal
- Participating in criminal forums may be illegal
- Always consult legal guidelines before investigation
- Law enforcement activity on dark web is active

---


## Ransomware Leak Sites
- Modern ransomware gangs operate leak sites on dark web
- They post stolen data if victim refuses to pay
- Monitoring these sites is important for threat intelligence
- Major ransomware groups with leak sites:
  - LockBit
  - ALPHV BlackCat
  - Cl0p
  - BlackBasta
  - Hive (taken down by FBI)
- Tools to monitor: ransomwatch.telemetry.ltd

---

## OSINT Without Accessing Dark Web
- Many dark web findings are indexed on surface web
- IntelX indexes dark web content on surface web
- Dehashed contains breach data without dark web access
- Ransomware leak site monitors work on surface web
- Threat intelligence feeds aggregate dark web data
- This approach is safer for most investigators

---

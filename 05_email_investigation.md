# Email Investigation

## What is Email Investigation?
- Email investigation is the process of gathering information linked to an email address
- It is used to verify identity, trace senders, and find linked accounts
- It is one of the most powerful OSINT techniques
- A single email address can reveal a lot about a person or organization
- Used by ethical hackers, investigators, and security researchers

---

## Why Email Investigation is Important in OSINT?
- Reveals identity of a person behind an email
- Finds linked social media accounts
- Checks if email was involved in data breaches
- Helps trace phishing emails back to source
- Verifies if an email address is real or fake
- Finds organization and job role of a person

---

## What Can Be Found From an Email Address?
- Full name of the owner
- Organization or company name
- Job title or role
- Linked social media profiles
- Phone number hints
- Location information
- Data breach history
- Whether email is active or not
- Spam or abuse reports
- Profile pictures linked to email

---

## Email Investigation Techniques

### Email Verification
- Checking if an email address actually exists
- Verifying if the mailbox is active
- Done without sending an actual email
- Uses SMTP verification method

### Reverse Email Search
- Searching the email address across internet
- Finds profiles, forums, registrations linked to that email
- Reveals username patterns used by the target

### Email Header Analysis
- Every email contains a header with technical details
- Header reveals the path email traveled
- Can find original IP address of sender
- Reveals email client used
- Shows mail servers involved in delivery
- Helps detect spoofed or fake emails

### Data Breach Search
- Checking if email was part of any data breach
- Breached data can contain passwords, usernames, phone numbers
- Very useful for building a profile of target

### Social Media Account Search
- Many platforms use email for registration
- Searching email on platforms can reveal linked accounts
- Password reset pages sometimes confirm if email is registered

---

## How to Read Email Headers

### What Email Headers Contain
- From → sender email address
- To → receiver email address
- Date → date and time email was sent
- Subject → subject of email
- Received → list of servers email passed through
- X-Originating-IP → original IP of sender
- Message-ID → unique identifier of email
- MIME-Version → format of email
- Content-Type → type of content in email
- Return-Path → address for bounced emails

### How to Get Email Headers
- Gmail → three dots → Show Original
- Outlook → File → Properties → Internet Headers
- Yahoo Mail → More → View Raw Message

### Analyzing Received Headers
- Read from bottom to top
- Bottom entry is where email originated
- Top entry is where email was received
- Each hop shows server name, IP, and timestamp

---

## Email Spoofing Detection
- Email spoofing means faking the sender address
- Can be detected by checking email headers
- SPF, DKIM, DMARC records help detect spoofing

### SPF (Sender Policy Framework)
- Defines which mail servers are allowed to send email for a domain
- If email comes from unauthorized server SPF fails

### DKIM (DomainKeys Identified Mail)
- Adds a digital signature to emails
- Verifies that email was not modified in transit

### DMARC (Domain-based Message Authentication)
- Combines SPF and DKIM
- Tells receiving server what to do if SPF or DKIM fails
- Can instruct to reject or quarantine suspicious emails

---

## Email Format Patterns
- Many organizations follow a pattern for email addresses
- Knowing the pattern helps guess email addresses of employees
- Common patterns:
  - firstname@company.com
  - firstname.lastname@company.com
  - f.lastname@company.com
  - firstname.l@company.com
  - flastname@company.com

---

## Tools for Email Investigation

### haveibeenpwned.com
- Checks if email was involved in any data breach
- Shows which breaches the email appeared in
- Free to use

### hunter.io
- Finds email addresses linked to a domain
- Reveals email format pattern of an organization
- Verifies if an email address is valid

### emailrep.io
- Shows reputation score of an email address
- Reveals if email is linked to social media
- Shows if email is suspicious or malicious

### epieos.com
- Finds Google account linked to an email
- Finds social media profiles linked to email
- Shows profile picture linked to Google account

### holehe
- Python tool for checking if email is registered on websites
- Checks 120+ websites silently without sending emails
```bash
holehe target@email.com
```

### theHarvester
- Collects emails from public sources like Google, Bing
- Used in reconnaissance phase
```bash
theHarvester -d company.com -b google
```

### mxtoolbox.com
- Analyzes email headers
- Checks SPF, DKIM, DMARC records
- Checks if domain is blacklisted

### infoga
- Python tool for email OSINT
- Gathers information from public sources
```bash
infoga --domain company.com --source all
```

### EmailHippo
- Verifies if email address exists
- Checks if mailbox is active

---

## Online Tools for Email Header Analysis
- mxtoolbox.com/EmailHeaders
- mail-header-analyzer.com
- google admin toolbox → messageheader
- emailheaderanalyzer.com

---

## Data Breach Databases
- haveibeenpwned.com
- dehashed.com
- intelx.io
- breachdirectory.org
- snusbase.com

---

## Email Investigation in Cybersecurity Use Cases
- Tracing phishing email back to attacker
- Finding if corporate email was leaked in breach
- Identifying fake or disposable email addresses
- Mapping employee email addresses of a target organization
- Finding personal accounts of a target using work email patterns
- Investigating spam or harassment emails

---

## Disposable Email Detection
- Attackers often use disposable or temporary emails
- These emails expire after short time
- Can be detected using email reputation tools
- Common disposable email services: tempmail, guerrillamail, mailinator

---



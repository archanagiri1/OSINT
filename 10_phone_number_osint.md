# Phone Number OSINT

## What is Phone Number OSINT?
- Phone Number OSINT is the process of gathering information
  linked to a phone number
- A phone number can reveal identity, location, and online presence
- It is one of the most direct ways to find personal information
- Used by ethical hackers, investigators, and security researchers
- A single phone number can be starting point for full investigation

---

## Why Phone Number OSINT is Important?
- Reveals identity of unknown caller
- Finds social media accounts linked to number
- Verifies if number is real or fake
- Detects spam and scam numbers
- Finds carrier and country of origin
- Helps trace harassing or threatening calls
- Used in fraud investigation
- Helps verify identity of a person during investigation

---

## What Can Be Found From a Phone Number?
- Full name of owner
- Country and region of number
- Carrier or network provider
- Number type (mobile, landline, VoIP)
- Linked social media accounts
- Linked email addresses
- Profile pictures linked to number
- Spam or scam reports
- Business name if business number
- Address hints
- Online accounts registered with number
- Whether number is active or disconnected
- WhatsApp and Telegram account linked
- Truecaller name and spam rating

---

## Phone Number Formats and Structure

### International Format
- Phone numbers follow E.164 international format
- Format: + Country Code + Area Code + Number
- Example: +91 98765 43210 (India)
- Example: +1 212 555 0100 (USA)

### Country Codes
- +1 → USA and Canada
- +44 → United Kingdom
- +91 → India
- +86 → China
- +61 → Australia
- +49 → Germany
- +33 → France
- +7 → Russia
- +92 → Pakistan
- +880 → Bangladesh

### Number Types
- Mobile number → assigned to SIM card
- Landline number → fixed to physical location
- VoIP number → internet based phone number
- Toll free number → 1800 type numbers
- Premium rate number → charged at higher rate
- Virtual number → temporary or disposable number

---

## Phone Number OSINT Techniques

### Reverse Phone Lookup
- Searching phone number to find owner details
- Works best for landline and business numbers
- Mobile numbers harder to find due to privacy
- Many online tools available for reverse lookup

### Carrier and Country Lookup
- Finding which carrier issued the number
- Finding which country number belongs to
- Helps determine if number is real or VoIP
- VoIP numbers are often used for scams and fraud

### Social Media Account Search
- Many platforms allow login or signup with phone number
- Password reset pages can confirm if number is registered
- WhatsApp and Telegram show profile picture and name
- Facebook allows searching by phone number sometimes

### WhatsApp Investigation
- Add number to contacts and open WhatsApp
- Profile picture visible even without accepting contact
- Last seen and online status visible if not hidden
- About section may contain information
- Profile picture can be reverse searched

### Telegram Investigation
- Search phone number in Telegram search
- If person has username it may appear
- Profile picture visible
- Username linked to number can be found

### Google Dorking for Phone Number
- Searching phone number in quotes on Google
- Finds mentions of number on websites and forums
- Reveals business listings, complaints, scam reports
- Example: "9876543210"
- Example: "+91 9876543210"

### Data Breach Search
- Phone numbers are often leaked in data breaches
- Breach databases contain numbers linked to emails
- Helps find email address linked to phone number

---

## Phone Number OSINT Tools

### Truecaller
- Most popular caller identification app
- Crowdsourced database of phone numbers
- Shows name, spam rating, and location
- Website: truecaller.com
- App available on Android and iOS

### PhoneInfoga
- Most powerful open source phone number OSINT tool
- Written in Python
- Gathers information from multiple sources
- Finds carrier, country, social media accounts

### NumVerify
- Phone number validation and lookup API
- Verifies if number is real and active
- Returns carrier, country, number type
- Website: numverify.com

### Sync.me
- Caller identification service
- Shows name and social media profile
- Website: sync.me

### GetContact
- Crowdsourced caller identification
- Shows how number is saved in other peoples contacts
- Reveals nickname or name used for that number
- Website: getcontact.com
- App available on Android and iOS

### Eyecon
- Caller identification app
- Links phone number to social media profiles
- Shows Facebook and LinkedIn profiles

### SpyDialer
- Reverse phone lookup tool
- Free basic lookup service
- Website: spydialer.com

### Whitepages
- Comprehensive people search
- Good for USA landline numbers
- Website: whitepages.com

### AnyWho
- Reverse phone lookup for USA numbers
- Website: anywho.com

### 800notes
- Community based spam number reporting
- Find reports about suspicious numbers
- Website: 800notes.com

### Should I Answer
- Community spam number database
- Shows if number is reported as spam or scam
- Website: shouldianswer.com

---

## WhatsApp OSINT Detailed

### Information Visible on WhatsApp
- Profile picture
- About or status message
- Last seen timestamp
- Online status
- Profile name

### WhatsApp OSINT Steps
- Save number in phone contacts
- Open WhatsApp and search contact
- Check profile picture and save it
- Note about section information
- Check last seen for activity patterns
- Reverse search profile picture on Google and Yandex

### WhatsApp Profile Picture Analysis
- Download profile picture
- Run reverse image search
- Find other accounts using same picture
- Extract EXIF data if original photo

### WhatsApp Group Search
- Some WhatsApp groups have invite links shared publicly
- Group links indexed by Google
- Search: site:chat.whatsapp.com "keyword"
- Can reveal groups target is part of

---

## Telegram OSINT Detailed

### Information Visible on Telegram
- Username if set
- Profile picture
- Bio section
- Phone number if not hidden
- Online status

### Telegram OSINT Steps
- Search phone number in Telegram search bar
- If account found note username and profile details
- Check bio for linked accounts and information
- Reverse search profile picture
- Search username on other platforms

### Telegram Username Search
- Telegram usernames are unique and public
- Search username directly in Telegram
- Use website: t.me/username
- Search username on Google for public mentions

### Telegram Group and Channel Search
- Search target related keywords in Telegram
- Find groups and channels target may be part of
- Tools: tgstat.com, telemetr.io

---

## Number Spoofing Awareness
- Phone number spoofing means faking caller ID
- Scammers use spoofed numbers to impersonate others
- A number showing on caller ID may not be real source
- Spoofed calls still go through real carrier infrastructure
- Truecaller and spam databases help identify spoofed scam calls

---

## VoIP Number Investigation
- VoIP numbers are internet based
- Harder to trace than regular carrier numbers
- Often used by scammers and fraudsters
- Common VoIP providers: Google Voice, Skype, TextNow, Burner
- Signs of VoIP number:
  - NumVerify shows VoIP type
  - Number not found on Truecaller
  - No carrier location matches claimed location
  - Number can be from any country

---

## Disposable and Virtual Number Detection
- Temporary numbers used to bypass verification
- Services: receive-sms-online.com, tempnumber.com
- Signs of disposable number:
  - Number shows up on receive-sms websites
  - No social media accounts linked
  - Not found on Truecaller
  - Very recently activated

---

## Phone Number to Email Discovery
- Data breach databases link numbers to emails
- Some platforms show email in profile
- Password reset flow on some sites confirms email linked to number
- Tools: dehashed.com, intelx.io

---

## Phone Number OSINT in Cybersecurity Use Cases
- Investigating spam and scam callers
- Tracing harassing phone calls
- Verifying identity of unknown contacts
- Finding accounts linked to suspicious number
- Fraud investigation and due diligence
- Social engineering awareness training
- Finding leaked numbers in data breaches
- Investigating phishing SMS (smishing) campaigns
- Identifying fake accounts using virtual numbers

---

## SMS Phishing (Smishing) Investigation
- Smishing is phishing done via SMS
- Investigate suspicious SMS by:
  - Looking up sender number on Truecaller
  - Checking number on spam databases
  - Analyzing link in SMS using VirusTotal
  - Searching number on Google for scam reports
  - Checking carrier type for VoIP indicators

---


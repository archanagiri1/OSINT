# Social Media OSINT

## What is Social Media OSINT?
- Social Media OSINT is the process of collecting publicly available
  information from social media platforms
- It is used to build a detailed profile of a target
- Social media is one of the richest sources of OSINT data
- People voluntarily share personal information on social media
- Used by ethical hackers, investigators, journalists, and researchers
- Also called Social Media Intelligence (SOCMINT)

---

## Why Social Media OSINT is Important?
- People share massive amounts of personal data on social media
- Reveals real name, location, workplace, and daily routine
- Finds friends, family, and connections of target
- Reveals interests, hobbies, and opinions
- Photos and videos can reveal location and identity
- Old posts can reveal information person forgot they shared
- Helps build complete profile of a target for investigation
- Used in background checks and due diligence

---

## What Can Be Found From Social Media?
- Full name and username
- Profile picture and photos
- Date of birth
- Location and home city
- Workplace and job title
- Education history
- Relationship status
- Friends and family members
- Daily routine and habits
- Phone number and email
- Political and religious views
- Travel history
- Financial hints
- Vehicle information
- Linked accounts on other platforms

---

## General Social Media OSINT Techniques

### Profile Analysis
- Reading all publicly available profile information
- Checking bio, about section, contact info
- Noting all linked accounts and websites
- Checking profile picture and cover photo

### Post and Content Analysis
- Reading through posts and tweets
- Analyzing writing style and tone
- Finding location clues in posts
- Finding date and time patterns of activity
- Identifying frequent topics and interests

### Photo and Video Analysis
- Extracting location from photo backgrounds
- Identifying people in photos
- Checking tagged locations
- Analyzing metadata if available
- Reverse searching profile pictures

### Connection Analysis
- Analyzing friends and followers list
- Finding mutual connections
- Identifying family members from tagged posts
- Mapping social network of target

### Historical Post Analysis
- Scrolling through old posts
- Using archive tools to find deleted posts
- Checking Wayback Machine for old profiles
- Finding information shared years ago

---

## Platform Specific OSINT

### Facebook

#### What Can Be Found
- Full name and username
- Date of birth
- Current city and hometown
- Workplace and education
- Relationship status and family members
- Friends list
- Check ins and locations visited
- Photos and tagged photos
- Groups joined
- Pages liked
- Events attended
- Phone number and email if not hidden

#### Facebook OSINT Techniques
- Search full name in Facebook search
- Check About section for all personal details
- Check Photos section for location clues
- Check Friends list for connections
- Check Groups for interests and community
- Check Check-ins for frequent locations
- Use Facebook Graph Search for advanced queries
- Search email or phone number in Facebook search
- Check tagged photos for events and people

#### Facebook Specific Tools
- sowsearch.info
- Facebook search bar with filters
- stalkscan.com (archived)
- lookup-id.com (find Facebook ID)

---

### Instagram

#### What Can Be Found
- Username and full name
- Bio and contact information
- Profile picture
- Photos and videos posted
- Tagged photos by others
- Location tags on posts
- Followers and following list
- Linked Facebook and Twitter accounts
- Stories highlights
- Reels and tagged content

#### Instagram OSINT Techniques
- Check bio for contact info and linked accounts
- Check tagged photos for events and people
- Check location tags for frequent places
- Analyze followers and following for connections
- Check story highlights for old content
- Use Google dorking: site:instagram.com username
- Reverse search profile picture
- Check tagged location pages for target photos

#### Instagram Specific Tools
- imginn.com (view without account)
- picuki.com (Instagram viewer)
- inflact.com
- Google dorking for Instagram profiles

---

### Twitter / X

#### What Can Be Found
- Username and display name
- Bio and location
- Website linked in bio
- Tweets and replies
- Liked tweets
- Following and followers list
- Pinned tweet
- Joined date
- Media posted
- Quoted and retweeted content

#### Twitter OSINT Techniques
- Read bio for personal details and links
- Analyze tweet history for interests and opinions
- Check replies for conversations and connections
- Search username on Google for mentions
- Use Twitter advanced search for specific keywords
- Check liked tweets for interests
- Use Wayback Machine for deleted tweets
- Search by location in Twitter advanced search
- Check lists created or followed

#### Twitter Advanced Search Operators
- from:username → tweets from specific user
- to:username → tweets sent to specific user
- @username → mentions of username
- since:2020-01-01 → tweets after date
- until:2023-12-31 → tweets before date
- near:city → tweets from location
- geocode:lat,long,radius → tweets from coordinates
- filter:media → tweets with media only
- filter:links → tweets with links only

#### Twitter Specific Tools
- tweetdeck.twitter.com
- socialbearing.com
- tinfoleak.com
- twint (Python tool for scraping tweets)

---

### LinkedIn

#### What Can Be Found
- Full name and profile picture
- Current job title and company
- Past work experience
- Education history
- Skills and endorsements
- Connections and network
- Posts and articles written
- Recommendations received
- Volunteer work
- Certifications and licenses
- Languages spoken
- Contact info if shared

#### LinkedIn OSINT Techniques
- Search full name with company name
- Check work history for career timeline
- Check education for graduation year and university
- Check connections for network mapping
- Check posts for opinions and activities
- Use LinkedIn search filters for precise targeting
- Search company page for employee list
- Check recommendations for colleague names
- Use Google dorking: site:linkedin.com/in/ "name"

#### LinkedIn Specific Tools
- LinkedIn search filters
- Google dorking for LinkedIn profiles
- hunter.io for finding emails from LinkedIn profiles
- RocketReach for contact information

---


### Reddit

#### What Can Be Found
- Username and profile picture
- Post history across subreddits
- Comment history
- Upvoted and saved posts if public
- Cake day (account creation date)
- Karma score
- Subreddits moderated
- Awards given and received

#### Reddit OSINT Techniques
- Read full post and comment history
- Note which subreddits user is active in
- Analyze writing style and topics
- Look for personal details mentioned in posts
- Use Reddit search for username mentions
- Check post history for location clues
- Use Google dorking: site:reddit.com username

#### Reddit Specific Tools
- camas.unddit.com (search deleted posts)
- redditmetis.com (user analysis)
- pushshift.io (historical Reddit data)
- unddit.com (view deleted comments)

---

### YouTube

#### What Can Be Found
- Channel name and profile picture
- About section with links
- Videos uploaded
- Playlists created
- Comments on videos
- Subscriptions if public
- Location if shared
- Joined date

#### YouTube OSINT Techniques
- Read about section for links and contact
- Analyze video content for location clues
- Check comments for interactions
- Search channel name on other platforms
- Check video metadata for upload patterns
- Reverse search profile picture

---

## Social Media OSINT Tools

### Maltego
- Most powerful OSINT and link analysis tool
- Visualizes connections between entities
- Has many social media transforms
- Used by professional investigators

### Social Searcher
- Searches across multiple social media platforms
- Finds mentions of name or keyword
- Website: social-searcher.com

### Spokeo
- People search engine
- Aggregates social media and public records
- Website: spokeo.com

### Pipl
- Deep web people search
- Finds social media profiles and public records



### Sherlock
- Finds username across 300+ platforms
- Useful for cross platform social media search

---

## Archive and Deleted Content Recovery

### Wayback Machine
- Archives web pages including social media profiles
- Find old versions of profiles
- Recover deleted posts and information
- Website: web.archive.org

### Google Cache
- Google caches pages before they are deleted
- Search: cache:instagram.com/username

### Cached Tweet Tools
- camas.unddit.com for Reddit
- snapbird.org for old tweets
- twaku.com for tweet archives

---

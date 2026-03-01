# Username Search

## What is Username Search?
- Username search is the process of finding all accounts linked to a specific username
- It is used to build a profile of a target across multiple platforms
- A person often uses the same username on many websites
- It is one of the easiest and most effective OSINT techniques
- Also called Username Enumeration or Account Discovery

---

## Why Username Search is Important in OSINT?
- Reveals all online presence of a target
- Finds social media accounts across platforms
- Discovers forum and community accounts
- Reveals hobbies, interests, and activities of target
- Can lead to real name, email, location discovery
- Helps connect multiple identities of same person
- Finds old or forgotten accounts with sensitive information

---

## What Can Be Found From a Username?
- Social media profiles (Facebook, Instagram, Twitter, TikTok)
- Forum accounts (Reddit, Hackforums, RaidForums)
- Gaming accounts (Steam, Xbox, PlayStation)
- Developer accounts (GitHub, GitLab, Stack Overflow)
- Shopping accounts (Amazon, eBay)
- Dating app profiles
- Real name linked to username
- Profile pictures across platforms
- Location hints from posts and bio
- Email address hints
- Phone number hints
- Interests and daily activities
- Friends and connections

---

## Username Pattern Analysis
- People often follow patterns when creating usernames
- Analyzing patterns helps find other accounts
- Common patterns:
  - firstname + lastname → johnsmith
  - firstname + numbers → john123
  - nickname + year of birth → darkwolf1999
  - initials + lastname → jsmith
  - random words combined → bluefoxhunter
- If one username is found, try variations like:
  - Adding numbers at end → username123
  - Adding underscore → user_name
  - Adding dots → user.name
  - Adding country code → username_in
  - Adding year → username2001

---

## Username Search Techniques

### Direct Platform Search
- Manually searching username on each platform
- Checking profile URL patterns
- Example: instagram.com/username, twitter.com/username

### Automated Username Search
- Using tools that check hundreds of platforms at once
- Faster and more efficient than manual search
- Tools like Sherlock, WhatsMyName

### Reverse Image Search from Profile Picture
- Downloading profile picture from one account
- Searching same image on other platforms
- Reveals accounts using same profile picture

### Google Dorking for Username
- Using Google search operators to find username
- Example: "username" site:twitter.com
- Example: "username" site:reddit.com
- Example: "username" inurl:profile

### Search Engine Search
- Simply searching username in quotes on Google
- Example: "darkwolf1999"
- Finds mentions, posts, profiles across internet

---

## Platform Specific Username Search

### GitHub
- github.com/username
- Reveals repositories, contributions, email sometimes
- Shows programming languages and projects
- Can reveal real name and location

### Reddit
- reddit.com/user/username
- Shows post history, comments, subreddits joined
- Can reveal interests, location, opinions

### Twitter / X
- twitter.com/username
- Shows tweets, followers, following
- Bio often contains real name, location, website

### Instagram
- instagram.com/username
- Shows photos, location tags, tagged people
- Bio may contain real name and contact

### LinkedIn
- linkedin.com/in/username
- Shows work history, education, skills
- Real name and organization almost always visible

### Steam
- steamcommunity.com/id/username
- Shows games, playtime, friends
- Can reveal real name if not hidden

### TikTok
- tiktok.com/@username
- Shows videos, bio, linked accounts
- Location sometimes visible in videos

---

## Cross Platform Username Correlation
- Finding same person across multiple platforms using username
- Steps:
  - Find username on one platform
  - Use tools to find same username on other platforms
  - Compare profile pictures, bio, writing style
  - Look for same email patterns mentioned
  - Check if linked accounts are mentioned in bio
  - Map all accounts together to build full profile

---

## Username Search for Threat Intelligence
- Finding hacker usernames on dark web forums
- Tracking cybercriminal activity across platforms
- Finding leaked credentials linked to username
- Identifying sock puppet accounts (fake identities)
- Connecting aliases used by same threat actor

---

## Avoiding Detection During Username Search
- Use tools that do passive checks only
- Avoid logging into platforms to check
- Some platforms notify users when profile is viewed
- Use VPN or Tor for anonymous searching
- Sherlock and similar tools do not notify targets

---

## Username to Email Discovery
- Some platforms show email in profile
- Password reset pages confirm if username or email exists
- GitHub sometimes exposes email in commit history
- Forum profiles sometimes show contact email
- Tools like holehe can check email linked to username

---


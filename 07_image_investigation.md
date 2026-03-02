# Image Investigation

## What is Image Investigation?
- Image investigation is the process of extracting information from images
- It is used to find the original source of an image
- It helps verify if an image is real or fake
- It can reveal location, identity, and other hidden details
- Also called Image OSINT or Photo Intelligence (PHOTINT)
- One of the most powerful techniques in OSINT investigations

---

## Why Image Investigation is Important in OSINT?
- Verifies authenticity of an image
- Finds original source of a photo
- Reveals location where photo was taken
- Identifies people in photos
- Finds fake profile pictures used by catfishers
- Detects manipulated or edited images
- Finds other accounts using same profile picture
- Reveals camera and device used to take photo
- Helps in missing person investigations
- Used in journalism to verify news photos

---

## What Can Be Found From an Image?
- GPS coordinates of location where photo was taken
- Date and time photo was taken
- Camera model and brand
- Device used (phone or camera)
- Software used to edit image
- Original source website of image
- Other accounts using same image
- Identity of person in image
- Landmarks and location clues in background
- Weather conditions at time of photo
- Other photos taken by same camera

---

## Image Investigation Techniques

### Reverse Image Search
- Uploading image to search engine to find its source
- Finds where image appeared on internet before
- Reveals original upload date and location
- Finds similar or duplicate images
- Detects fake or stolen profile pictures

### EXIF Metadata Extraction
- EXIF stands for Exchangeable Image File Format
- Every photo contains hidden metadata
- Metadata is automatically added by camera or phone
- Contains technical and location information
- Can be viewed using special tools

### Geolocation from Image Content
- Analyzing visual clues inside the image
- Looking for landmarks, signs, buildings
- Checking sun position for direction and time
- Checking vegetation for climate and region
- Checking license plates for country and region
- Checking language on signs for country
- Checking architecture style for region

### Image Manipulation Detection
- Checking if image has been edited or faked
- Looking for inconsistencies in lighting and shadows
- Checking pixel level anomalies
- Using error level analysis (ELA)
- Detecting AI generated images

### Facial Recognition Search
- Searching face in image across internet
- Finding other photos of same person
- Revealing identity of unknown person
- Note: Must be used ethically and legally only

---

## EXIF Metadata Explained

### What is EXIF Data?
- EXIF is hidden data stored inside image files
- Automatically added by camera or smartphone
- Contains technical details about how photo was taken
- Most social media platforms strip EXIF data for privacy
- Photos shared directly via email or messaging may still contain EXIF

### EXIF Data Fields
- GPS Latitude and Longitude → exact location
- GPS Altitude → height above sea level
- Date and Time Original → when photo was taken
- Camera Make → brand of camera (Apple, Samsung, Canon)
- Camera Model → exact model of camera
- Lens Model → lens used for photo
- Focal Length → zoom level used
- Aperture → light setting of camera
- Shutter Speed → exposure time
- ISO Speed → light sensitivity setting
- Flash → whether flash was used
- Orientation → rotation of photo
- Software → editing software used
- Artist → name of photographer sometimes
- Copyright → copyright information

### How to Extract EXIF Data

#### Using ExifTool (Linux/Windows)
```bash
exiftool image.jpg
exiftool -GPS* image.jpg
exiftool -a -u -g1 image.jpg
exiftool -csv image.jpg
exiftool -r /folder/
```

#### Using Online Tools
- exifinfo.org
- exif.regex.info
- metapicz.com
- jimpl.com

---

## Reverse Image Search Tools

### Google Reverse Image Search
- Most popular and widely used
- Go to images.google.com
- Click camera icon and upload image
- Or drag and drop image
- Shows where image appeared on web

### TinEye
- Specialized reverse image search engine
- Tracks image usage across web
- Shows oldest known use of image
- Website: tineye.com

### Yandex Image Search
- Russian search engine with powerful image search
- Often finds results Google misses
- Very good for facial recognition searches
- images.yandex.com

### Bing Visual Search
- Microsoft's image search
- Good for finding similar images
- bing.com/visualsearch

### Google Lens
- AI powered image search by Google
- Identifies objects, landmarks, text in images
- Available on mobile and desktop

---

## Geolocation Techniques

### Finding Location from Landmarks
- Identify buildings, monuments, bridges in background
- Search landmark name to find city and country
- Cross reference with map services

### Finding Location from Street Signs
- Read text on street signs
- Identify language and alphabet
- Search sign text to find location

### Finding Location from License Plates
- Different countries and states have unique plate formats
- Identify plate format to narrow down region

### Finding Location from Vegetation
- Palm trees indicate tropical region
- Pine trees indicate cold or mountain region
- Specific plants can identify continent or country

### Finding Location from Sun Position
- Sun position reveals direction and time of day
- Combined with shadow direction can estimate compass direction
- Tools like SunCalc can help analyze sun position

### Finding Location from Architecture
- Building styles vary by country and region
- Roof styles, window designs, wall materials differ by region
- Electrical poles and wires style varies by country

### Tools for Geolocation
- Google Maps Street View
- Google Earth
- Bing Maps
- suncalc.org
- geospy.ai (AI based geolocation)
- GeoGuessr (practice tool)

---

## Image Manipulation Detection

### Error Level Analysis (ELA)
- Detects areas of image that have been edited
- Edited areas show different compression levels
- Tools: fotoforensics.com, forensically.29a.ch

### Metadata Inconsistency
- Checking if metadata matches claimed photo details
- Date in metadata vs claimed date
- Camera model vs claimed device

### Pixel Analysis
- Checking for copy paste artifacts
- Checking for cloning or patching
- Tools: forensically.29a.ch

### AI Image Detection
- Detecting if image was generated by AI
- AI images have specific artifacts and patterns
- Tools: hivemoderation.com, aiornot.com, illuminarty.ai

---

## Social Media and Image OSINT

### Facebook
- Profile pictures can be reverse searched
- Tagged photos reveal friends and locations
- Check in photos reveal frequent locations

### Instagram
- Location tags reveal where photos were taken
- Tagged accounts reveal connections
- Story highlights can reveal old locations

### Twitter / X
- Profile pictures can be reverse searched
- Images in tweets often contain metadata
- Location can sometimes be enabled on tweets

### LinkedIn
- Profile pictures can be reverse searched
- Background photos can reveal office location

---

## Fake Profile Picture Detection
- Many fake accounts use stolen profile pictures
- Steps to detect:
  - Download profile picture
  - Run reverse image search on Google and TinEye
  - Check if same image appears elsewhere
  - Check if image is from stock photo website
  - Check if image is AI generated

---





# Week 3


## Accessibility -Human Factors to Consider in Web Design (3.01)


### What does a web accessibility coordinator does
- help guide policy and purchasing decisions
- evaluate web interfaces for accessibility
- assist those with disabilities access online material
- keep pace with changing technology



### 1 in 5 prople have a disability (US)
- 60 million people with disabilities in U.S.
- half are impeded when using web based software


### Visual Disabilities
- blindness, low-vision, color-blindness
- 8 million have difficulties reading newspaper even with glasses
- 1.8 million are completely blind
- font size, color contrasts, font style are important aspects of it


### Hearing disabilities
- from partial to total deafness
- 8 million have difficulty hearing a normal conversation
- 1 million are completely deaf
- videos closed-captioning, users might not realize you are showing music


### Motor disabilities
- inability to use a mouse or physical keyboard
    - slow response time or limited fine motor skills
- dexterity issues
    - 8 million americans have difficulty using their arms or hands
- what happens when someone tries to "tab" throught your page, do you require a steady hand?


### Cognitive disabilities
- learning, distraction, dyslexia, memory or focus on large amouts of information
- traumatism (post-traumatic stress disorder, traumatic brain injury)
- actually amout to more people than physical and perceptual disabilities numbers added


### Web offers unprecendented opportunities for disabled
- education (online courses!)
- news
- commerce (Amazon, Ebay)
- social (facebook, chats, etc.)
- benefits of the web are amplified for disabled (at least if done right)


### Web accessibility definition
- making the web accessible for the wides possible audience
- includes Temporarily Able-Bodied users (which we all are)
- online infrastructures is generally hostile to those with disabilities
- inseparable from SEA, mobile and usability: improving one generally improves the others
- can be done through adherence to standards



### W3C WCAG 2.0 (Web Content Accessibility Guidelines)
- principles, not technology-based
- the 4 principles: POUR
    - Perceivable
    - Operable
    - Understandable
    - Robust


### Summary
- design with accessibility in mid is the right thing to do for many reasons
- adhering to standards (not flashy, cool effects) is key
- pay special attention to the semantics behind the HTML5 tags (and use them accordingly)
- check out the WAVE tool for accessibility @ http://wave.webaim.org/



## Validating your site (3.02)

### Why validate?
- browsers are robust and fix common mistakes (but you should never rely on it)
- often, can break websites when gets too big and rely on auto-fixing

### Three (validator w3.org)
- URL validation
- Filename validation
- Direct input validation


### Summary
- validated sites are more robust than unvalidated




## Putting your code on the web (web hosting)


### What is needed?
- domain name
- hosting service

### Domain name
- typically purchased for multiple years at a time
- most is .com but other extensions are gaining acceptance
- by themselves, domain names are useless


### Hosting services
- what is your URL right now?
- need a registered IP address to connect with your domain names
- hosting services types
    - free
    - mid-range
    - full-service


### Free services
- little or no control of domain name
- limited tools
- advertising and redirects, bothersome when typos
- good to start learning


### Paid services
- tend to have better tools
- support is available (at least better than free services)


### Byethost
- recommended to start
- https://byethost.com
- remember the password (pretty hard to get it back)
- check your spam to get instructions



## cPanel (3.04)

### Overview
- interface to manage website
- good to post website


### Connecting to cPanel
- need to have the URL for CPanel account
    - usually a variation of domain name or hosting service domain name

### public_html
- regardless of the cPanel configuration, every syste should have a file manager
- search for the public_html directory (could be named "public")
- what is inside it should be supposed to be viewed by everyone


### Working locally
- possible to edit your files via cPanel but maybe not a good idea
    - changes are immediately public
    - less opportunity to test and debug
- ideally, work locally, test, and then apply small fixes if needed


### Summary
- versions of cPanel often differ depending on paid or free sites
- offers many admnistrative tools (email accounts, database management, cron jobs)
- an alternative is to use sftp to transfer files



## sftp (3.05)

### Secure File Transfer Protocol
- common way to transfer files is with FTP/SFTP


### What is needed?
- need a SFTP client


### Summary
- can upload your files many ways
- make sure you know your login information




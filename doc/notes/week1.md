# week 1: Html5

## History and Evolution

### Html files
- structured multimedia files
- long history


### Learning curve
- first learn syntax and then semantics

### Html1 history overview
- 1990, connect data via hypertext files (through hyperlinks)
- about content, not layout (CERN...)
- keep it simple, content-based
- was pushed for layout (1993, Mosaic graphical browser, 341x adoption)


### Browser wars
- proprietary tags (blink, marquee which were browser specific)
- sometimes, could not display colors due to hardware
- created "Best Viewed On" comments...


### Web Standards (organizations)
- no one runs the internet or the web (but some take roles)
    - IETF (internet engineering task force)
    - W3C (World Wide Web Consortium)
    - WAI (Web Accessibility Initiative)


### Web conventions timeline
- 1990-1994: simple text-based html
- 1993-1994: mosaic, graphical browsers
- 1995-1999: cross-browser compatibility fuckups (browser wars)
- 2000-2005: content vs. style separation initiated
- 2005-2008: HTML + CSS becomes new standard


### HTML evolution
- 1993: 1.0. Tim Berners-Lee
- 1995: 2.0. IETF RFC to include stylized text and tables
- 1996: CSS 1
- 1997: 3.2. W3C; included browser specific features (browser wars)
- 1998: CSS 2
- 1999: 4.0. Different document types
- 2012: 5. Back to HTML + semantic tags


### Current state
- HTML5 is cooperation between W3C and WHATWG (Web Hypertext Application Technology Working Group)
- Guidelines
    - build from HTML, CSS, DOM and Javascript
    - Reduce need for external plugins (e.g. Flash)
    - Markup to replace scripting (macros basically)
    - Device Independence (you wish)


### Review
- HTML
    - file describing content, not style (UI)
    - purpose of facilitating content types (multimedia)
- HTML5
    - brought by the presence of non compatible extensions
    - aims at simplicity and composability



## How it works (page requests)

### Some Lingo
- Networks
    - LAN: Local Area Network, e.g. shared printers
    - WAN: Wide Area Network,  e.g. enterprise network or the internet itself

- Client/Server
    - Server: holds shared resources, always connected
    - Client: make the requests, user's interface

- Request/Response cycle
    - what happens when client REQUESTS a page and server RESPONDS it with (hopefully) appropriate files

- URL (Uniform Resource Locator, expression of a request)
    - 3 parts
        - protocol: how to understand the request
        - domain: to whom the request is addressed
        - document: which specific file client wants

- Protocols
    - HTTP(S): (Secure) Hypertext Transfer Protocol
    - (S)FTP: (Secure/SSH) File Transfer Protocol: more generic

- Domain Names
    - Indentifies an entity to connect to
    - Different top-level domains (umich.[edu], google.[com], wikipedia.[org])
        - edu: education institutions
        - com: buisness
        - org: non-profit organization
        - de/ca/.. : countries
        - ... many others
    - Managed by ICAAN (Internet Corporation for Assigned Names and Numbers)


### IP Addresses and the Domain Name Server (DNS)
- Internet Protocol Version (Ipv4)
    - uses format xxx.xxx.xxx.xxx
    - identifies each domain
    - can represent 2^32 permutations

- DNS (domain name server) maps domain -> IP address
    - think of it as a Dictionary<String, Integer>
    - that way there's no need to remember the huge IP address

### Document
- URLs can ask for specific document
    - http://www.intro-webdesign.com/[contact.html]
    - usually there's a default fallback if no domcument is specified
        - index.html is a convention
- Most web pages are actually a compound of many files

### Request
- workflow
    1- IP address is determined (through DNS if needed)
    2- browser creates HTTP request
        - hides lot of meta-information (header, cookies, form data, others...)


### Response
- files are returned (not beautiful, well-formatted web pages)
    - the internet browser used reads, understands and present content as well as possible
- error codes are returned if the server cannot fulfill the request
    - e.g. 404, 500 and other standard error codes


### Request-response cycle
- example flow
    1- Browser looks up the domain in the DNS
    2- DNS returns the IP address (hopefully)
    3- Browser formulates and sends HTTP request to the server at said address
    4- Server fulffils the request and sends it back as response
    5- Browser renders the response
        - formulates appropriate requests for linked resources (e.g. embedded video)


### Additional Notes
- IPV6 increases length of IP addresses to allow for 2^128 permutations

### Summary
- URL (Uniform Resource Locator) has 3 parts
- Request-Response cycle usually requires multiple iterations of request-response


## Browsers

### Differing browsers
- various pro/cons (no obvious winners)
- users get used to a browsers or have some unique features
    - must develop for many target browsers and test

- Comparisons
    - Internet Explorer
        - one of the most popular
        - installed by default and free
        - unavailable as is on many OS (operating systems, particularly linux and mac)
    - Safari
        - works on mac and windows
        - not on linux
    - Chrome
        - Mac, Windows and Linux
        - very fast
        - greater security (compared to Internet Explorer)
    - Firefox
        - very fast
        - very secure
        - lots of developer tools
        - more resource heavy (slows down computer)

- Different market shares for each browsers (October 2014, rounded to nearest)
    - IE11    24%
    - Chrome  21%
    - IE8     17%
    - Firefox 14%
    - IE9     9 %
    - IE10    6 %
    - Safari  5 %
    - Others  4 %

### Summary
- variable respect for HTML5 standards
    - details tag doesn't work on Firefox
- should test on at least 2 different browsers, if not all



## How to use an editor to create an HTML file

### Creating and editing files
- protips
    1- organize files into a sensible naming and folder schema
    2- choose a naming convention
        - under_scores, camelCase (let's use dashes '-')
        - no spaces in file names, consistent capitalization
    3- choose text editor
        - Sublime, Notepad, etc... (I'll go with Kate and see where it takes me)
    4- type code by hand
    5- always save files in UTF-8 format


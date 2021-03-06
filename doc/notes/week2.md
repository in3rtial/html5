# Week 2


## DOM (Document Object Model)

### Basics of DOM
- basis of HTML5 is that HTML, CSS, DOM and Javascript are the basic building blocks

- DOM provides tree-like structures that pages should follow (template of sorts)

- CS (Computer Science) people love trees (that they do)

- HTML is built on the DOM
    - root structure (<html>)
    - head, body, etc...

- 3 parts of a well-formed document (HTML5)
    1- doctype: version of HTML under use
        - tag: <!DOCTYPE html>
        - much simpler now in html5
    2- head: some metadata; mostly invisible to user (except title)
        - tag: <head>
        - metadata: language, title
        - supporting files: javascript, styling, add-ons (dependencies)
        - title is the name displayed on the tab
    3- body: content to display; 

### Validators
- can validate the code using online parsers/checkers
    - often forget to close tags
    - evaluation of the actual number of errors is hard (cascade of errors...)
    - browsers often correct mistakes making mistakes invisible which is dangerous
- looking good is no substitution for good testing


## HTML5 Tags and Syntax (generics)


### Tags basics
- tags have a beginning <x> and ending tag </x> (where x is any tag)
    - some tags are self-closing (<img src="x.gif"> includes all necessary information)
    - some tags have attributes

- tags documentation is easily available online


### Display
- important attribute of an element is its display
    - block
        - take amount of width and height
        - 
    - inline
        - take as much space as needed

### Common tags
- headings [block]
    - <h1>..<h6>
    - can have syntax and semantics
    - don't juste take into account the looks, rank by importance
    - can confuse the user
- paragraphs [block]
    - <p> .. </p>
    - should only contain inline elements

- divs [block]
    - <div> .. </div>
    - generic section
    - larger than paragraph
    - lack semantics

- ordered lists [inline]
    - <ol> <li> item1 </li> <li> ... </li> </ol>

- unordered lists [inline]
    - <ul> <li> item1 </li> <li> item2 </li> </ul>


- line breaks [inline]
    - <br>
    - self-closing


### Attributes
- additional information about an element
    - often facultative

- always specified in the opening of a tag (not closing)

- attributes come in pairs [key:value]


### Images (example of attributes)
- <img src="frontImage.jpg" alt="front image">
- images rarely work the first time (many possible problems)
    - too big, too smal, broken link, etc.
- choose intelligent image size and naming convention to avoid common problems
- real-world would look something like <img src="logo.jpg" alt="company logo" title="..." ...>


### More Attributes
- as you learn the tags, you learn their specific attributes
- some attributes are shared by all tags
    - class
        - applies special properties to groups of elements
        - to apply style over subset of elements
    - id
        - specifies a unique id to one element of the document
        - provides unique identifier
    - style
        - avoid at all cost
        - used to be popular (but with style-content separation, it makes little sense)
    - acceskey
        - shortcut key to activate an element
        - very important to accessibility
    - tabindex
        - which order people get to in the page
        - 1 is the highest priority possible (bigger tab index = smaller priority)

### Special Entitites
- to display used symbols, must use special entities
    - < : &lt
    - > : &gt
    - copyright symbol : &copy
    - blank space : &nbsp
    - cent : &cent
    - & : &amp

### Summary
- difference between a tag and an attribute
    - look for the <> brackets
- what two symbols end a self-closing tag
    - </x>



## Sematic Tags

### How to design
- the most important step in web design is design
- need a good idea of what you want


### Using semantic tags
- div used to be very popular
    - used to have different class attributes

### <header>
- introductory or navigational aids
    - title
    - navigation links (wikipedia style)


### <nav>
- a section of the page that link to other pages or to parts within the page

    <nav>
        <ul>
            <li><a href="overview">Overview</a></li>
            <li><a href="history">History</a></li>
        </ul>
    </nav>

- often found in the header tag


### <footer>
- usually contains info such as copyright data, related documents, links to social medias
- typically at the bottom of the page, but not required!
    - won't show up at bottom if you place it elsewhere


### <figure>
- more semantics (and information) than <img>
    - caption <figcaption>
    - multiple multi-media resources



## Template
- please see week2-index.html



## Images

### Image Formats
- many file types are supported
    - JPEG, gif, png
    - SVG and BMP are additional options
    - file extensions must be included
- size of images is important because they are downloaded
- every image requires an HTTP Request

### Image Sizes
- browser will display the image in its original size (which is usually not good)
    - quick solution is to change file or use width/height attributes

- img tag includes width and height attributes
    - breaks the style/content separation
    - can set height and width independently
    - can set both, but doesn't preserve aspect ratio
    - can also be described in percents (width = "50%")


### Favicon
- can put next to the title of the page in the tab
- must go into the <head> section
- cannot be jpg or gif


### Alternative text attributes
- textual alternative to non-text content
- read by screen readers
- displayed in place of image (in case it is not available)
- provides semantic meaning for search engines


#### Create good alt text
- accurate
- succinct
- not redundant
- no "picture of..." and the likes of it


### Empty alt text
- can be alt=""
    - better than skipping the alt text at all


### Summary
- careful with file extensions and file paths
- for now, style the image inside the html


## Hyperlinks (2.06)

- they create the web


### Anchor links

- syntax: <a href="http://www.umich.edu">University of Michigan</a>
- <a> tag for Anchor link
- needs a hyper-reference and content
    - href is the reference of new content
    - content is the clickable part (can be text, image...)


### Types of links
- absolute
    - <a href="http://intro-webdesign.com/">Web Design</a>
    - links to someone else's page
- relative
    - <a href="page2.html">Second Page</a>
    - links to a local file
    - use on own webpage to avoid having to rename
    - links should never have folders specified
        - e.g. C:/Documents/Doc1.html
- embedded references
    - link to part of the same file (sections)

### Using Images as the link
- clickable component doesn't have to be text
    - <a href="http://www.redcross.org"> <img src="img/img1.png" alt="Logo"/></a>


### Usability issues
- make sure that clickable link component has an informative name
- information in the image should be available to those who can't see the image


### Targets
- anchors take other attributes
    - _self: default action
    - _blank: open in new tab or window (some users don't like)
    - _top and _parent


### Summary
- page without links is extremely rare
- relative, absolute, internal links
- use caution with links (for accessibility)



## Multimedia (2.07)

### HTML5 multimedia
- designed to avoid use of extra software/plugins for multimedia
- not fully implemented (but getting there)


### Video element <video>
- uses a src attribute or embedded <source>
- common attributes
    - height, width
    - autoplay
    - loop
    - controls
- text inside <video>..</video> is displayed if browser cannot support tag


### Audio element <audio>
- src attribute to link to audio file (.mp3 or .wav usually)
- commmon attributes
    - autoplay, controls, loop
    - buffered
    - muted
    - volume
- set clips with #t tag
    - .ext#t=5:25 (begin:start)


### Plugins
- before html5, no standard for multimedia
    - plugins were required
- some browsers might still require Flash



### Accessibility issues
- make sure to provide links to plugins
- include text description and closed captioning (or otherequivalent content)
- multimedia should enhance, not distract



## Tables (2.08)

### Table Design
- sketch the layout before you code
- decide on the number of rows and columns
- decide if any rows/columns will span multiple cells


### Tags
- <table> as container tag
- <tr>..</tr> the rows
- <td>..</td> the columns


### Table heading
- some people use bold fonts
- we'll use semantic tags
    - <th>..</th>, table heading


### Captions
- link text to a table
- <caption>


### Summary
- tables should only be used for tabular data
- draw your table before you code it
- check for unclosed tags





## Useful Tags (2.09)


### Choosing tags
- block tags
    - generic <p> <div>
    - semantic <header> <nav> <footer> <figure>
    - should use semantic tags as much as possible

### Block tags (some unknown)
- containers
    - <article> <aside> <section> <main>
- <hr>
- <address>
- <blockquote> which has a cite attribute
- <details> with <summary>


### Inline tags
- <span> original inline tag for plain text
- <cite>
- <abbr>
- <time>
- <code>
- <sub> and <sup>


### More advanced tags
- <button>
- <meter>
- <progress>
- <iframe> often used to embed documents
    - not very portable
- <bdo> attribute dir (ltr or rtl), bidirectional orientation
- <map> with <area> creates clickable element in image but requires Javascript


### Summary
- use the most specific tag possible
- sometimes tags don't work
    - go through a validator, might be a syntax error
    - run the code in multiple browsers (good idea, even if it looked good)









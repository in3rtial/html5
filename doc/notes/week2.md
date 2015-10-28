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
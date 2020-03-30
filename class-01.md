This is going to be my attempt at the latest read concepts in a tutorial / note like fashion.

### Introduction to HTML + CSS

### web browser 
* peoples access to the internet

### web servers 
* computer that host websites

### web hosting 
* basically a company that will host your site for a fee.

### screen readers 
* programs that read out the contents of a computer screen to a user; ie. people who are visually impared use this service

Web server hosting or 
### Dommain Name System
(DNS) can be hosted anywhere in the world.

ISP (Internet Service Provider)
DSN - acts like a telephone book; it tells your computer the IP address of that domain name. 

### Structure
The structure is very much like writing an essay. You have headers, fonts, paragraphs, spacing etc. 

### HTML
is what describes & defines the structure of these pages.

example: 

<html>
    <body>
        <h1>Here's my Main Heading Example</h1>
        <p>And here's my beginning paragraph about some interesting things going on and what not.</p>
        <h2>This is a little sub header I thought I should add</h2>
        <p>Here's another paragraph for added content.</p>
        <h3>And another sub heading to keep things interesting.</h3>
    </body>
</html>

<html></html> - the opening tag for any HTML code (both open and closing tags - note the / on the end code... it's what closes it for you)

<body></body> - this is what's shown in the main browser window. This is where you want to place your content. 

<h1></h1> - a header form (both open and closed) and also comes in other variations (header sizes)

There are also 
    - Attributes that tell us more about the elements. They appear on the opening tag of an ### element and are made up of 2 parts: a ### Name and a ### Value
* for example:

<p lang="en-us">This is telling us that our Paragraph is in English! Wowie!</p>
The ### lang in the above example is the 
### attribute name. - this indicates what kind of extra info is being supplied in the element's content. It should be written in 
### lowercase

 The "en-us" is our ### attribute value. - This is the information / setting for our attribute. It shoudl be placed in ### double quotes (" ") 

 There is also the 
 <title></title> tag that will appear at the very top of the ### title bar or ### tabs at the top of the browser window. 

To look into how others are building their websites, you can go to the page and look for the ### View menu in yoru browser. Then select the option that says ### Source or ### View Source (the location may vary depending on the browser being used.)

### Extra Make Up
    * Learning the different versions of HTML and how to indicate which version being used
    * How to add comment to your code
    * Global attributes - used on any element, including ### class and ### id attributes
    * Elements that are used to group together parts of the page (where no other element is suitable)
    * Embedding a page within a page using ### iframes
    * How to add info about the web page using the ### <meta> element
    * Adding characters such as angled brackets <> and copyright symbols 
       &copy; or &#169;
    
The evolution of HTML:
    HTML 4 ===> XHTML 1.0 ===> HTML 5 (work in progress)
    each new version was designed to be an improvement on the last

### Doctypes
    Because of so many different versions of HTML, we have ### doctypes to help us tell which version of HTML the page is using. 
    Here are some examples of different doctypes.

*   HTML5
    <!DOCTYPE html>    

*   HTML 4
    <!DOCTYPE html PUBLIC
    "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd">

*   Transitional XHTML 1.0
    <!DOCTYPE html PUBLIC    
    "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/DTD/xhtml1/xhtml1-transitional.dtd">

*   Strict XHTML 1.0
    <<!DOCTYPE html PUBLIC
    "-//W3C//DTD XHTML 1.0 Transitional//EN"
    "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">

*   XML Declaration
    <?xml version="1.0" ?> 
    note: Because XHTML was written in XML, you will sometimes see pages that use XHTM strict DOCTYPE start with an optional XML declaration. Where this is used, it should be the first thing in a document. There must be ### nothing before it. Not even a space.

<!-- -->
    * is used when you want to add a comment to your code, that will NOT be visible in the user's browser. 
    An example for that would look like the following (highlighted in gree):
    
<html>
    <!-- and this is where I'd like to leave and unseen comment to the user on the web page -->
    <body>
        <h1>Here's my Main Heading Example</h1>
        <!-- As you can see, I can do this here -->
        <p>And here's my beginning paragraph about some interesting things going on and what not.</p>
        <!-- and there -->
        <h2>This is a little sub header I thought I should add</h2>
        <p>Here's another paragraph for added content.</p>
        <!-- Just about anywhere! -->
        <h3>And another sub heading to keep things interesting.</h3>
    </body>
</html>

It's good to have comments for your code so if someone else needs to look at the code, it's much more user friendly and retainable. Anyone viewing the source code of the page will be able to see your notes. These comments can also help explain the code better. Comments can also be used around blocks of code to stop that code from being displayed.

*   ID Attribute
    - the id attribute is used to uniquely identify that element from other elements on the page. 
    - It's value should start with a ### letter
    or an ### underscore (not a number or any other character)

*   Class Attribute
    -this helps you identify different elements on the page. It can distinguish and emphasize different parts of your content.    
    
    Please see below for examples of both:
<html>
    <body>
        <p> Here's some content in this paragraph.</p>
        <p id="pullquote">Here's a paragraph containing a pullquote style! Cool beans, right?! </p>
        <p class="important admittance"> Just some more content for good measure. Apparently this is very important content! </p>
    </body>
</html>

*   Block elements -
    appear to start a new line and create a block like structure to your content. 
    Examples of block elements would be the following:
    <h1></h1>
    <p></p>
    <ul></ul>
    <li></li>

*   Inline elements -
    emphasize content ex.:
    <em> make this darker </em>
    <b> highlight me! </b>

*   <div> - an element that allows you to group a set of elements together in one block-level box. ex:
    

<div id="header">
    <img src="images/logo.gif" alt="Anish Kapoor" />
    <ul>
        <li><a href="index.html">Home</a></li>
        <li><a href="biography.html">Biography</a></li>
        <li><a href="works.html">Works</a></li>
        <li><a href="contact.html">Contact</a></li>
    </ul>    
</div><!-- and here's the end of the header/ example! ==>    

* <span> - the span element acts like an inline equivalent of the  <div> element. It's used for either: 
    1. to contain a section of text where there is no other suitable element to differentiate it from in the surrounding text. 
    2. to contain a number of inline elements. 
    But the most common reason people use <span> elements is so they cna control the appearance of the content of these elements using CSS. 
    <span>
ex. 
    <p>This is some important writing that may need to be emphasised somehow. <span class="gallery">So I might as well make it pretty!</span>
    </p>

* <iframes> - a little window that has been cut into your page, that allows you to see into another page. A great example of that would be google maps! It would look something like this:

    <iframe
        width="450"
        height="350"
        src="http://maps.google.co.uk/maps?q=moma+new+york&amp;output=embed">
    </iframe>    

*   src - this attribute specifies the URL of the page to show in the frame. 

*   height - this attribute specifies the height of the iframe in ### pixels.

*   width - this attribute specifies the width of the iframe in ### pixels.

Other bits of Iframes to consider: 
    scrolling
    frameborder
    seamless

*   <meta> - this element lives inside the <head> and contains information about that web page. It is an empty element so it does ### NOT have an ending tag.

*   description - contains a description of the page. This is commonly used by search engines to understand what the page is about andshould bbe a maximum of 155 characters. Some are also displayed in seach engine results (think SEO).

*   keywords - words that a user might search to find your page.

*   robots - this indicates whether search engines should add this page ot their search results or not. 

Other things to consider with the <meta> element:
    author - defines the author of the web page
    pragma - prevents the browser from caching the page
    expires - because browsers often cache the content of a page, the ### expires option can be used to indicate when the page should expire (and no longer be cached).

Here are some ### escape charaters that are good to know.

| Character | Code | Alturnative |
| ------ | ------ | ------- |
| < less than | &lt; | &#60; |
| > greater than | &gt; | &#62; |
| & ampersnd | &amp; | &#38; |
| " quotation mark | &quot; | &#34; |
| Cent sign | &cent; | &#162; |
| Pound sign | &pound; | &#163; |
| Yen sign | &yen; | &#165; |
| Euro sign | &euro; | &#8364; |
| Copyright symbol | &copy; | &#169; |
| Yen sign | &yen; | &#165; |
| Registered trademark | &reg; | &#174; |
| Trademark | &trade; | &#8482; |
| ' left single quote | &lsquo; | &#8216; |
| ' right single quote | &rsquo; | &#8217; |
| " left double quote | &ldquo; | &#8220; |
| " right double quote | &rdquo; | &#8221; |
| X multiplication sign | &times; | &#215; |
| Division sign | &divide; | &#247; |

### HTML Layouts 
    - the new HTML5 elements indicate the purpose of different parts of a web page and help describe its structure. 
    - new elements provide clearer code (compared to using mulipul <div> elements).
    - older browsers don't understand HTML5 elemnts, so they need to be told which elements are block-level elements. 
    - to make HTML5 work in older versions of IE (internet explorer), extra JavaScript is needed. 

*   traditional HTML layout - defined by <div> elements (such as the elements that form a header, article, footer or sidebar) ie.
    
<body>
    <div id="page">
        <div id="header">
    <div id="nav>    
</body>

*   new HTML5 layout - limit the <div> placement to create cleaner code/page structure. ie.

<body>
    <div id="page">
        <header>
        </header>
    <nav>   
</body>     

*   <header> </header> 
*   <footer> </footer> 
    - the main header or footer that appears at the top or bottom of every page on the site. You can also have a header or footer for an individual <article> or <section> within the page.

*   <nav> </nav>
    - the <nav> element is used to contain the major navigational blocks on the site, such as primary site navigation. ie. 

<nav>
    <ul>
        <li><a href="" class="current">home</a></li>
        <li><a href="" class="current">classes</a></li>
        <li><a href="" class="current">catering</a></li>
        <li><a href="" class="current">about</a></li>
        <li><a href="" class="current">contact</a></li>
    </ul>
</nav> 

*   <article> </article> - this element acts like a container for any section of a page that could stand alone, such as an individual article or blog entry, a comment or forum post, or any other independent piece of content. 

*   <aside> </aside> - the aside element has two purposes, depending on whether it's inside an <article> or not. 
When it is used ### inside of an <article> it should contain information that is related to the article but not essential. ie. a pullquote or glossary might be considered as an aside to the article it's realted to. 
When <aside> is ### outside an <article> it acts as a container for content that is related to the ### entire page. ie. links to other sections of the site, a search box, recent posts list, or recent tweets... etc. 

*   <sections> </sections> - groups related content together and typically each section would have its own heading. 

*   <hgroup> </hgroup> - this element groups together a set of one or more <h1> through <h6> elements so that they are treated as one single heading. ie.

<hgroup>
    <h2>Japanese Vegetarian</h2>
    <h3>Five week course in London</h3>
</hgroup>

*   figures <figure> </figure> <figcaption> </figcaption> - can be used to contain any content that is referenced from the main flow of an article (not just images). It should only be used when the content simly references the element (and not for something that's an integral to the flow of the page). ex. 
    - images
    - videos
    - graphs
    - diagrams
    - code samples
    - text that supports the main body of an article

<figure>
    <img src="images/bok-choi.jpg" alt="Bok Choi" />
    <figcaption>Bok Choi</figcaption>
</figure>

*   sectioning elements <div> - the <div> element remains an important way to group together related elements. 

*   <a> </a> linking around block-level elements - HTML5 allows you to place an <a> element around a block level element that contains child elements .This allows you to turn an entire block into a link. 

### Key elements to focus on when Designing your Website
    - who is the site for?
    - why do people visit your site? 
    - what are your visitors trying to achieve?
    - what information do your visitors need?
    - how often will people visit your website? 

### Tools to use along the way
    - site maps
    - wire frames
    - (creating a) message by design
    - visual hierarchy
    - grouping and similarity
    - design navigation

### ABC's of Programming

*   <html> = content layer .html files (where the content of the page lives)
*   {css} = present layer (background, borders, box dimensions, colors, fonts, etc. all things design) .css files
*   javascript() = behavior layer (where we can change how the page behaves, adding interactivity)

*   JavaScript - is written in plain text, just like HTML and CSS, so you do not need any new tools to write a script.
ex.

var today = new Date();
var hourNow = today.getHours();
var greeting =

if (hourNow > 18) {
    greeting = 'Good evening!';
} else if (hourNow > 12) {
    greeting = 'Good afternoon!';
} else if (hourNow > 0) {
    greeting = 'Good morning!';
} else {
    greeting = 'Welcome!';
}

document.write('<h3>' + greeting + '</h3>');

*   linking to a Javascript file from an HTML page

<link rel="stylesheet" href="css/c01.css" />
   
<script src="js/add-content.js"></script>
 <!-- this tells the HTML <script> element that is used to load the JavaScript file onto the page -->

*   Objects and Methods
ex.
    document.write('Good afternoon');

In this example, the 

    ### document object represents the entire web page. 

    ### . (the period) - is the member operator. You can access the members of an object using a dot between the object name and the member you want to access. 

    ### Method - in this example is the ### write() method of the ### document object allow new content to be written into the page where the <script> element sits.

    ### Parameters - the 'Good afternoon' in this example. Whenever a method requires some information in order to work, the data is given inside the parentheses (). Each piece of information is called a parameter of the method. In this case, the ### write() method needs to know what to write into the page. 

    I hope this document finds you well and helps further one's study of code!
    




    
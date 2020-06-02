Common HTML tags
There are many HTML tags to choose from depending on what elements you want to structure on your page. You can always look up HTML tags here. However, here is a short list of some of the most common HTML tags, ones you'll see us use throughout this course.

>>> HTML

The root element of a document is <html>, and this is the first tag you'll need in your document (after the DOCTYPE, of course!). All your other HTML tags should go inside this one, meaning all HTML documents should start with <html> at the top and end with </html> at the bottom.

You'll notice in the below code that we set the language to English (<html lang="en">) . You can set another language of the text in your page using language attributes (see also this resource).

It is important that you take care to use the lang attribute to indicate the actual language of text in your page because many CSS features will function differently, depending on what language is declared here.

    <!DOCTYPE html>
    <html lang="en">
       <body>
          <p> Hello World</p>
       </body>
    </html>

>>> HEAD

This is the element that contains all the metadata for your site, such as your link to your CSS, the page's title and links to other files. This should be the first tag in your document, and there should only be one per document.

Note that this is where you will also set the charset to "utf-8" (<meta charset="utf-8">). This shows that you saved the markup using the UTF-8 character encoding, which has many characters outside English, so it should be able to display characters not in the English alphabet.

    <!DOCTYPE html>
    <html lang="en">
        <head>
            <meta charset="utf-8">
            <title>My First Page</title>
        </head>
        <body>
            <p> Hello World</p>
        </body>
    </html>
    
>>> BODY

The section element that contains all the visible content for your site like your text, images, links etc. There should only be one body tag per document and it should come after the head tag.

    <!DOCTYPE html>
    <html lang="en">
        <head>
            <meta charset="utf-8">
            <title>My First Page</title>
            <link rel="stylesheet" href="styles.css">
        </head>
        <body>
            <p> Hello World</p>
        </body>
    </html>

>>> P

"p" stands for "paragraph" which is a block of text that is physically separated from adjacent blocks through blank lines. This is the most basic way to group text content.

    <p>
       This is my introductory paragraph to my Web page! This text will wrap around in a single block and then after the paragraph is done there will be a line of white space.
    </p>

Documentation
<a>

By surrounding text with an <a> tag you turn it into a hyperlink. You will want to use the "href" attribute to indicate to which target the link should take the user when clicked. The default style of the a tag is to turn the text blue and underlined, and then change the color to purple after you have clicked the link. You can adjust all these styles with CSS.

    <a href="https://www.microsoft.com">Microsoft Main Page</a>


>>> IMG

This tag will insert an image based on the source you provide via the "src" attribute. If the source is inaccessible, you can also specify "fall back" options via the "alt" attribute. You will always want to specify the "alt" attribute with a short phrase describing the image. This text is what will be read aloud if your user is using a screen reader, or will be displayed if the user's browser will not load images. Note that this is an example of a "self-closing" tag meaning there is no closing tag, you just end the opening tag with a forward slash. 

    <img src="images/proPic.jpg" alt="a headshot of the instructor" />

>>> UL

The UL tag creates an "unordered list" element, meaning a collection of elements in which the order is meaningless. This is a tag that sets the framework for you to add list elements inside it. You will want to add your elements within the ul tag each surrounded your content with list item or "<li>" tags like in the below example.

    <ul>
       <li>This is one element in the list</li>
       <li>One of the elements</li>
       <li>Another element</li>
    </ul>

>>> OL

The OL tag works exactly like the UL tag, except that the list element order matters. OL stands for "ordered list" and by default, the list element items are displayed with a number preceding them.

    <ol>
       <li>This is the first element</li>
       <li>The second element</li>
       <li>Finally, this is the third element</li>
    </ol>

>>> BR

The br element is a self-closing tag that inserts a line break. This is most evident when placed in a block of text as it essentially represents a carriage return or hitting the "enter" key. 

    <p>
       this is my text.
       <br />
       this text will appear on the next line down.
    </p>

>>> HEADER

The header tag is one of the section elements, it's role is to group other HTML elements according to their role on their page. The header element contains all the introductory content on the page typically a title and tagline or navigational elements. 

    <body>
       <header>
          <h1> Welcome to my page!</h1>
          <h2> My very first web page</h2>
       </header>
    </body>

>>> SECTION

Another sectioning element, the "section" tag is a general-purpose grouping element. It most often should include a header tag at the top. This typically will come after a header tag and before a footer tag.

    <body>
       <header>
          <h1> My Page </h1>
       </header>
       <section>
          <h2> My Blog </h2>
       </section>
    </body>

>>> FOOTER

Another sectioning element, the "footer" tag is supposed to organize the final content on the page such as the credits or contact info. 

    <body>
       <header>
          <h1>My Page</h1>
       </header>
       <section>
          <h2>My Blog</h2>
       </section>
       <footer>
          <p>
             copyright 2016
          </p>
       </footer>
    </body>

>>> DIV

The div element is a generic element to hold content. It is considered a last resort, for when no other element is suitable but is often used to collect together large portions of a site that contain multiple different types of content. 

        <div>
           <h1> Title for Content </h1>
           <img src="images/contentImage.jpg" />
           <p> This is a paragraph explaining this section of content associated with the above image and title </p>
        </div>


>>> Here is an example CSS "rule":

    p {
        color: blue;
    }

This rule tells the browser to make all text within a paragraph tag blue. A CSS rule is broken into two parts: the selector and the property css anatomy

>>> Selector

This is the portion of the rule before the first open curly brace ( "{" character). This is what tells the browser what HTML tags this rule applies to. Often, you'll just see a selector that matches an HTML tag, like in this instance- our selector is just "p". However, as we get further into this course, you'll find that there are many ways to target specific HTML elements and many different ways to structure selectors so that you are targeting exactly the part of your site you want to style.

>>> Property

This is the portion of the rule between the two curly braces. This is what tells the browser how to style the HTML tag that has been selected. This can be as many lines of code as you choose, each of which has two parts- the property and the value you want that property to be. For our example, "color" is the property and "blue" is the value, but we could also have had a value of "black" or "#FFFFFF" (which is HEX code for white). Each property line is constructed so:

property anatomy

The style for your page will consist of a list of many CSS rules put together. As we move through this course we will help you build up these rules to style your entire page.


>>> What is a selector?

CSS selector is the portion of the CSS rule that tells the browser on which HTML element to apply the defined style.

When your HTML is simple, the selectors can be simple as well. The most basic selectors simply mirror the HTML tag. For example "p" attaches to all <p> tags, "img" will attach to all <img> tags and so on. As you can imagine, there will often be times when you don't want every single HTML element of a particular type to have identical style. In Module 3, we'll discuss a variety of ways to use selectors to attach to specific HTML elements. 

When choosing your selector you might want to keep the following aspects of an HTML element in mind:

    How many of these HTML elements are on my page? Do I want this style to apply to every one of these elements?
    What are this HTML element's children, and do I want this style to apply to them as well?
    Is this element a block element or an inline element, and does this style make sense in that context?

It is possible to independently target every HTML element on the page using selectors, but for this module we are going to stick to basics and only use selectors that match the HTML tag name. For example, here are some example selectors we'll use in this module:

    a {
     /* style for a tags */
    }

This would affect the style of all link tags on the page.

    p {
     /* style for p tags */
    }

This would affect the style of all paragraph tags on the page and the style of elements contained within the paragraph tag. 

    body {
     /* style for all elements in the body */
    }

This would apply style to the body tag as well as allow the elements inside the body tag to inherit certain styles applied here. 

Here is a Code Pen that demonstrates how styles apply to different selectors.

>>> HTML code:

    <!DOCTYPE html>
    <html lang="en">
        <head>
            <meta charset="utf-8">
            <title>My HTML page</title>
            <link rel="stylesheet" href="style.css">
        </head>
        <body>
            <h1>Title</h1>
            <p>In unit 2.3, we defined a CSS selector as the portion of the CSS rule that tells the browser on which HTML element to apply the defined style.
                <a href="http://www.microsoft.com">Click Here!</a>
            </p>
            <ul>
                <li>When your HTML is simple, the selectors can be simple as well</li>
                <li>he most basic selectors simply mirror the HTML tag</li>
                <li>For example "p" attaches to all tags, "img" will attach to all tags and so on</li>
                <li>As you can imagine, there will often be times</li>
                <li>when you don't want every single HTML element of a particular type to have identical style</li>
            </ul>
            <p>           
    In Module 3, we'll discuss a variety of ways to use selectors to attach to specific HTML elements. 
    In unit 2.2, we briefly mentioned the fact that properties apply to the entire hierarchy of HTML elements to which they are attached. This means that you will have to be very careful which selectors you choose to use in combination with your chosen style 
     <br />
    <a href="http://www.w3.org">Check this out</a>
    It is possible to independently target every HTML element on the page using selectors, but for this module we are going to stick to basics and only use selectors that match the HTML tag name. For example, here are some example selectors we'll use in this module:
            </p>
            <ol>
                <li>This would affect the style of all link tags on the page</li>
                <li>This would affect the style of all paragraph tags on the page</li>
                <li>and the style of elements contained within the paragraph tag</li>
                <li>This would apply style to the body tag</li>
                <li>as well as allow the elements inside the body tag to inherit certain styles applied here. </li>
            </ol>
        </body>
    </html>
>>> CSS code:

    body {
        color: red; /* every element inherits this except those with more specific style */
    }
    ul {
        color: blue;/* li elements inherit this color */
    }
    p {
        font-style: italic; /* this even the a tags inherit within the paragraphs */
    }
    li {
        text-decoration: line-through; /* applies to all li elements, in both ul and ol tags */
    }


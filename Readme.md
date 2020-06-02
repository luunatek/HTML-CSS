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


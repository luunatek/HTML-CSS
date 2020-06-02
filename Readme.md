Common HTML tags
There are many HTML tags to choose from depending on what elements you want to structure on your page. You can always look up HTML tags here. However, here is a short list of some of the most common HTML tags, ones you'll see us use throughout this course.
<html>

The root element of a document is <html>, and this is the first tag you'll need in your document (after the DOCTYPE, of course!). All your other HTML tags should go inside this one, meaning all HTML documents should start with <html> at the top and end with </html> at the bottom.

You'll notice in the below code that we set the language to English (<html lang="en">) . You can set another language of the text in your page using language attributes (see also this resource).

It is important that you take care to use the lang attribute to indicate the actual language of text in your page because many CSS features will function differently, depending on what language is declared here.

    <!DOCTYPE html>
    <html lang="en">
       <body>
          <p> Hello World</p>
       </body>
    </html>

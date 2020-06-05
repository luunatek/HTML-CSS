>>> Spacing properties

CSS provides a great set of tools to help you position the HTML elements on your page, and we will cover that in depth in Module 4. For now we will talk about how to apply white space around individual HTML elements.

There are two different ways you can define white space:

        in absolute terms: using an exact number of pixels,
        and in relative terms: using percentages or ems.

For now, we'll use pixels because that is easier to learn. However, ultimately you will want to use percentages and ems so your content adapts to different screens. We will discuss how to use percentages in Module 4. 

When you view an element in your browser tools you can see the white space around it represented like so:

>>> Margin padding border

The above image is called the "box model", which we will get into more detail about in Module 4. For now, you can see that the space around the content is broken into three distinct regions. 
Padding

    p {
       padding: 20px;
    }

"Padding" is the white space that sits closest to an HTML element. Many elements already have a default padding defined. For example, ul elements by default are indented to the left a bit because they have a left padding.

You can set the padding on an element's four sides independently using padding-top, padding-right, padding-bottom and padding-left. Or you can use the more compact padding: 10px 15px 20px 25px. In this case, the order of the numbers sets the top, right, bottom and left paddings. In the above example, I collapsed all of these and just set the padding on all four sides to be 20px. Here is a code pen that demonstrates all these different ways to set padding.

>>> Border

    p {
       border: 1px black solid;
    }

The "border" is the area outside the padding of an HTML element. By default, borders are set to be empty, but you can set their width, color, pattern, even an image! Like padding, you can even adjust the four sides of a border independent of one another using border-top, border-right, border-bottom or border-left. You can also adjust the different aspects of a border with border-width, border-color, and border-style. In the above example, I collapsed all of these properties into a single simple property and value set. 

>>> Margin

    p {
       margin-bottom: 50px;
    }

An HTML element's "margin" is the white space that sits outside the border. Margins of HTML elements interact with other another on the page to determine how they are arranged on the page. A lot of elements have default margins applied.

For example, the body tag typically has a margin that causes any content to not extend all the way to the extreme edge of the page. Be careful, margins can be tricky. When two margins touch they "collapse" such that the space between the elements is equivalent to the larger of the two margins. Like the above properties, you can also set the margins on each side independently using margin-top, margin-left, margin-bottom and margin-right. 

>>> Example:
>>> HTML code:

    <!DOCTYPE html>
    <html lang="en">
        <head>
            <meta charset="utf-8">
            <title>My HTML page</title>
            <link rel="stylesheet" href="style.css">
        </head>
        <body>
            <h1>Main Title</h1>
            <ul>
                <li> List element 1</li>
                <li> List element 2</li>
                <li> List element 3</li>
            </ul>
            <p>
                Integer euismod at lectus vel placerat. Nam laoreet a quam in maximus. Duis turpis tellus, accumsan ac efficitur in, tempus vel augue. Aenean vitae venenatis tortor. Praesent dignissim nisl id odio fringilla, ac dapibus enim euismod. Sed id tellus vel est blandit finibus non vel magna. Nullam mattis, odio in suscipit dapibus, mauris dolor mollis nisl, et ultricies sem justo ac dui. Etiam ut turpis ipsum. Vivamus sodales vel nibh ut gravida. Pellentesque eu nunc elementum, sodales diam dictum, lobortis magna. Suspendisse id mattis ipsum. Vivamus scelerisque facilisis justo, id facilisis dui auctor sed.
           </p>
        </body>
    </html>

>>> CSS code:

    body {
        background-color: #99ffff;
        margin-top: 20px;
        margin-left: 70px;
    }
    h1 {
        background-color: #ff6699;
        border-bottom: 20px #ff0066 solid;
        margin-bottom: 10px;
        padding: 5px;
    }
    ul {
        background-color: #ff9933;
        border-left: 5px black dashed;
        margin: 50px;
    }
    li {
        background-color: #ffcc66;
        margin: 10px;
        padding: 10px;
    }
    p {
        background-color: #ccff99;
        border: 10px white double;
        padding: 0px;
        margin: 0px;
    }


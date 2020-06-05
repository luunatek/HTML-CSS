>>> Titles

There are a couple different categories of text on a Web page: titles, body text, links, captions, etc.

You'll want to style each of these differently to help your user understand the proper context for your text. One of the most important categories of text to stand out are your titles. 

There are different aspects of text you can alter to make it stand out. 

    size 
    font
    capitalization
    color
    emphasis
    weight

However, you should only alter a few of these following aspects at a time to prevent your titles from being too distracting. The below is an example of using too many different aspects of font for emphasis:

Image of too busy title

    #busyTitle h1{
        font-size: 2em;
        font-family: Impact
        color: yellow;
        background-color: gray;
        font-style: italic;
        font-variant: small-caps;
        font-weight: bold;
        text-decoration: underline;
    }

>>> Title 1

This title uses soft clean colors based on print media, so we chose a serif font. We also increased the size and color to help the title appear more prominent than the body text. 

>>> title 1

    #design1 {
        background-color: #F4F4F4;
        font-family: "Lucidia Sans Unicode", sans-serif;
    }
     
    #design1 h1 {
        color: #C0B283;
        font-size: 4em;
        font-weight: 700;
        font-family: Garamond;
        width: 300px;
    }
     
    #design1 p {
        color: #373737;
        font-size: 1.2em;
    }

>>> Title 2

This design is intended to look futuristic, so it only uses sans-serif, thin font with high contrast colors.

>>> title 2

    #design2 {
        font-family: Century Gothic, sans-serif;
        background-color: #0E0B16;
    }
     
    #design2 h1 {
        font-weight: 400;
        font-size: 2.3em;
        color: #A239CA;
        font-style: italic;
    }
     
    #design2 p {
        color: #E7DFDD;
    }

>>> Title 3

This design is based on pastel primary colors and uses color as a highlight against the default white background. We have achieved the separation between title and body text by setting its background color separately and giving it a bottom border. 

>>> title 3

    #design3 {
        color: #DF744A;
        font-family: Arial, sans-serif;
    }
     
    #design3 h1 {
        background-color: #BFD8D2;
        text-align: center;
        font-size: 4em;
        font-weight: 100;
        padding: 30px;
        border-bottom: 5px #DCB239 solid;
        font-family: Helvetica, sans-serif;
    }
     
    #design3 p {
        background-color: #FEDCD2;
        padding: 50px;
    }


>>> Buttons

Buttons are a key way that your users will interact with your page. Often buttons are a call to action for your user- so you will want them to stand out!

When styling a button you aren't just styling the text, but also the area around it, including the border. By giving them a distinct background color or border you make it clear that this whole area is "clickable".

Typically your user will expect your button to be wider than it is tall, to accomplish this you'll want to set the left and right padding to be greater than the top and bottom paddings. 

Here is an example of a button where it's not immediately clear that it is actually a button. 
>>> Button 1

This design is a pretty traditional button where it has a distinct background-color and border-color to help it stand out from both the background and the body text.

button design 1 image

    #design1 {
        background-color: #94618E;
        color: #F8EEE7;
        font-family: Corbel;
    }
    #design1 button {
        background-color: #F4DECB;
        padding: 10px 25px;
        border: 5px solid #F8EEE7;
        color: #49274A;
        font-weight: bold;
        font-size: 1.2em;
     }

>>> Button 2

This is a more modern button design where there is no distinct border, but just a flat color background.

button design 2 image

    #design2 {
        background-color: #D9D9D9;
        color: white;
        font-family: "Century Gothic", sans-serif;
    }
    #design2 button {
        background-color: #4484CE;
        border: 0px;
        color: white;
        padding: 10px 50px;
        font-family: Impact, sans-serif;
        font-size: 1.3em;
    }

>>> Button 3

This is a big graphic button that uses border-radius to give the button rounded corners.

button 3 design image

    #design3 {
        font-family: Impact, sans-serif;
        font-size: 2em;
    }
     
    #design3 button {
        font-family: Impact, sans-serif;
        font-weight: 100;
        background-color: white;
        border: 7px #EC576B solid;
        border-radius: 20px;
        font-size: 0.8em;
    }

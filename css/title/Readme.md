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

Title 1

This title uses soft clean colors based on print media, so we chose a serif font. We also increased the size and color to help the title appear more prominent than the body text. 

title 1

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

Title 2

This design is intended to look futuristic, so it only uses sans-serif, thin font with high contrast colors.

title 2

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

Title 3

This design is based on pastel primary colors and uses color as a highlight against the default white background. We have achieved the separation between title and body text by setting its background color separately and giving it a bottom border. 

title 3

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

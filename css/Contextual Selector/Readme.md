When you use two selectors separated by a space on a rule, you scope the rule to the elements that correspond to the selector on the right that are INSIDE the elements that correspond to the selector on the left. Let's say we have the following HTML:

    <!DOCTYPE html>
    <html lang="en">
        <head>
            <meta charset="utf-8">
        </head>
        <body>
            <img src="images/pic1.jpg" alt="pic 1" />
            <p>
                This is my paragraph full of useful information
                <img src="images/pic2.jpg" alt="pic 2" />
                Since there is text around these images they should be styled a little differently.
                <img src="images/pic3.jpg" alt="pic 3" />
            </p>
            <img src="images/pic4.jpg" alt="pic 4" />
        </body>
    </html>

If we applied the following CSS rule then the images INSIDE the paragraph would be set to a width of 100px, but that rule would not apply to the images outside the paragraph. 

    p img {
        width: 100px;
    }

As your Web pages get more complex, contextual selectors become more important, because it won't scale to apply classes and IDs to each individual item. Contextual selection becomes especially useful when you structure your HTML with section tags like header, section, article and footer. 


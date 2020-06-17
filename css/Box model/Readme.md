The Box Model

The Box Model is how Web browsers see individual HTML elements. Each element is comprised of 4 areas: the element, the padding,
the border and the margin.


- element - This is always contained within a square, even if it is a text block with jagged edges or a transparent image that 
isn't rectangular. Web browsers will impose a rectangle around the smallest area the HTML element's content actually occupies.
Until now we've allowed the Web browser to determine the size of the element based solely on the content, but later in this 
section we'll learn how to adjust this sizing.
- padding - This is the white space just outside the element's content. You can set each of the four sides independently, and 
you can set the value to 0. If you set the element's background color, that color will apply to the padding as well.
- border - This is the area just outside the padding. Most HTML element's border default width is 0 and thus invisible. You can
set each of the four sides independently. You can set a color, a pattern, even an image. This is a great way to add horizontal 
or vertical lines to an element on your page.
- margin - This is the space surrounding an element, outside the border. Margins are the part of HTML elements that interact 
with one another. When two margins interact the larger of the two wins meaning the smaller margin "collapses", thus the actual 
space between two elements is the larger of the two, not the sum of the margins.

>>> width and height

    p {
       width: 30%;
    }

You can use pixel values for both width and height, but you'll most often want to use percentages to set these so that your elements grow and shrink as appropriate based on the screen size.

For example, if we set the width of a paragraph to 30% as you resize the browser window, you'll see how that element dynamically resizes. That's because when you use percentages, the size is computed based on the element's "containing block", or the element that contains the one you're styling. If your element is just within the body tag, the width is computed based on the relationship with the screen width.

Things are a bit more complicated with using a percentage to set an element's height. This is because typically the body's height is not specified, so if you use a percentage the size won't adjust.
min-width, max-width, min-height, max-height

Setting width and height with percentages will save you work because your design will automatically optimize for the user's screen size. However, some elements can't grow and shrink as dynamically as text can.

For example, images will get "pixelated" if you let them grow too large, and they can look really distorted. Thankfully, you can set max and min width and heights. This way, you can set a range for your image to grow and shrink where you know it will still look good. 

>>> Padding and margin
Whenever possible, it is ideal to position your elements by adjusting their padding and margins. Sometimes this isn't enough to get the element exactly where you'd like it to be, so we'll learn more tools later in this module. Regardless, you'll almost always want some padding and margin around your element so it's best to adjust these before progressing onto more complicated positioning methods.

Once you have set the width for your element, then you can set margins as a way to position your element relative to others. One of the most commonly used margin settings is "auto". That is because if you set an element's left and right margin to auto it will be dynamically centered within its containing block.

    div {
       width: 50%;
       margin-left: auto;
       margin-right: auto;
    }

However, note that this only works for block HTML elements like paragraphs, divs and headers. If you want to use this to position an inline element, such as img or a, you will need to tell CSS to treat them as block elements by setting display: block;

    img {
       display: block;
       width: 200px;
       margin-left: auto;
       margin-right: auto;
    }


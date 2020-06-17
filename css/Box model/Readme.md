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

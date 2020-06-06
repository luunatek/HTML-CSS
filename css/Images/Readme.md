>>> Images

Images are an extremely important part of your page, not only as part of your content but as a key way to help style your page. Before you even get to styling them you need to put considerable thought into what type of images to include in your page. One of the easiest ways to slow down your site's performance is to include lots of large, high-quality images. There are two general things to consider when picking your images: what format and how large are they? 
Formats

    JPEG - Possibly the most common image format used on the web, because it does a good job of compressing colorful, complex images into reasonably sized files. JPEG is often used for photos because otherwise, photos can take a very long time to load. 
    PNG - Provides a higher quality image, but you pay for it with a larger file size. PNG also has the ability to have transparent backgrounds, so you'll often see this used for graphics as part of the page's layout. 
    GIF - Supports moving images and transparent backgrounds. These can be especially large files so try to use sparingly!

>>> Sizing

It's important to format and size your image before uploading it to your site, because while you can use CSS to resize it, the browser will download the full image even if you've chosen to display it smaller than it is. 

You can resize images using the width or height properties of CSS like so:

    img {
        width: 100px;
        height: 100px;
    }


Rarely does it look nice when your content images touch your text content. You'll often want to give your images a good amount of white space surrounding them, and you can do this with padding and/or margin. In the examples below, you can see how you can even use padding and margin to achieve some interesting stylistic effects with your images. 
Border Radius


When you see complicated styles as part of a Web page's design, chances are there are images as a foundational element. For example, you will often see images set as backgrounds or as a link. Remember that you can put an <img> tag within an anchor tag to turn it into a link. You can also use the background-image CSS property to set an image as a background instead of just using a solid color. You can read more about background images here. 
Text in images

It is best to overlay real text rather than use pixelated text. This makes it possible to search, copy and style the text, as well as making translation much easier. It also has accessibility benefits and makes translation much easier.

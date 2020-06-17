https://www.w3.org/TR/CSS22/visuren.html#propdef-clear

If your elements are still not exactly where you want them to be after adjusting the padding, margins and alignment, then you 
can try out the float property. The "float" property is one of the most powerful tools you can master when learning CSS.


    h1 {
       width: 20em;
       float: right;
    }

Up until now, we haven't moved elements very far from wherever the web browser automatically places them, but as you've 
probably noticed this has left our page very left side heavy. This is because, by default, elements are stacked one on top of 
the other, and they don't share horizontal space. With the float property, we can change this.

The float property liberates an element from its automatic position and lifts it up to "float" on top of other elements in the 
direction you specify.  You can specify float either right, left or the default of none. 

Elements underneath a floating object will automatically wrap themselves around the content. For example, if you float an image,
the text underneath will wrap around it so that none of it is actually obscured underneath the image, but now both text and an 
image can share horizontal space. 

You'll often want to set the width of a floating object so that you have tighter control over the space that object occupies. Remember that, by default, block HTML elements occupy the entire width of the page, even if there isn't actual content that extends that far. In this case, you'll want to set the width so that your element's size more accurately represents its content and you don't have unnecessary white space. 
The clear property

Once you have some elements floating things can get a little messy. Its easy for floating objects to overlap, and to prevent 
this you can use the "clear" property.

Documentation

    p {
       clear: both;
    }

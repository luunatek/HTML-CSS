>>> Pseudo-classes are a way to select HTML elements based on their state as opposed to their HTML structure. You can read more about pseudo-classes here.

Pseudo-classes must always be applied to an existing selector. Their "flag character" is the colon (":"), as you can see used in the below examples. Here are some of the most popular pseudo-classes.
:link and :visited

    a:visited {
       color: gray;
       font-style: italic;
    }

These pseudo classes are the ones you are probably most familiar with. Even on this page you've probably noticed that links have different style than paragraph text. The <a> tag by default sets the text color to blue with an underline, but have you ever seen a purple link? This is the "visited" pseudo-class that applies a different style to links that the user has already clicked. The opposite of visited is "link" which is a link a user has not yet clicked. These two states are mutually exclusive, meaning a link cannot be both at the same time.

Documentation
:hover

    li:hover {
       background-color: yellow;
    }

The hover pseudo-class is applied when the user points at an object but doesn't activate it, most commonly when they let their mouse cursor lay on top of an element without clicking. Some form factors don't support this, such as touch devices or pen surfaces. This is a really good way to encourage a user to click a link and you will often see it used in navigation bars. 
:focus

    input:focus {
       background-color: blue;
    }

The focus pseudo class is when a user has chosen to begin interacting with an element, often when the click into a form input such that the input is then ready to accept keyboard input.
:active

    p:active {
       color: red;
    }

The active pseudo-class applies when an element is activated. This happens in the time between when the user clicks their mouse and they release it.

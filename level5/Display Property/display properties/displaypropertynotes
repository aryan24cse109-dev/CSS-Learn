<!--Display Property :
   1) Block Element:
   a) New line : Starts on a new line
   b) Width : Takes up the full width available
   c)Styling : Can be styled with width, height, margin, padding, etc.
   d) Examples : <div>, <p>, <h1> to <h6>, <form>, <header>, <footer>,<ul> , <li>  etc.
   
   2) Inline Element:
   a) New line : Does not start on a new line
    b) Width : Takes up only as much width as necessary
   c) Styling : Cannot be styled with width, height, margin, padding, etc.
   d)NO Break : Cannot strat a new line and cannot have line breaks
   e) Examples : <span>, <a>, <strong>, <em>, <b>, <i>, <img> etc.

    3) Inline-Block Element:
   In inline block elements, the element itself is formatted as an inline element, but you can apply height and width values. It allows you to set a width,height , margin and padding on the element, but it will still flow inline with other elements.For it to be inline-block, the element must be set to display: inline-block; in CSS.
   Examples : <button>, <input>, <select>, <textarea> etc.

    4) None Element:
    a) New line : Does not start on a new line
   b) Width : Takes up only as much width as necessary
   c) Height : Takes up only as much height as necessary
   d) Styling : Cannot be styled with width, height, margin, padding, etc.
    
   QUES) What is the difference between none elements and visibility hidden elements and why we need none elements?
   Ans) The difference between none elements and visibility hidden elements is that none elements are not visible but they still take up space in the layout, while visibility hidden elements are not visible and do not take up any space in the layout. We need none elements when we want to hide an element completely from the page, without affecting the layout of other elements.

   In summary, the display property in CSS is used to control the layout and visibility of elements on a web page. It allows us to specify whether an element should be displayed as a block, inline, inline-block, or none, and each value has its own unique characteristics and use cases.
   
   If we does not use display property then by default all the elements are block elements and they will take up the full width available and start on a new line. This can cause layout issues and make it difficult to control the positioning of elements on the page. By using the display property, we can change the default behavior of elements and create more flexible and responsive layouts.

   If elements are inline elements but the display porperties is inline block , block and none then the elements will be displayed as inline elements, but they will still take up space in the layout and can be styled with width, height, margin, padding, etc. This allows us to create more complex layouts and control the positioning of elements on the page.

   Ques) What is box Sizing ?
   Every HTML element is rendered as a rectangular box made up of four layers (from inside out):
content → padding → border → margin
box-sizing is a CSS property that controls how the width and height you specify are calculated — specifically, whether padding and border are included inside that width/height, or added on top of it. Margin is never included in either case.

Ques) Types of box SIzing ?
1) Content-Box :
width/height apply only to the content area.
Padding and border are added on top, increasing the total rendered size.
Formula:
Total width  = width + padding-left + padding-right + border-left + border-right
Total height = height + padding-top + padding-bottom + border-top + border-bottom
Example:
csswidth: 100px;
padding: 10px;
border: 5px solid black;
Total rendered width = 100 + 10+10 + 5+5 = 130px
Use case: Rarely chosen deliberately today — mostly kept for legacy compatibility. Useful only when you specifically want content size to stay fixed regardless of padding/border changes.

2) Border-Box:
width/height include content + padding + border.
The content area shrinks to accommodate padding/border, but the total box size stays exactly what you set.
Formula:
Total width  = width you set (padding & border eat into content space)
Total height = height you set
Example:
csswidth: 100px;
padding: 10px;
border: 5px solid black;
Total rendered width = 100px (content area becomes 100 − 20 − 10 = 70px)
Use case: This is what almost all modern developers/frameworks use, because it makes layouts predictable — you set a width, that's the width, no mental math needed. 

3)Padding-Box:
Was proposed to include only padding (not border) in width/height.
Never got proper browser support and is now deprecated/removed from the spec. Not usable in practice.

Ques) Which type of elements use Which default border size ?
1) Content-Box: div, span, p, h1–h6, ul, li, img, most elements
2) Border-box: button,input, select , textarea ,progress and meter .


    -->
    
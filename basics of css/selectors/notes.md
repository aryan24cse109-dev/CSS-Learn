<!-------------------------Notes of Basics------------------------------------------------->

1)Class Selector :
 In Class Selector we select the element by its class and apply styles to it for define class in style , we use . symbol.
 In this file , we will use class selector on two pragraph define in two different type of p and div but there class is same . 
 Here instead of type of elements like h1 for heading and p for paragraph , we can also use div tags 

2) Id Selector:
In Id Selector we select the element by its id and apply styles to it for define id in style , we use # symbol.
Here we can also use div or span tags .

3)Group Selector:
 In Group Selector we select multiple elements and apply styles to them.
 In this file , we will use group selector on one heading deine in h type and two pragraph define in two different type of p and div but there class is same . 
 
4)Element Selector:
In Element Slector we select the element we have to apply style and changes just like here we have selected h1 and p element and applied color to them .
5)Descendent Selector:
In Descendent Selector we select the element by its id and apply styles to it for define id in style , we use # symbol. Here you can see in First div we define id as firstParagraph and in that we have p tag and we apply color to it. In Second div we define id as first-Pragraph and in that we have p tag and we apply color to it but you also se a another p a tag which is not in any div so id is not applied to it and it will be in deafult color and if you see style of any id on that p tag you should include p tag in any of div 

A few details worth knowing:
Technically, HTML5 allows almost any character in an id except whitespace — so spaces are the one thing you really can't use. Anything that looks like a space (literal space, tab, newline) breaks the id into multiple tokens.
The hyphenated style (first-paragraph) is called kebab-case, and it's the most common convention for ids and classes in CSS. You'll also see camelCase (firstParagraph) used sometimes, especially if the id is also being referenced in JavaScript, since getElementById("firstParagraph") reads a bit more naturally to JS developers than working with hyphens (which aren't valid in JS variable names anyway).

So your options are:
id="first-paragraph" then target it as #first-paragraph in CSS
id="firstParagraph" then target it as #firstParagraph in CSS

Both work fine — just pick one convention and stay consistent across your project so you don't trip over this again.

6)Universal Selector:
In Universal Selector, we select all elements on the page and apply styles to them and for universal selector we use asterisk (*) .
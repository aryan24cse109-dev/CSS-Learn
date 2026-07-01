<!-------Notes-->
-------------Float Property Notes-----------------
Eliment Alignment: The float property in CSS is used to position an element to the left or right of its container, allowing other content to flow around it. It is commonly used for creating layouts, such as wrapping text around images or creating multi-column designs.
2) Values: The float property can take the following values:
   - left: Positions the element to the left of its container.
    - right: Positions the element to the right of its container.
    - none: The element will not float and will remain in its normal position within the document flow.
    3) Clearing Floats: When using the float property, it is important to clear the floated elements to prevent layout issues. The clear property can be used on subsequent elements to ensure they do not wrap around the floated element. Common values for the clear property are:
     - left: Clears the left side of the floated element.
     - right: Clears the right side of the floated element.
     - both: Clears both sides of the floated element.
     4)Old Layout Technique: The float property was widely used in the past for creating layouts, but it has some limitations and can lead to complex and fragile designs. Modern CSS layout techniques, such as Flexbox and CSS Grid, provide more robust and flexible solutions for creating responsive layouts.
     5)Real life example: A common use case for the float property is to create a two-column layout, where an image is floated to the left and text wraps around it. This allows for a visually appealing arrangement of content on a webpage.
# Responsive Web Design
Reading 01

* how to build websites suitable for all users? The response to this question has become responsive web design, also known as **RWD**.
### Responsive Overview
Responsive web design is the practice of building a website suitable to work on every device and every screen size, no matter how large or small, mobile or desktop.<br>
* RWD is largely developed, by ***Ethan Marcotte***
### Responsive vs. Adaptive vs. Mobile the difference between all of them.
1. Responsive generally means to react quickly and positively to any change.
2. Adaptive means to be easily modified for a new purpose or situation, such as change.
3. Mobile generally means to build a separate website commonly on a new domain solely for mobile users.<br>

Currently the most popular technique lies within responsive web design.<br>
### RWD Has three components :
1. Flexible layouts : is the practice of building the layout of a website with a flexible grid, capable of dynamically resizing to any width using percentages or *em* units.

2. Media queries : provide the ability to specify different styles for individual browser and device circumstances, the width of the viewport or device orientation for example.
3. Flexible media : important aspect to responsive web design involves flexible media.<br>

* Relative Viewport Lengths<br>
1. vw<br>
Viewports width
2. vh<br>
Viewports height
3. vmin<br>
Minimum of the viewport’s height and width
4. vmax<br>
Maximum of the viewport’s height and width<br>

Fortunately, Ethan pointed out an easy formula to help identify the proportions of a flexible layout using relative values.<br>

The formula is based around taking the target width of an element and dividing it by the width of it’s parent element. The result is the relative width of the target element.


`target ÷ context = result`<br>

The flexible layout approach alone isn’t enough. At times the width of a browser viewport may be so small that even scaling the the layout proportionally will create columns that are too small to effectively display content. Specifically, when the layout gets too small, or too large, text may become illegible and the layout may begin to break. In this event, media queries can be used to help build a better experience.<br>

Initializing Media Queries<br>
Generally speaking it is recommend to use the @media rule inside of an existing style sheet to avoid any additional HTTP requests.<br>
/* @media Rule */
`@media all and (max-width: 1024px) {...}`<br>
* Logical Operators in Media Queries<br>
`and`, `not`, and `only`.<br>



# Float:
Float is a CSS positioning property.Floated elements remain a part of the flow of the web page. This is distinctly different than page elements that use absolute positioning. Absolutely positioned page elements are removed from the flow of the webpage.Absolutely positioned page elements will not affect the position of other elements and other elements will not affect them, whether they touch each other or not.<br>

### What are floats used for?
Floats can be used to create entire web layouts and they are also helpful for layout in smaller instances.

### Clearing the Float
An element that has the clear property set on it will not move up adjacent to the float like the float desires, but will move itself down past the float.<br>
* Clear has four valid values as well:
1. **Both** is most commonly used, which clears floats coming from either direction.
2. and  3.  Left and Right can be used to only clear the float from one direction respectively 
4. None is the default, which is typically unnecessary unless removing a clear value from a cascade

### Problems with Floats
Floats often get beat on for being fragile.The majority of this fragility comes from IE 6 and the slew of float-related bugs it has.

# THe END




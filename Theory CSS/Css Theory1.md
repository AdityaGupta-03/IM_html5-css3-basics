## CSS 3

-   Introduction
-   How to add CSS
-   selectors
-   comments
-   colors
-   backgrounds
-   Fonts
-   Opacity
-   Units
-   Text
-   borders
-   Margins
-   Paddings
-   Height and Width
-   Outline
-   Icons
-   Links
-   Lists
-   Tables
-   Display
-   max-Width
-   position
-   overflow
-   Specificity
-   Box Model
-   variables
-   media queries

Older versions - CSS1, CSS2, CSS2.1

CSS - Cascading StyleSheet

    - Help me to make website look better
    - Fonts, colors, borders etc...

1. Inline
2. Internal
3. External
4. Import

## New features

1. New Selectors - Better selection of HTML Elements
2. Shadow Effects - Box shadow, text shadow
3. Rounded Corners - Round the corners of images and block elements
4. Gradients
5. Opacity
6. Transitions
   7.Tranformations
7. Animations
8. Flexbox
9. Multi column layout - Build one dimensional layout
10. grids - Builds 2d

CSS3 - is supported in HTML5 based browsers - IE8 and lesser versions doesn't support css3 - IE9 supports CSS3 but not fully - IE10, Edge, chrome, firefox, safari 5.1 supports CSS3

## CSS 3 - Vendor Specific prefixes

e.g. background-color : yellow

    -webkit-background-color: yellow

1. -webkit- : Chrome, firefox, safari
2. -moz- : old firefox browser
3. -ms- : For IF9 and above
4. -o- : Opera 11 and above

## How to Add CSS

---

1. Inline
2. Internal
3. External
4. Import

## Selectors

---

1. simple selectors - selects elements based on name, id and class
2. combinator selectors - selects elements based on specific relationship between them
3. pseduo class selectors - Selects elements based on certain state
4. pseduo element selectors - set the styles to elements
5. Attribute selector - select elements based on attribute or attribute value

## Advantages of CSS

1. Saves time
2. Pages load faster
3. Easy maintain
4. Superior style to HTML
5. Multiple device compatibility
6. Global webstandards

## Selectors

1. Combinator selector

- 4 different combinators

    1. Descendant Selector (space)
    2. child selecctor ( > )
    3. Adjacent sibling selector (+)
    4. general sibling selector (~)

## Descendant Selector (space)

Matches all elements that are desecandants of a specified element.

Father - daughter
Great Grand father - Grand Father - Father - Son

## Child Selector ( >)

Matches all elements that are children of specified element

## Adjacent Sibling Selector (+)

The Adjacent sibling selector selects all the elements that are
adjacent siblings of specified elelemnt

Sibling - Must have the same parent element

adjacent - Immediately following

With adjacent sibling combinator only one element will be styled

## General Sibling selector (~) tilde

The general sibling selector selects all elements that are
siblings of a specified element

With the general sibling combinator one or more elelemnts will be styled

pseduo class selectors

---

Matches components based on an additional condition

allows you to style the dynamic state of en element

for e.g Hover, active and foucs

selector:pseduo-class {
porperty: value
}

Pseduo Element Selectors

---

Pseduo element sector is used to style specified parts of an element

for e.g

1.  Style the first letter or line of an element
2.  Insert the content before or after the content of an element

Selector::pseduo-element {
property: value
}

Note: ::first-line pseudo element can only be applied to block-level elements

---

In CSS2 and CSS1 pseduo class and pseduo elements used to have single colon,
In CSS3 this has changed and double colon is used for pseduo elements

## ::before

It can be used to insert some content before the content of our element

## ::after

It can be used to insert some content after the content of our element

## content

Content is a property in CSS which is used to generate the content dynamically.
It can generate content before and after pseduo element

## ::selection

It matched the portion of en element selected by the user

color, background-color, cursor and outline can be applied to selection

## Attribute selector

if attribute is target then, it selects all elements with target attribute

a[target] {
background-color: yellow - Selects all a elements with target attribute
}

## [attribute="value"] selector

Is used to select elements with a specified attribute and value

## [attribute ~ ="value"] selector

Is used to select elements with an attribute value containing a specific word

## [attribute | ="value"] selector

Is used to select elements with an attribute value containing a specific value

## [attribute ^ ="value"] selector

It is sed to select elements whose attribute begins with specified value

## [attribute $ ="value"] selector

It is sed to select elements whose attribute ends with specified value

## [attribute * ="value"] selector

It is used to select elements whose attribute value contain a specified value

## Comments

Will help you to comment your code

Syntax : /_ Commented code _/

## Colors

Will apply colors to your elements

4 ways to apply colors

1. color name - red, yellow, blue, orange.. etc
2. HTML5 color names - coral, teal etc...
3. Hexadecimal colors - Represented with 6 digit numbers
4. RGB - RED GREEN BLUE - rgb(23,23,45) or rgb(15%, 35%,45%)

0 to 255

## Background

To Define background effect of an element

## 1.Background-color

Sets a background color to our elements

2. Background-image

---

Sets the background image for your element

repeat-x - rpeats the background-image horizontally

repeat-y = repeats the background-image vertically

3. Background-position

---

It has got 3 different values

1. length - 100px 50px
2. percentage - 100%
3. Keywords - top right

4. Background attachment [scroll, fixed, local]

---

This specifies whether background image to should be scrolled or fixed

5. Background Clip

---

This defines how far the background should extend with in element

## Fonts

Will help you to set the font properties for our elements

Font-Family - Used to change the face of the font
Font-style - Property used to make font italic or oblique
font-variant - used to create small CAPS effect
font-weight - Help us increase or decrease how bold or light the font appears (for e.g bold)
font-size - helps us to increase or decrease the size of the font
font - Shorthand to specify other font properties

Value Common weight name
100 Thin (Hairline)
200 Extra Light (Ultra Light)
300 Light
400 Normal (Regular)
500 Medium
600 Semi Bold (Demi Bold)
700 Bold
800 Extra Bold (Ultra Bold)
900 Black (Heavy)
950 Extra Black (Ultra Black)

## CSS Units

1. Absolute Units

a. pixels (px)
b. inches (in)
c. centimeters (cm)
d. millimeters (mm)
e. points (pt)
f. picas (pc)

2. Relative Units

---

a. percentage (%)
b. font-sizes ( em & rem)
c. charcter-sizes (ex & ch)
d. viewport dimensions (vw & vh)
e. viewport max (vamx)
f. viewport maximum (vmax)

Relative units are based on

---

1.  The parent dimensions (%)
2.  The currently declared font-attributes (em, rem, ex, ch)
3.  The viewport dimensions (vh, vw, vmin, vmax)

Viewport - user's visible are of the webpage

## Opacity / transparency

This specifies the opacity/ tranparency of an element.

it can value from 0.0 to 1.0

The lower the value the more transparent it becomes

div {
opacity : 0.3
}

When using this all of its child elements inherit the same transparency

## Transaprency Using RGBA

If you don't want to apply opacity to child elelements use RGBA color value

RGBA - RedGreenBlueAlpha

background-color - rgba(red, green, blue, alpha)

alpha parameter is a number between 0.0 (fully transparent) to 1.0(fully opaque)

div {
background : rgba(0,128,0,0.3);
}

## Units

1. Absolute units
2. Relative

3. Absolute Units

---

1. Pixels (px)
2. inches (in)
3. Centimeters (cm)
4. Millimeters(mm)
5. points (pt)
6. picas (pc)

7. Relative Units

---

1. Percentage (%)
2. charcater-sizes(ex & ch)
3. font-sizes (em & rem)
4. Viewport dimensions (vh & vw)
   vh- viewport Height
   vw -viewport Width
   viewport - user's visible area
5. vmin - viewport minimum
6. vmax - viewport maximum

## Relative units are based on :

1. The parent dimensions (%)
2. Font-attributes (em, rem, ex, ch)
3. viewport dimensions (vh, vw, vmin, vmax)

ex - Relative to the x-height of the current font (rarely used)

x-height is roughly the height of lower case letters such a a,b,c,d,m, o...

ch - relative to the width of "0" 1ch == 8px

em - Relative to the font-size of the parent element

rem - relative to the font-size of root element

## Note : In amlmost every browser 16px is the standard for font

user can control the font-size

1rem = 16px

vh - viewport height
1vh - is equal to 1% of the current viewport height
vw - viewport width
1vw - is equal to 1% of the current viewport width
vmin - Uses the raito of smallest size. That is if the height of the browser
windows is less than its witdh 1vmin will be equivalent of 1vh. if the
width of the browser is less than its height 1vim is equivalent to 1vw

vamx - Uses the ratio of largest size. So if 1vamx is equivalent to 1vw if
viewport is wider than it is tall. if the browser is taller than it
is wide 1max is eqivalent to 1vh

Viewport - user's visible area

## Absolute Units

The aboluste units are fixed and length expressed in any of these will appears
exatcly the same size

1. Centimeters (cm) ( 1cm = 37.8 px)

---

use for "print" media type style sheet

2. Millimeter (mm) ( 1mm = 0.1cm = 3.78px)

---

---

## 1em == 16px == 0.17in == 12pt == 1pc == 4.2 mm ==0.42cm

3. Inches (in) (1in ==96px ==2.54cm)

---

Incjes is same as cenyimeters and will be used for "print" media type style sheet

4. Pixel (px)

---

It is most usable and considered measure in browsers. Normalizes measure for all
devices and display true measure

5. Point (pt) (1pt ==1/72 of in)

---

point is used for physical measurement - Print Media

6. Picas (pc) (1pc =12pt)

---

Picas is same as point

## CSS Text

Used to manipulate text using CSS properties

1. color - set the color of the text
2. direction - set the direction of the text
3. letter-spacing - to add or sutract space between the letter that makes up a word
4. word-spacing - add or subtract space between the words of a sentence
5. text-align - aling the text of a document
6. text-indent - indent the text of a pragraph
7. text-decoration - to underling, overline or strike through the text
8. text-transform - to capitaize the text or convert the text to
   uppercase or lower case letters
9. whit-space - to control the flow and format the text
10. text-shadow - to set the text shadow around the text

## Border

Allows us to specify style, width and color of an element's border

## Border-styles

Specifies what kind of borders to display

dotted - defined dotted border
dashed - defines a dashed border
solid - defines a solid border
double - defines a double border
groove - Defines a 3D grooved border, depends on background color
ridge - defines a 3D ridge border, depends on background color
inset - defines a 3D inset border, depends on background color
outset - defines a 3D outset border, depends on background color
none - Defines no border
hidden - Defined hidden border

Border-style can have one to four values

-   top border
-   right border
-   bottom border
-   left border

Border-width ( Will not work without border style)

---

specifies the wodth of our border

-   we can specify width using specific size
-   we can use predefined values thin, medium, thick
-   can have one to four values top, right, bottom , left

## Border-color

is used to set the color of the four borders

## Border-Sides

used to specify border for each Sides

## Border-Shorthand

To shorten the code , it is possible to specify the individual
border properties in one property

border - shorthand for the following individual properties

-   border width
-   border style
-   border color

## Rounded borders

Border-radius property to add rounded borders to an element

## Margins

Used to create space around elelemnts outside of any defined border

margin-top
margin-right
margin-bottom
margin-left

auto - The browser will calculate the margin
length - specify a margin in px, pt , em, cm, mm etc..
% - specify margin in %

-   Negative values are allowed

## Auto

1.  To horizaontally center the elelemnt with its container
    2 . Takes up specified width, remaining space will be split equally
    between left and right margins

## margin-collapse

Top and bottom margins of elements are sometimes collapsed in to a single margin
which is equal t the largest of tw margins.

## Note: This only happens with top and bottom margins.

## Paddings

Space between your content and your border.

it has four properties

padding-top
padding-right
padding-bottom
padding-left

length - specifes padding in px, pt, cm, em etc..
% - specifies padding in % width

Note : Negative values are not allowed

## Padding and element width

width property specifies the width of element's content area

if elelemnt has a specified width then padding added to that
elelemnt will be added to the total width of that elelemnt

width : 300
padding : 25 px
total width : width + padding right + padding left

(300px width + 25px left padding + 25px right padding)

## Outline

An outline is a line that is drawn around elements outside
the border to make the element stand out

outline is not part of element's dimensions

Elements total width and hieght is not affected by the width of the outline

outline-style - sets the style of outline
outline-color - sets the color of an outline
outline-width - sets width of an outline
outline-offset - specifies the space between outline and border, space is transparent
outline - short hand for style, width, color

## Width and Height

In order to set the width and height of an elelement correctly in all browsers
we should know how that box model works

## Total elelemt width

width + left padding + right padding + left border +
right border + left margin + right margin

## Total elelemt height

height + top padding + bottom padding + top border +
bottom border + top margin + bottom margin

## HTML Lists

unorderd Lists <ul>
Ordered Lists <ol>

## CSS Lists

1. can set different list item markers for orderd and unorderd list
2. set an image
3. add background color to list and list items

## List position

outside : means bullets points will be outside the list item
inside : means bullet pooints will be inside the list items

## display

specifies how an element is displayed

every element has a default display value depending
on what type of elelemt it is

The deafult display value for elelemnts is block or Inline

## block -level elelemnts

Always starts on a new line
takes up full width

div, h1-h6, p, form, header, footer, section

## Inline elelemnt

doesn't start on a new line
takes up as much width as necessary

span, <a>, <img>

## display : none

To hide and show elements without deleting or recreating them

## position

Specifies the type of positioning method used for an element

positions your elelemnt with help of top, left , bottom, right

1. static
2. relative
3. fixed
4. absolute
5. sticky

## position : static

HTML elelemnts are positioned static by deafult

static positioned elelemnts are not affected by the top, bottom, left, right

Always position according the to the normal flow of the page

## Document flow

order of code elelements

1. display
2. position
3. float

## top - margin-top

top - is a position property
it is used with position property relative or absolute

margin-top - It is element's own property

Position : relative

---

HTML elements are positioned according to the properties top, right, botoom , left

Position : absolute

---

Completely removes the element from the document flow and everything else renders
as if that absolute element didn't even exist

Absolutely positions an element inside of some parent container that it can reference.

Position : fixed

---

very similar to absolute position with some caveats.

always fixed based on the entire HTML element and it has nothing to do with parents

## Position : sticky

Combination of relative and fixed

## Float

specifies how an element should float

It is used for positioning and formatting

for e.g Let an image float left to the text in a container

It can have following properties

left- The element floats to the left of its container

right = the element floats to right of its container

none - The element doesn't float , this is a default option

inherit - The element inherits the float value of its parent

Note : Float property can be used to wrap text around images

## Float: Clear

Clears the eefect of floating on the parent element

## clear:left

clears the effect of floating left on its parent element

## clear:right

clears the effect of floating rigt on its parent element

## Specificity

Specificity is the means by which browser decide which CSS
property values are the most relevant to an element and therfore
will be applied

If two selectors apply to the same elelemnt, the one with heigher
specificity wins.

4 to 5 different categories

1. Inline-styles
2. Ids
   3.classes
   4.attributes
   5.elements

## Rounded Corners

Special corners to body or text

border-radius - property defines the radius of an elelemnts' corner

1. Assisgn specified background-color
2. assign border
3. assign background-image

border-radius is a short cut for below properties

border-top-left radius
border-top-right-radius
border-bottom-right-radius
border-bottom-left radius

It can have 1 to 4 values

border-radius : 15px 50px 30px 5px

                top-left corner   top-right corner bottom-right corner   bottom-left corner

border-radius : 15px 50px 30px

                top-left corner   top-right corner bottom-right corner   bottom-left corner

border-radius : 15px 50px

                top-left corner              top-right corner
                bottom-right corner          bottom-left corner

## Gradients

Gradients displays the combination of two or more colors

## Types

linear Gradient
Radial Gradient

## Linear Gradient (top-to-bottom) - default

Used to arrange two or more colors in linear format

background-Image is the one which helps with gradients

## 1st way

background: red;
background: linear-gradient(#FF0000, yellow);

## 2nd way

background-color : red /_ cab treated like fallabck _/
background-Image: linear-gradiant(crimson, white)

background-position : top left
background: red
background:linear-gradient(#FF0000, yellow);

## Linear Gradient

1. most common and useful type
2. gradient axis can go left-to-right or top-to-bottom
3. to make it left to right , you pass a additional parameter which starts with
   word "to right"
4. To syntax will work for corners. for instance if you wanted the axis of the
   gradient to start at the bottom left corner and go to the top right corner
   you could say "top right"

## Color-stops

You can decide where ou want any perticular color to start

## Repeat the liner gradient

Helps us to repeat the linear gradient

repeat-linear-gradient

## Radial Gradient

It will start at a single point and emanate outwards

The default is - first color which starts in the center of the elelemnt
and fade to the end color towards edge of the element.

To create radial gradient we must also define at least two color stops

radial-gradient (position, start color, ..., last color)

By default the shape is ellipse

## Transistions

Allows you to change property values smoothly

- transition
- transition-delay
- transition-duration
- transition-property
- transistion-timing-function

## How to use

1. CSS property you want to add an effect to
2. duration of the effect

## Transition-Timing-function

Specifies the speed curve of the transistion effect

liner - specifies transition effect with same speed from start to end
ease - specifies a transition effect with a slow start then moves fast
and ends slowly ( default)
ease-in - specifies tarnsition effect with slow start
ease-out - specifies tarnsition effect with slow end
ease-in-out - specifies tarnsition effect with slow start and end slow

## Transformations

Allows us to move, rotate, scale and skew elelemnts

transform - is the property

2d Transofrmation methods

1.transalate() - moves an element from its current postion (according to X and Y axis) 2. rotate() - rotate your elelemnt based on angle 3. scaleX() - Increases or decreases the size of an elelemnt ( as per width) 4. scaleY() - Increases or decreases the size of an elelemnt ( as per height) 5. sclae() - Increases or decreases the size of an elelemnt ( as per width and height) 6. skewX() - skews an elelent along the X axis nd Y axis 7. skewY() - skews an elelent along the X axis 8. skew() - skews an elelent along the Y axis 9. matrix - combines all the 2D transformations into one

matrix (scaleX(), skewY(), skewX(), scaleY(), tranasalateX(), transalateY())

## position:absolte vs transform

Position :absolute : element is placed according to its parent element.
changes according to its parent position

transform : This is based on itself. if the object is moved it will transalate according to new position

## 3D Transformations (transform use X, Y, Z)

rotateX - rotate an elelemnt aroudn X-axis at a given degree
rotateY - rotate an elelemnt aroudn Y-axis at a given degree
rotateX - rotate an elelemnt aroudn Z-axis at a given degree

## CSS Variables ( custom properties)

Gives us the mechanism to reuse and easily change the repeatedly occuring CSS properties

To declare CSS variable we will have to use double dash before the name of the variable

body {
--english-green-color : #00FF00
}

in order to use that variable we can use var() function

    .my-green-component {
        background-color : var(--english-green-color)
    }

The easiest wat to manage our css variables is by declaring them into :root psedo calss.

Havimg them im the :root will ensure tha all selectors will gain access to these variables

:root {
--english-green-color : #00FF00
}

## :root

Pseudo Class matches the root elelement of the tree representing the document.

in HTML :root represents the <html> elelemnt and is identical to selector html

complex websites have very large amounts of CSS and often with lot of repeated values

Custom properties allows a value to be stored in one place then referenced in
multiple other places

An Additional benifit is semantic identifiers

for e.g. --main-text-color this is easier to understand than #00FF00

## Shorcuts to generate HTML

div>p - creates DIV element and p as a child element of div

div>p>span - creates DIV element and p as a child element div
and span as child element of p

div.one - this would create div element with class property

div#id - this would create div with id property

!+tab key - that will fetch html template

doc+tab key - this will fetch html template

lorem8 - will generate lorum ipsum content with 8 words

lorem50 - will generate lorum ipsum content with 50 words

## Media queries

Allows us to customize the presentation of our web pages for a specific range of
devices like mobile phones, tablets, desktops etc... without any change in the markup

media query is a logical expression can be resolve to true or false

media query will be true if the media type specified in the media query matches
the type of device in which html content being diplayed on.

## Z-Index

Property specifies stack order of an element

1. An elelemnt with greater stack order is always in front of an element
   with lower stack order

2. Only works with positioned elements

positions : absolute, relative, fixed, sticky

3. It can have negative values

4. it can't have decimal values

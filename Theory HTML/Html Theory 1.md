HTML - Hypertext Markup Language

     - Create web pages
     - Widely used in web technologies
     - Is a Markup Language not a programming language

Hypertext

-   Text with in Text - Link two or more webpages - Click on link will take you to new page

` <!doctype html>` - This tag specifies the language we write on the page , in our case it is HTML5

`<html>` - Starting point of our HTML code, it signals that from here we are going to write HTML code

` <head>` - Here we write meta data for the pages, mostaly for search engines for SEO Purpose

` <body>` - This is where content of the page goes for e. h headers, paragraphs, images, hyperlinks

` <title>` - Title of HTML page

## HTML Element

Element is defined by start tag, some content and end tag

Element : `<html> something </html>`

`<body> come contnent </body>`

Some elements will have no end tags ( closing tags)

`<title> Name </title>`
`<br> name </br>` - This is wrong as there will be no end tag

`<br>` - Empty element

`<hr>` - No content

Only content inside the body will displayed in the webpages

## Features

1. simple and easy
2. Platform independent ( Windows, Mac, Linux)
3. case insensitive language
4. Write all tags in lowercase for consistency and for the better readability

## Building Blocks of HTML

Tags - Surrounds the content and apply meaning to it. Written using < and > brackets

Attribute - Porvides extra information about the element

`<tag attribute-name="attribute-value"></tag> `

1. Heading Tags -

```
       </h1>, </h2>, <h3>, <h4>, <h5>, <h6>
       bold - <b></b>
       Italics - <i></i>
       Underline - <u></u>
```

2. Meta Tags -

```
Doctype, title, link, meta, style

style - <style>
              .website {
              color: teal;
              }
       </style>

link - <link href="./styles.css" rel="stylesheet">
```

3. Text Tags - `<p>, <h1> to <h6>, <strong>, <em>`

4. Link Tag - `<a>`

5. Image Tag - `<image>, <area>`

6. List Tags - `<ul> <ol> <li>`

7. Table Tags - table, tr, td, thead, tbody, th

8. Form tags - Form, Input, textArea, select

9. Script Tags - `<Script> , <noscript>`

10. Mark - Tag will Mark or Highlight a text that is of relevance

11. code - Defines a fragment of computer code

12. small - defines smallar text copyright or side-commennts

13. sub - Subscript , will be used for displaying text as subscript for e.g. Chemical forumlas

14. sup - Superscript, will be used for displaying text as superscript for e.g. Maths Algebra

15. del - Tag is used to identify text that has been deleted from a document but
    retained to show the history of modification made to the document.

16. ins - Tag defines a text that has been inserted into a document

17. cite - Defines the title of creative work ( book, poem, song, movie)

18. q - quotation

19. abbr - abbreviation

20. p - paragraph

21. space - to add space se `&nbsp;`

## HTML Text Tags

```
<b> - bold
<i> - italic
<u> - underline
<strong>
<em> - display content in italic
<mark> - to highlight the text that is of relevance
code - Defines a fragment of computer code
<small> - Defines smaller text e.g. copyright or other side-comments
<sup> - Super Script
<sub> - subscript
<del> - is used to identify text that has been deleted from a document
but retained to show the history of modification to the document
<ins> - is used when a text that has been inserted into a document
<cite> - Defins title of some creative work
<q> - Quotation
<abbr> - abbreviation

<address> - To display Address
&nbsp; - used to add space
```

## Link Tags

```
<a> - achor tag , defines a hyperlink which is used to provide link from one page to other page.

href - Most import attribute of element
target -  _blank - opens link in a new table_parent, _self, _top
```

## Image Tags

```
<img> - Will help us to display images
src - which is source
alt - Alternate text
```

## List Tags

-   Ul - Unordered List -> No order is required
-   Ol - Ordered List - Use it when you are lsiting steps which needs be in order

## HTML CSS

1. CSS - Cascading Stylesheet - To format the layout of my webpage - With CSS you can control the color, font, size of the text,
   elemepnt position, background, background images, background colors

2. CSS - Can be added to HTML docuemnt in 3 ways

-   Inline - by using style attribute inside HTML Elelment
-   Internal - by using `<style>` element in `<head>` section
-   External - by using `<link>` element to link external CSS

## CSS Colors, Fonts, sizes

-   color - defines the text of your color
-   font-family - defines font to be used
-   font-size - defines size of the font
-   border - define border for all HTML elelments
-   padding - defines space between your text and the border
-   margin - defines the space between border

## HTML Forms

Required to collect some data from the user. for e.g Name, Email, Phone
May be used for registartion where we collect information.

```
<form action="/user" method="get">
      form elements
</form>
```

HTTP Methods - GET, PUT, POST, DELETE ( CRUD Operations)

## HTML FORM Controls

1. Text Input Control - Single line Input, Password Input, Multiline Input
2. Checkbox Control - value, checked
3. Radiobox Control
4. Selectbox control
5. File Control
6. Hidden Control - Hides the data inside the page which later can be used to pass to server
7. Clickable button
8. Submt and reset Button

## Block-level elements & Inline elements

-   Block level element occupies the entire space of the parent
-   Every element has default display value depending on what type it is
-   There are two display values : block and inline
-   Always starts on new line and takes up the full width available
-   occupies entire space of the parent

## Inline elements

1.  Doesn't start on a new line
2.  Only takes up as much width as necessary
3.  Can not contain block-level element

## Block-Level elements

```
1. H1-H6
2. <table>
3. <p>
4. <div>
5. <form>
6. <video>
7. <hr>
8. <address>
9. <header>
10. <footer>
```

## Inline elements

```
1.  <span>
2.  <a>
3.  <button>
4.  <sup>
5.  <sub>
6.  <textArea>
7. <label>
8. <b>
9. <strong>
10. <img>
```

span - container used to amrk up a part of text or part of document

div - Known as DIVISON Tag

       It is often used as a container for other HTMl elements

       defines a division or a section in an HTML document

       any sort of content can be placed inside <div> tag

```
<div>
      <p></p>
      <h1><h1>
      <labe>
      <span>
      .....
</div>
```

## label vs span

Label is used when we have form or input elements

Span is used anywhere, this is a general container for any inline content

## HTML DOM ( Document Object Model)

When page is loaded, browser creates a docuemnt object Model of the page

Usage: With HTML DOM Javascript can access all the elements of HTML Document

       Javascript can add, remove, change all the HTML elelments, HTML Attributes,
       CSS Styles in the page.

       Javascript can react to HTML events, can create new HTMl events in the page.

## value vs innerHTML

       Setting the value is normally used for input/form elements.
       innerHTML is normally used for div, span, td and similar elements.

## Video

`<Video controls autoplay muted>`

Will help you display video in the page

controls - The browsers will offer controls to allow the user
to control audio, playback, volume, pause /Resume

autoplay - The audio will automatically begin playback as soon as it can.

muted - will mute the audio

## Audio

`<Audio controls autoplay muted>`

Will help you display audio in the page

controls - The browsers will offer controls to allow the user
to control audio, playback, volume, pause /Resume

autoplay - The audio will automatically begin playback as soon as it can.

muted - will mute the audio

## HTML Class

This is an attribute which is used to specify a class for an HTML element

Multiplw HTML elements can share same class

## Padding & margin

Padding - is the space between the text and border

margin - is the space between the elements

## HTML Responsive

Responsive web design is about creating webpages that look good on all devices.
<br>
This will automatically adjust for different screen sizes and viewports to create responsive website we need <meta> tag

`<meta name="viewport" content="width=device-width", intial scale 1.0">`

This will set the viewport of your page whivh will give browser instructions on how to control page diemsnsions and scaling.
<br>
meta - Elelment Speicfy the charcter set, page description, keywords,
author of the document and viewport settings. This will set the viewport of our page which will give instructions to browser
on how to control page's deminesion and scaling

viewport - This is user's visible are of the webpage.
This varies with device.
This will be smaller on mobile phone and larger on computer screen
<br>
Initial-scale - Governs the zoom level when page is loaded for the first time.

## Semantic elelments

Elements with meaning and clearly tell us what the content is about

```
<article>
<aside>
<details>
<figcaption>
<figure>
<footer>
<header>
<nav>
<main>
<mark>
<section>
<summary>
<time>
```

## Non Semantic Elements

```
<div>
<span>
<p>
```

Tells nothing about the content

```
<div id="nav">
<div class="header">
<div class="footer">
```

## CSS3

1. Colors Names -
   The 17 standard colors are: aqua, black, blue, fuchsia, gray, green, lime, maroon,
   navy, olive, orange, purple, red, silver, teal, white, and yellow.

2. HTML5 Colors
3. Hexadecimal colors - #
4. RGB colors - rbg()

Selectors

1. Combinator Selector

    a. decendent selector (space)
    b. child selector (>)
    c. adjacent sibing selector (+)
    d. general sibling selector (~)

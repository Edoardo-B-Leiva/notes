[Edoardo Borgia Leiva](https://edoardo-b-leiva.github.io) (31st October 2023 - x)
# CSS3
## CSS Introduction
CSS3 (a.k.a. Cascade Style Sheets) is a ... made to complement HTML5 and give it styling to it's content.  
There are different alternatives that innovate to the existing idea of traditional CSS, some examples are:
- [SASS/SCSS](https://sass-lang.com/)
- [Bootstrap](https://getbootstrap.com/)
- [Tailwind](https://tailwindcss.com/)

More Documentation can be found in different websites, the most recommended are:
- [Mozilla MDN](https://developer.mozilla.org/)
- [W3 Schools](https://www.w3schools.com/css/default.asp)

__This notes will include links that redirect to the correspondent MDN documentation page.__

CSS styling can be implemented in 3 different ways inside an HTML5 file:
- [`<style>` tag](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/style):

The CSS styling is written directly inside the HTML file using this tag inside the `<head>`. The style will apply to all the HTML document but cannot be used in multiple of them.
```html
<html>
    <head>
        <style>
            p{
                color: #beef;
                top: 50%;
            }
        </style>
    </head>
</html>
```
- [`<p style="">` attribute](https://developer.mozilla.org/en-US/docs/Web/API/HTMLElement/style):

The styling is written inside this attribute, the styling written in this attribute will apply exclusively to the tag it's in.
```html
<html>
    <head>
        ...
    </head>
    <body>
        <p style="color: #f00d; position: absolute;">Lorem Ipsum...</p>
    </body>
</html>
```
- [`<link rel="stylesheet href="/path/to/file.css" />` tag](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/link):

This tag located in the `<head>` will link an already existing CSS file. This gives the possibility to apply the same styling to multiple HTML documents.
```HTML
<html>
<head>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <p>Lorem Ipsum...</p>
</body>
</html>
```
```CSS
p{
    color: #face;
    position: relative;
    top: 50%;
}
```
---
## HTML/CSS Identifiers
There are multiple ways to identify specific parts of a webpage:
### Classes
### IDs

---
## [CSS Box model](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/The_box_model)
The HTML5 components are composed of 4 "main subcomponents":
### Content
It's the content written in the HTML file, no further explanation should be needed.
### [Padding](https://developer.mozilla.org/en-US/docs/Web/CSS/padding)
The padding is a CSS property that defines a space between the [Content](#Content) and the [Border](#Border).
```CSS
p{
    padding: <size/size-top/size-vertical> <size-horizontal/size-right> <size-bottom> <size-left>;
    padding-top: <size-top>;
    padding-bottom: <size-bottom>;
    padding-left: <size-left>;
    padding-right: <size-right>; 
}
```
### [Margin](https://developer.mozilla.org/en-US/docs/Web/CSS/margin)
The margin is the space used to separate the [Border](#border) to everything else in the page.
It is defined in CSS using the border group of properties.
```css
p{
    margin: <size/size-top/size-vertical> <size-horizontal/size-right> <size-bottom> <size-left>;
    margin-top: <size-top>;
    margin-bottom: <size-bottom>;
    margin-left: <size-left>;
    margin-right: <size-right>; 
}
```
### [Border](https://developer.mozilla.org/en-US/docs/Web/CSS/border)
The border is located between the [Margin](#margin) and [Padding](#padding), it's thickness, style, color, radius can be modified with these properties:
```css
p{
    border:<size> <style> <color>;
    border-color: <color>;
    border-style: [none, solid, dashed, dotted, etc.];
}
```
## [ULs](), [OLs]() & [LIs]()
### [List styles]()
It's possible to freely customize Bullet Lists using these CSS properties.
```css
p{
    list-style: <none/>;
    list-style-type: ;
    list-style-position: <inside/outside>;
    list-style-image: url("<src>");
}
```

[Edoardo Borgia Leiva](https://edoardo-b-leiva.github.io)
# HTML5
More Documentation can be found in different websites, the most recommended are:
- [Mozilla MDN](https://developer.mozilla.org/)
- [W3 Schools](https://www.w3schools.com/css/default.asp)
## HTML5 Introduction
HTML5 (HyperText Markup Language) is the base of a webpage where it's contents resides.
It's structured using `<tags>` with its name and elements.
```html
<html>
    <head>
        <title>Document</title>
    </head>
    <body>
        <p>Lorem Ipsum...</p>
    </body>
</html>
```
### Little mention about [`<style>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/style)
This element is used in the `<head>` to embed [CSS styling](../CSS3/CSS3.md) into the HTML file.
## The base structure
The HTML document is structured on it's root by 3 different tags:
- `<html>`
- `<head>`:
  The "head" of the document, it contains information not made for being displayed, such as encodings, files to link, styling, etc.
- `<body>`:
  The body contains the actual content of the webpage such as: text, images, hyperlinks, embeds, videos, etc.
## The title...
The most important thing when trying to sell a book is choosing a memorable title that catches the eyes of interested people.
For this same purpose, on the tabs there's a space reserved for text, this text can be filled using the tag `<title>` in the head.
```html
<title>An awesome website</title>
```
## Text elements and text modifiers
The most basic content you will find in a webpage is text.
There are many ways to display text in a webpage and to display it in different ways.
### Headers
Headers go from 1 (being the main and biggest) to 6 (the most minor), they are defined using the `<h1>` to `<h6>` tags.
```html
<h1>Header 1</h1>
<h2>header 2</h2>
<h3>Header 3</h3>
<h4>Header 4</h4>
<h5>Header 5</h5>
<h6>Header 6</h6>
```
### Paragraphs
Paragraphs are the main element in basic html webpages. Nowadays used mainly to improve upon SEO.
```html
<p>Your text goes here</p>
```
### Bold
You can easily make your text **BOLD** using the `<b>` tag.
```html
<b>Your bold text here...</b>
```
### Italic
To italicize your text you can easily use the <i> tag.
```html
<i></i>
```
### Underline
### Strong
From a visual perspective, `<stong>` is exactly like [`<b>`](#bold).  
But if we instead we see in a technical perspective, strong can be important to do SEO operations.
## Span
## Div
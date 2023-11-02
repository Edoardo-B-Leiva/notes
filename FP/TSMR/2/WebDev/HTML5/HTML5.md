[Edoardo Borgia Leiva](https://edoardo-b-leiva.github.io)
# HTML5
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
More Documentation can be found in different websites, the most recommended are:
- [Mozilla MDN](https://developer.mozilla.org/)
- [W3 Schools](https://www.w3schools.com/css/default.asp)
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
<html>
    <head>
        <title>An awesome website</title>
    </head>
    ...
</html>
```
## Text and texting
The most basic content you will find in a webpage is text.
There are many ways to display text in a webpage and to display it in different ways.
### Headers
Headers go from 1 (being the main and biggest) to 6 (the most minor), they are defined using the h1 to h6 tags.
```html
<html>
<body>
    <h1>Header 1</h1>
    <h2>header 2</h2>
    <h3>Header 3</h3>
    <h4>Header 4</h4>
    <h5>Header 5</h5>
    <h6>Header 6</h6>
</body>
</html>
```
###paragraphs

---
tags:
  - TSMR2
  - TSMR
  - IT
  - CSS
  - BAW
  - FP
---

Author: [Edoardo Borgia Leiva](https://edoardo-b-leiva.github.io)
# CSS Cheat sheet
## Units
### Colors
|Color Unit|Description|Example 1|Example 2|
|-|-|-|-|
|RGB||`rgb(25,52,99)`||
|RGBA||`rgba(53,124,255,88)`||
|Hex 4 bits||`#14C`|`#99FC`|
|Hex 8 bits||`#000000`|`#FFFFFF88`|
|Color Name||`blue`|`whitesmoke`|
### Measurements
|Measure unit|Type|a|Description|
|-|-|-|-|
|Pixels|Absolute|`px`|Individual pixel counting|
|Percentage|Relative|`%`|Percentage of the parent element's size|
|em|Relative|`em`||
|rem|Relative|`rem`||
|vh|Relative|`vh`|Viewport horizontal size's percentage|
|vw|Relative|`vw`|Viewport vertical size's percentage|
## Positioning
### `position:`
Defines the way other position-related attributes work

|Direction|Description|
|-|-|
|`static`|Position related attributes will be ignored and position will be default.|
|`absolute`|Position is based off its parent element's size|
|`relative`|Position attributes are relative to the other HTML elements around the affected one|
|`fixed`|Position will reference the browser's view-port instead of the DOM|
### `float` 
Defines which direction the HTML element will be place itself towards.

|Specified value|Computed value|
|---|---|
|`right`|block|
|`left`|block|
|`inline`|block|
|`inline-block`|block|
|`inline-table`|table|
|`table-row`|block|
|`table-row-group`|block|
|`table-column`|block|
|`table-column-group`|block|
|`table-cell`|block|
|`table-caption`|block|
|`table-header-group`|block|
|`table-footer-group`|block|
|`inline-flex`|flex|
|`inline-grid`|grid|
|_other_|_unchanged_|

- **top: \<size\>**: Distance from top of father element.
- **left: <size\>**: Distance from left wall of father element.
## Element spacing
- **_Margins_**: Space between element's border and other element's own margin.
  - **margin**: defines margin spacing; one, two, and four values are supported.
    - **-top | -bottom | -left | -right**: Define the spacing of the correspondent side.
- **_Borders_**: Border between the Margin and the Padding.
  - **border**: defines thickness, style, color and other information about the border.
    - **-color**: Defines the color of the border.
    - **-style**: Defines the style of the border.
    - **-radius**: Define the radius of the border.
    - **-top | -bottom | -left | -right**: Define the thickness of the correspondent side.
- **_Paddings_**: Space between the element's content and it's border.
  - **padding**:
	- **-top | -bottom | -left | -right**: Define the spacing of the correspondent side.
## Flex, Flexbox & Grid
## ULs, ILs & LIs
### UL: Unordered lists
- `list-style-type: <disc/cirle/square/decimal/cjk-decimal/decimal-leading-zero/lower-roman/upper-roman/lower-greek/...>`: Styling for the bullet points.
## Simple CSS selectors

| Selector   | Description                   | Example             |
| ---------- | ----------------------------- | ------------------- |
| `*`        | Selects every HTML element    | `*{color:red;}`     |
| `.<class>` | Elements with the given class | `.navbar{top: 0%;}` |
| `#<id>`      | Element with the given id     | `#footer{bottom: 0%;}` |
| `<HTMLElement>` | All corresponding HTML element | `p{font-size:16px;}` |
| `<any>.<class>` | All corresponding selectors with given class |`p.navbar{font-weight:bold;}`|
| `<any> <any>` |||
| `<any> + <any>`|||
| `<any> > <any>`|It matches only elements matched by the last selector that are direct children of the previous selector||
| `<any> , <any>`|Selects all corresponding elements||
| `<any> ~ <any>`|||
| `.<class> .<class>` |||
| `<any>[<attribute>]` |Selects all corresponding elements with given attributes||
## CSS pseudo-selectors
|Pseudo-selector|Description|Example|
|-|-|-|
|`:hover`|Only applies whenever the cursor is hovering on the element.||
|`::first-line`|Only applies to the first line of text in the selector, mostly used in `<p>`.||
|`::last-line`|Only applies to the last line of text in the selector, mostly used in `<p>`.||

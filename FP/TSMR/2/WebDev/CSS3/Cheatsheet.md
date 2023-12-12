Author: [Edoardo Borgia Leiva](https://edoardo-b-leiva.github.io)
# CSS Cheatsheet
## Units
### Colors
- Hex colors
  -`#rgb(a) : #DEAD`
  - `#rrggbb(aa): #BEEFACE`
- rgba(red_channel, green_channel, blue_channel, alpha_channel): `rgba(255,0,234,100)`
- Color names (red, green, blue, white, gray, etc.): `red`
### Measurements
- Absolute units
  - pixels: `1337px`
- Relative units
  - percentage: `69%`
  - em: `404em`
  - rem: `420rem`
## Positions
- `position: <static/absolute/relative/fixed/float>`: Defines the way other position-related attributes work:
  - `static`: Position-related attributes will be ignored and position will be default.
  - **: absolute**: Position is based off its father element size.
  - **: relative**: Position attributes are based off other elements.
  - **: fixed**: Position will reference the view port instead of HTML Document structure.
  - **: float**: 
- **top: \<size\>**: Distance from top of father element.
- **left: <size\>**: Distance from left wall of father element.
## Element spacings
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
- `*`: Every single element
- `.<classname>`: elements with given class
- `#<id>`: elements with given id
- `<elementname>`: all given elements
- `<HTMLElement>.<classname>`: all given element with given class
- `<something> <something>`
- `<something> + <something>`
- `something,something`
- `something~something`
- `.class .class`: Selects all elements with both _name1_ and _name2_ set within its class attribute
- `.class.class`: Selects all elements with both _name1_ and _name2_ set within its class attribute
- `something > something`: where the first element is the second's element parent

# Learn CSS

CSS stands for Cascading Style sheets.

### CSS Syntax

CSS syntax is made of two parts which are:

- selector: THis points to the HTML element you want to style
- declaration: The declaration part contains one or more declarations separated by a semicolon

e.g 
```css
p {
color: red;
text-align: center
}
```

### Types of CSS Selectors
- Simple selectors e.g select based on name, id or class
- Combinator sectors eg select based on a specific relationship between them
- Pseudo-class selector e.g select elements based on certain state
- Pseudo-element selectors e.g select and style a part of an element
- Attribute selectors e.g select elements based on an attribute or attribute value

**Note**
- You can specify in css that only specific element should affect a certain child element of a certain class like below;

```css
p.center {
  text-align: center;
  color: red;
}
```

#### Universal Selector
This selects all HTML elements on the page
The common use of this selector is as below;
```css
* {
  margin: 0;
  padding: 0;
}
```

#### Grouping Selector
This selects all the HTML elements with same style definitions 
e.g
```css
h1, h2, p {
  text-align: center;
  color: red;
}
```

### Cascading Order
The cascade is an algorithm that defines how user agents combine property values originating from different sources. The cascade defines the origin and layer that takes precedence when declarations in more than one origin or cascade layer set a value for a property on an element.

All the styles in a page will "cascade" into a new "virtual" style sheet by the following rules, where number one has the highest priority:

1. Inline style (inside an HTML element)
2. External and internal style sheets (in the head section)
3. Browser default

So, an inline style has the highest priority, and will override external and internal styles and browser defaults.

### Colors
##### RGB Value
In CSS, a color can be specified as an RGB value, using this formula:

rgb(red, green, blue)

Each parameter (red, green, and blue) defines the intensity of the color between 0 and 255.

For example, rgb(255, 0, 0) is displayed as red, because red is set to its highest value (255) and the others are set to 0.

To display black, set all color parameters to 0, like this: rgb(0, 0, 0).

To display white, set all color parameters to 255, like this: rgb(255, 255, 255).

##### RGBA Value
RGBA color values are an extension of RGB color values with an alpha channel - which specifies the opacity for a color.

An RGBA color value is specified with:

rgba(red, green, blue, alpha)

The alpha parameter is a number between 0.0 (fully transparent) and 1.0 (not transparent at all):

##### HEX Value
In CSS, a color can be specified using a hexadecimal value in the form:

#rrggbb

Where rr (red), gg (green) and bb (blue) are hexadecimal values between 00 and ff (same as decimal 0-255).

For example, #ff0000 is displayed as red, because red is set to its highest value (ff) and the others are set to the lowest value (00).

To display black, set all values to 00, like this: #000000.

To display white, set all values to ff, like this: #ffffff.  

##### HSL Value
In CSS, a color can be specified using hue, saturation, and lightness (HSL) in the form:

hsl(hue, saturation, lightness)

Hue is a degree on the color wheel from 0 to 360. 0 is red, 120 is green, and 240 is blue.

Saturation is a percentage value. 0% means a shade of gray, and 100% is the full color.

Lightness is also a percentage. 0% is black, 50% is neither light or dark, 100% is white

##### HSLA Value
HSLA color values are an extension of HSL color values with an alpha channel - which specifies the opacity for a color.

An HSLA color value is specified with:

hsla(hue, saturation, lightness, alpha)

The alpha parameter is a number between 0.0 (fully transparent) and 1.0 (not transparent at all):
## HTML Images :

**Images can improve the design and the appearance of a web page.**

**Example :**
```
<img src="img_chania.jpg" alt="Flowers in Chania">

```
### HTML Images Syntax :

**In HTML, images are defined with the `<img>` tag. The `<img>` tag is empty, it contains attributes only, and does not have a closing tag.**

**The src attribute specifies the URL (web address) of the image:**
```
<img src="url">
```
## CSS height and width Values :

**The height and width properties may have the following values:**

1. `auto` - This is default. The browser calculates the height and width
2. `length` - Defines the height/width in px, cm etc.
3. `%` - Defines the height/width in percent of the containing block
4. `initial` - Sets the height/width to its default value
5. `inherit` - The height/width will be inherited from its parent value

## Center Align Elements :

**To horizontally center a block element (like `<div>`), use margin: auto;**

**Setting the width of the element will prevent it from stretching out to the edges of its container.**

**Example :**
```
.center {
  margin: auto;
  width: 50%;
  border: 3px solid green;
  padding: 10px;
}
```

## Transparent Image :

**The opacity property can take a value from 0.0 - 1.0. The lower value, the more transparent:**
```
img {
  opacity: 0.5;
}
```

## CSS Color :
**Color can really bring your pages to life :**

**The color property allows you to specify the color of text inside an element. You can specify any color in CSS in one of three ways:**
```
 1. rgb values : These express colors in terms of how much red, green and blue are used to make it up. For example: rgb(100,100,90)
 2. hex codes : These are six-digit codes that represent the amount of red, green and blue in a color, preceded by a pound or hash # sign. For example: #ee3e80
 3. color names :There are 147 predefined color names that are recognized by browsers. For example: DarkCyan.
Here is a link (Links to an external site.) that can help you pick a color for your site .
this information refrenced by : HTML & CSS Design and Build Websites By Jon Duckett .
```

## CSS Fonts :

**The CSS font properties define the font family, boldness, size, and the style of a text.**

**Difference Between Serif and Sans-serif Fonts:**

![Difference Between Serif and Sans-serif Fonts](https://www.w3schools.com/css/serif.gif)

## CSS Units :

**CSS has several different units for expressing a length.Many CSS properties take "length" values, such as width, margin, padding, font-size, etc.Length is a number followed by a length unit, such as 10px, 2em, etc.A whitespace cannot appear between the number and the unit. However, if the value is 0, the unit can be omitted.For some CSS properties, negative lengths are allowed.There are two types of length units: absolute and relative.**

|Unit	|Description|
|cm	|centimeters|
|mm	|millimeters|
|in	|inches (1in = 96px = 2.54cm)|
|px *	|pixels (1px = 1/96th of 1in)|
|pt	|points (1pt = 1/72 of 1in)|
|pc	|picas (1pc = 12 pt)|



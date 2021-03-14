## HTML Text :

### * HTML Headings : HTML headings are defined with the <h1> to <h6> tags. 

![HTML Headings](https://www.oxfordwebstudio.com/user/pages/06.da-li-znate/sta-je-html/sta-je-html.jpg)

 - Examples :

#### <h1>Heading 1</h1>
#### <h2>Heading 2</h2>
#### <h3>Heading 3</h3>
#### <h4>Heading 4</h4>
#### <h5>Heading 5</h5>
#### <h6>Heading 6</h6>

#### Search engines use the headings to index the structure and content of your web pages. Users often skim a page by its headings. It is important to use headings to show the document structure.

### * HTML Paragraphs : The HTML <p> element defines a paragraph.

**A paragraph always starts on a new line, and browsers automatically add some white space (a margin) before and after a paragraph.**

- Examples :

#### <p>This is a paragraph.</p>
#### <p>This is another paragraph.</p>

### * HTML Text Formatting : HTML contains several elements for defining text with a special meaning.

#### **HTML Formatting Elements**

#### **Formatting elements were designed to display special types of text:**

#### <b> - Bold text
#### <strong> - Important text
#### <i> - Italic text
#### <em> - Emphasized text
#### <mark> - Marked text
#### <small> - Smaller text
#### <del> - Deleted text
#### <ins> - Inserted text
#### <sub> - Subscript text
#### <sup> - Superscript text

***HTML Formatting Elements also provide semantic information (e.g. where emphasis should be placed, the definition of any acronyms used, when given text is a quotation).***

## Introducing CSS : 

* What is CSS?
1. CSS stands for **C**ascading **S**tyle **S**heets
2. CSS describes how HTML elements are to be displayed on screen, paper, or in other media
3. CSS saves a lot of work. It can control the layout of multiple web pages all at once
4. External stylesheets are stored in CSS files

### * Why Use CSS?
**CSS is used to define styles for your web pages, including the design, layout and variations in display for different devices and screen sizes.**

### A CSS rule-set consists of a selector and a declaration block:
1. The selector points to the HTML element you want to style.
2. The declaration block contains one or more declarations separated by semicolons.
3. Each declaration includes a CSS property name and a value, separated by a colon.
4. Multiple CSS declarations are separated with semicolons, and declaration blocks are surrounded by curly braces.

#### * Example :
In this example all **<p>** elements will be center-aligned, with a red text color:
p {
  color: red;
  text-align: center;
}

### There are three ways of inserting a style sheet:

1. External CSS : With an external style sheet, you can change the look of an entire website by changing just one file! Each HTML page must include a reference to the external style sheet file inside the <link> element, inside the head section.
2. Internal CSS : An internal style sheet may be used if one single HTML page has a unique style. The internal style is defined inside the <style> element, inside the head section.
3. Inline CSS : An inline style may be used to apply a unique style for a single element. To use inline styles, add the style attribute to the relevant element. The style attribute can contain any CSS property.

#### CSS Selectors : CSS selectors are used to "find" (or select) the HTML elements you want to style.

**All CSS Simple Selectors**
|Selector|	Example	  |   Example description|
|.class	    |.intro	     |Selects all elements with class="intro"|
|#id	         |#firstname	 |Selects the element with id="firstname"|
|*	         |*	         |Selects all elements|
|element	     |p	         |Selects all <p> elements|
|element,element,..	|div, p	|Selects all <div> elements and all <p> elements|

## Basic JavaScript Instructions :

#### * JavaScript Statements :
**JavaScript statements are composed of: Values, Operators, Expressions, Keywords, and Comments. This statement tells the browser to write "Hello Dolly." inside an HTML element with id="demo":**

#### * JavaScript Comments : JavaScript comments can be used to explain JavaScript code, and to make it more readable. JavaScript comments can also be used to prevent execution, when testing alternative code.

#### * JavaScript Variables : JavaScript variables are containers for storing data values.

#### * JavaScript Arrays :  JavaScript arrays are used to store multiple values in a single variable.

#### * JavaScript Expressions : An expression is any valid unit of code that resolves to a value.

#### * JavaScript Operators : JavaScript operators are used to assign values, compare values, perform arithmetic operations, and more.

#### * JavaScript Strings : JavaScript strings are used for storing and manipulating text.

## Decisions and Loops : 

#### Conditional Statements : Very often when you write code, you want to perform different actions for different decisions.

#### You can use conditional statements in your code to do this.

#### In JavaScript we have the following conditional statements:

1. Use if to specify a block of code to be executed, if a specified condition is true
2. Use else to specify a block of code to be executed, if the same condition is false
3. Use else if to specify a new condition to test, if the first condition is false
4. Use switch to specify many alternative blocks of code to be executed

#### Comparison Operators : Comparison operators are used in logical statements to determine equality or difference between variables or values.

**Examples :Given that x = 5, the table below explains the comparison operators:**

|==    |equal to	|x == 8	|false|		
|===	|equal value and equal type	|x === 5	|true|		
|!=	|not equal	|x != 8	|true|	
|!==	|not equal value or not equal type	|x !== 5	|false|	
|>	|greater than	|x > 8	|false|	
|<	|less than	|x < 8	|true|	
|>=	|greater than or equal to	|x >= 8	|false|	
|<=	|less than or equal to	|x <= 8	|true|

### JavaScript if else and else if : Use the if statement to specify a block of JavaScript code to be executed if a condition is true. Use the else statement to specify a block of code to be executed if the condition is false.Use the else if statement to specify a new condition if the first condition is false.
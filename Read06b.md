# What is CSS?

**CSS:** (Cascading Style Sheets) allows you to create great-looking web pages, but how does it work under the hood? This article explains what CSS is, with a simple syntax example, and also covers some key terms about the language.
>
~~~
Prerequisites: Basic computer literacy,                                   basic software installed,basic knowledge of working with files, and HTML basics (study Introduction to HTML.)
~~~
>
~~~
Objective:	To learn what CSS is.
~~~


## CSS syntax:
CSS is a rule-based language — you define rules specifying groups of styles that should be applied to particular elements or groups of elements on your web page. For example "I want the main heading on my page to be shown as large red text."

The following code shows a very simple CSS rule that would achieve the styling described above:

>
~~~
h1 {
    color: red;
    font-size: 5em;
}
~~~

**The rule opens with a selector . This selects the HTML element that we are going to style. In this case we are styling level one headings (<h1>).**

**We then have a set of curly braces { }. Inside those will be one or more declarations, which take the form of property and value pairs. Each pair specifies a property of the element(s) we are selecting, then a value that we'd like to give the property.**

**Before the colon, we have the property, and after the colon, the value. CSS properties have different allowable values, depending on which property is being specified. In our example, we have the color property, which can take various color values. We also have the font-size property. This property can take various size units as a value.**

> A CSS stylesheet will contain many such rules, written one after the other.

~~~
h1 {
    color: red;
    font-size: 5em;
}

p {
    color: black;
}
~~~

### Three Ways to Insert CSS
**There are three ways of inserting a style sheet:**

- External CSS
- Internal CSS
- Inline CSS

1- External CSS:

With an external style sheet, you can change the look of an entire website by changing just one file!

Each HTML page must include a reference to the external style sheet file inside the <link> element, inside the head section.

~~~
<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="mystyle.css">
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
~~~
**Internal CSS:**

An internal style sheet may be used if one single HTML page has a unique style.

The internal style is defined inside the <style> element, inside the head section.

~~~
<!DOCTYPE html>
<html>
<head>
<style>
body {
  background-color: linen;
}

h1 {
  color: maroon;
  margin-left: 40px;
}
</style>
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
~~~

**Inline CSS:**

An inline style may be used to apply a unique style for a single element.

To use inline styles, add the style attribute to the relevant element. The style attribute can contain any CSS property.

~~~
<!DOCTYPE html>
<html>
<body>

<h1 style="color:blue;text-align:center;">This is a heading</h1>
<p style="color:red;">This is a paragraph.</p>

</body>
</html
~~~
#### CSS color Property:

~~~
body {
  color: red;
}

h1 {
  color: #00ff00;
}

p.ex {
  color: rgb(0,0,255);
}
# Q.1. Explain the difference between inline, internal, and external CSS.

### Ans:-

#### 1.Inline CSS:-

- Inline CSS is applied directly to an HTML element using the style attribute like....

```javascript
<div style="color:pink"></div>
```

#### 2.Internal CSS:-

- Internal CSS is defined within a <style></style> tag element in the HTML document like into the style tag into the header part like....

```javascript
<style>color:pink;</style>
```

#### 3.External CSS:-

- External CSS is defined in new CSS file which is linked with HTML file like....

```javascript
<link rel="stylesheet" href="style.css">

.CSS file which is a separate file of CSS which is linked with HTML file.
```

# Q.2. Describe CSS selectors and list the types of selectors (e.g., element, class, id).

### Ans:-

- A CSS selector is the first part of a CSS Rule.
- In CSS, selectors are used to target the HTML elements on our web pages that we want to style.
- There are a wide variety of CSS selectors available like as given below.

----------CSS selector----------

-Five types of Selectors in CSS...

1. Simple selector
2. Combinator selector
3. Attribute selector
4. Pseudo-class selector
5. Pseudo-element selector

1)) Simple selector:-

- Simple selector are five types:

1. Element selector
2. I'd selector
3. Class selector
4. Universal selector
5. Grouping selector

2)) Combinator selector:-

- Combinator selector are four types:

1. Decendant selector
2. Child selector
3. Adjacent siblings selector
4. General sibling selector

[1] Element selector:-

Element selector is for element selection that contain multiple data element.

- syntax:-

Selector{ Property1: property-value; Property2: property2-value; PropertyN: propertyN-value;}

for ex.:-

```javascript
    p{color:red; font-size: 22px;}

    h1{color:blue; font-size:22em;}
```

[2] I'd selector:-

- The id selector uses the id attribute of an HTML element to select a specific element.
- The id of an element is unique within a page, so the id selector is used to select one unique element.
- To select an element with specific id,write a hash(#) character, followed by the id of the element.

```javascript
<html>
  <head>
<style>
#container{
background-color:lightblue;
width: 300px;
height: 400px;
}
</style>
</head>
    <body>
       <div id="container">
    </body>
</html>
```

[3] Class selector:-

- The class selector selects all elements that have the given class attribute denoted by the class name prefixed with a period(.).

```javascript
<html>
<head>
<style>
   .xyz{
    color:blue;
    background-color:brown;
}
</style>
</head>
<body>
    <h1 class="xyz">Class selector:-</h1>
    <p class="xyz">Paragraph One</p>
    <p>Paragraph two</p>
    <p class="xyz">Paragraph three</p>
</body>
```

[4] Universal selector:-

The universal selector is indicated by an asterisk(_). It selects everything in the document.
for example, p_ selects all the nested elements in the <p> element.

```javascript

  *{
    margin:0;
    padding:0;
}
```

[5] Grouping selector:-

- CSS Grouping selector is used to select multiple elements and style them togather.
- This reduces the code and extra effort to declare common styles for each element.
- To Group Selector, each selector is separated by a space.
- To Group selection we can select multiple elements with the use of semicolon(,) between them.

```javascript
<html>
  <head>
<style>
   h1,p{
   color:pink;
   background-color:blue;
}
</style>
</head>
  <body>
    <div>
      <h1>Types of css selectors:-</h1>
      <h2> Group selector</h2>
      <p>Paragraph One</p>
      <p>Paragraph Two</p>
      <p>Paragraph Three</p>
    </div>
  </body>
</html>
```

# Q.3. Discuss the CSS boxmodel and its components.

## Ans:-

The CSS box model as a whole applies to block boxes ans defines how the different parts of box- Margin,Border,Padding, and Content-work together to create a box that you can see on a page. Inline boxes use just some of the behavior defined in the box model.

To add Complexity,there is a Standard and an alternate box model. By default, browsers use the standard box model.

- Parts Of a Box:-

Making up a block box in CSS we have the:

[1] Content Box:-
[2] Padding Box:-
[3] Border Box:-
[4] Margin Box:-

To turn on the alternative model for an element, set BOx-sizing: border-box on it:
for example...,

```javascript

.box{
  box-sizing:border-box;
  width:350px;
  height:150px;
  margin:10px
  border:5px solid black;
}
```

## Standard Box Model:-

By default, the browsers use the Standard Box Model.
In the Standard box model, if you set width and height property values on a box,these values define the width and height of the content box. Any padding and borders are then added to those dimensions to get the total size taken up by the box.as shown above example.
for example..,

```javascript

.box{
  width:350px;
  height:150px;
  margin:10px
  border:5px solid black;
}
```

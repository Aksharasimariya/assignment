# Q.1. Define responsive design and its importance in modern web development.

## Ans:-

- Responsive Web Design comprises two words i.e., responsive and web design.
- Responsive means to respond and web design means to design website.
- Therefore, responsive web design generally means website that respond to or resize or adjust itself depending upon screen size it is being seen through.
- It automatically adjusts to fit user’s screen whether it’s desktop, laptop, mobile, tablet, etc.
- It only uses one layout for web page and it can be done either using CSS and HTML or CSS3 and HTML5.

### When to use it?

- Responsive web design is a way by which website that contain flexible layout that automatically scale its content and elements according to screen size on which it is viewed.
- -It simply resizes, shrink, enlarge, hide web pages so that it can look better on all type of devices and does not have to zoom and pan to see any content on website.
- But still some people get confused in deciding when to use responsive web design.

## Uses:-

- Responsive web design is best for small to large scale business or company.
- Responsive web design is best for small to large scale business or company.
- Responsive web design is best for service-based industries because it includes creative UX and UI design and is made up of images and text. Images and graphics are also clear and crisp when viewed on mobile device.
- Responsive web design is also best for companies that have less or tight budget and limited resources because responsive design is budget friendly.

# Q.2. Explain the role of media queries in responsive design.

### Ans:-

What Are CSS Media Queries?

- Contrary to popular belief, they go beyond responsive design.
- Media queries are basically a way to write conditional CSS. That means CSS markup that the browser will only render if certain conditions are met.
- Its most commonly use is in responsive design, where it’s a way to tell browsers to change the display of website elements when above or below a certain screen size. However, as see below, there are other ways you can use them.

How Do You Write a Media Query?

- In css we can write the condition of display with the help of "@media".
- All the condition and changes will be written after this "@media".
- for example.,

```javascript
@media [media-type] ([media-feature/condition/view screen size]) {
	// custom CSS
}

```

- In this the condition or vie screen size are also called a break point, meaning a point at which the design changes notably to accommodate a different screen size.
- for example.,

```javascript
 @media screen and (min-width: 320px) {
	// custom CSS
 }
```

- In above example the targets devices with screens above 320 pixels. Everything that’s placed inside curly brackets of the media query will only be output in the browser on devices with screens that meet that condition.
- In CSS media queries, you can also use operators like and, or, and not to combine conditions like so:

- for example.,

```javascript
@media screen and (min-width: 320px) and (max-width: 786px) {
	// custom CSS
}

```

- There’s also only, which makes a style apply only if the entire query matches.
- It is also often used to improve compatibility of media queries with older browsers.
- For example, an older browser might interpret @media screen and (min-width: 320px) as only @media screen and apply it in a wrong way.
- Including only as in @media only screen and (min-width: 320px), fixes this behavior while it does not affect modern browsers negatively.

Available Media Types:-

- While screen is the most common type of media to query, we have other options:

[1] all
[2] print
[3] speech

# Q.3. Describe how viewportsettings affect mobile displays.

### Ans:-

- What is viewport?

Viewport is the visible area of a web page that varies depending on the device and is smaller on a mobile phone than on a computer screen.

- How to Set Up the Viewport?

To set up the Viewport, add the following meta tag to the <head> section of your HTML document:

```javascript
<meta name="viewport" content="width=device-width, initial-scale=1.0">


```

- Before tablets and mobile phones, web pages were designed only for computer screens with a static design and a fixed size.
- When we started using the Internet on tablets and mobile phones, fixed-size web pages were too large to fit in the Viewport.
- To adjust this, the browsers on those devices reduced the size of the entire web page to fit on the screen.

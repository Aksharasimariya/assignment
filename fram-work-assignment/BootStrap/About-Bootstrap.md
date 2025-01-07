# Q.1. What is Bootstrap, and why is it useful for website design?

### Ans:-

Bootstrap is a powerful front-end framework designed to create responsive and mobile-first websites efficiently. It combines HTML, CSS, and JavaScript, offering a range of components and utilities to streamline web development.

Bootstrap is a free yet powerful front-end HTML, CSS, and JavaScript CSS framework. This open-source toolkit contains code dedicated to supporting the front-end web development process.

- Reasons Why You Should Use Bootstrap:-

1. Time-saving.
2. Easy to Use.
3. Responsive Grid System.
4. Customizable.
5. Cross-browser Compatible.
6. Maintain Consistency.
7. Open Source.
8. Community-centered.

# Q.2. Explain the Bootstrap grid system and how it helps create responsive layouts.

### Ans:-

Bootstrap Grid is a very powerful tool that makes developing websites easier. It is made with flexbox hence fully responsive and also adjusts the items in the container according to the device width. The container is a wrapping element that wraps all other items and content on the web page. CSS requires this wrapping element to make the grid work properly. The .container class is the class that we usually use while making use of bootstrap in our code as it also provides some additional options like setting the alignment to the centre and horizontally padding the content.

The bootstrap grid has 12 columns present it, although it is not necessary to make use of all the columns, the sum must not go beyond 12. They can also be merged to make wider columns as per the preference.

The .row and .col classes can be used to create and manipulate the rows and columns of the grid respectively.

On basis of the device or browser’s width, the bootstrap grid system has the following five classes:

#### For small devices:-

- col: It has the browser’s width of less than 576px.
- col-sm: It has the browser’s width equal to or greater than 576px.

#### For medium devices:-

- col-md: It has the browser’s width equal to or greater than 768px.

#### For large and extra-large devices

- col-lg: It has a screen width equal to or greater than 992px.
- col-xl: It has a screen width equal to or greater than 1200px

### Basic Structure:-

```javascript
<div class="container">
  <div class="row">
    <div class="col-lg">column-1</div>

    <div class="col-lg">Column-2</div>
  </div>
</div>
```

This will create 2 centre-aligned columns of equal widths. The class container wraps all the rows, columns, and content of the grid. The class row is used to create a row and the class col-lg denotes the device width is large.

#### Example:

Creating 3 equal columns of equal width.

```javascript
<html>

<head>
    <title>Three Equal columns</title>

    <link rel="stylesheet" href=
"https://maxcdn.bootstrapcdn.com/bootstrap/3.4.1/css/bootstrap.min.css">
</head>

<body>
    <h1 style="text-align: center; color: rgb(18, 171, 18);">
        GeeksforGeeks
    </h1>

    <div class="container">
        <div class="row" style="text-align: center;">
            <div class="col-lg-4 col-md-4 col-12" style=
                "background-color:#ffbe76; padding: 5px; height: 150px;">
                <h2>column-1</h2>
            </div>
            <div class="col-lg-4 col-md-4 col-12" style=
                "background-color:#34bcc4; padding: 5px; height: 150px;">
                <h2>column-2</h2>
            </div>
            <div class="col-lg-4 col-md-4 col-12" style=
                "background-color:#ff7979; padding: 5px; height: 150px;">
                <h2>column-3</h2>
            </div>
        </div>
    </div>
</body>
```

# Q.1. List and explain at least three Bootstrap components (e.g., navbar, cards, buttons).

### Ans:-

Bootstrap provides dozen of reusable components. They are built to provide dropdowns, buttons, icons, etc to our web pages. Bootstrap components are responsively built with base and modifier classes.

Base class and modifier class in Bootstrap components.

Let us look at some components of Bootstrap.

## [1] Navbar:-

Navbars allow users to quickly navigate the entire content of a product or a section of the application.

Responsive navbar built with the latest Bootstrap 5. Navbars allow users to quickly navigate the entire content of a product or a section of the application.

- Navbar example:-
  The navbar is a horizontal list of links when in the expanding state. It can include Dropdown, Button, Form, etc., if your need.

```javascript
<nav class="navbar navbar-expand-lg">
  <div class="container-fluid">
    <button
      class="navbar-toggler"
      type="button"
      data-bs-toggle="collapse"
      data-bs-target="#navbarExample"
      aria-controls="navbarExample"
      aria-expanded="false"
      aria-label="Toggle navigation"
    >
      <span class="navbar-toggler-icon"></span>
    </button>
    <a class="navbar-brand" href="#">
      <img src="/images/bootstrap-logo.svg" width="36" />
    </a>
    <div class="collapse navbar-collapse" id="navbarExample">
      <ul class="navbar-nav me-auto mb-0">
        <li class="nav-item">
          <a class="nav-link active" aria-current="page" href="#">
            Home
          </a>
        </li>
        <li class="nav-item">
          <a class="nav-link" aria-current="page" href="#">
            Team
          </a>
        </li>
        <li class="nav-item dropdown">
          <a
            class="nav-link dropdown-toggle"
            href="#"
            role="button"
            data-bs-toggle="dropdown"
            aria-expanded="false"
          >
            Projects
          </a>
          <ul class="dropdown-menu">
            <li>
              <a class="dropdown-item" href="#">
                Action
              </a>
            </li>
            <li>
              <a class="dropdown-item" href="#">
                Another action
              </a>
            </li>
            <li>
              <hr class="dropdown-divider" />
            </li>
            <li>
              <a class="dropdown-item" href="#">
                Something else here
              </a>
            </li>
          </ul>
        </li>
      </ul>
      <div class="d-flex align-items-center flex-column flex-lg-row">
        <form class="me-2 mb-2 mb-lg-0">
          <input
            type="text"
            class="form-control form-control-sm"
            placeholder="Search"
          />
        </form>
        <a class="btn btn-primary" href="">
          Sign up
        </a>
      </div>
    </div>
  </div>
</nav>
```

### How it works:-

Here’s what you need to know before getting started with the navbar:

- Navbars require a wrapping .navbar with .navbar-expand{-sm|-md|-lg|-xl|-xxl} for responsive collapsing and color scheme classes.
- Navbars and their contents are fluid by default. Change the container to limit their horizontal width in different ways.
- Use our spacing width, height and flex utility classes for controlling spacing and alignment within navbars.

## [2] Cards:-

Bootstrap Cards are versatile UI components used for organizing and presenting content within a webpage. Comprising key elements such as a container, header, body, footer, and optional image, these cards provide a structured and visually appealing way to showcase information.

- Card Container:-
  The outermost container with the class card serves as the foundation for the card element.

```javascript

<div class="card">
  <!-- Card content goes here -->
</div>
```

- Card Header:-
  The card-header class is used to define the header section of the card, typically containing a title or other relevant information.

```javascript

<div class="card-header">
  <!-- Header content goes here -->
</div>
```

- Card Body:-
  The card-body the class encapsulates the main content of the card, housing text, images, or any other elements.

```javascript

<div class="card-body">
  <!-- Main content goes here -->
</div>
```

- Card Footer:-
  The card-footer class represents the bottom section of the card, often utilized for additional information, buttons, or links.

```javascript

<div class="card-footer">
  <!-- Footer content goes here -->
</div>
```

- Card Image:-
  The card-img-top class can be used to insert an image at the top of the card.

```javascript

<img src="image.jpg" class="card-img-top" alt="Card Image">
```

- Button in Card:-
  Buttons can be added using the btn class and placing them inside the card structure.

```javascript
<a href="#" class="btn btn-primary">
  Learn More
</a>
```

### Features:-

- You can nest cards within other cards for complex layouts.
- Cards can be combined with other Bootstrap components like buttons, forms, and modals for enhanced functionality.
- Bootstrap offers pre-built card variations like "alert" and "list group" for specific use cases.

## [3] Buttons:-

Bootstrap provides a variety of button styles that can be used for different semantic purposes in your web projects. These buttons come with predefined styles that can be easily integrated into forms, dialogs, and more, offering support for multiple sizes and states.

- Basic Button Syntax:-

- To create a button in Bootstrap, you would typically use the

```javascript
 <button>
```

element with the class .btn followed by the style you want to apply.

````
- For example, to create a primary button, you would write:

```javascript
<button type="button" class="btn btn-primary">
Primary
</button>
````

#### Button Styles:-

Bootstrap includes several predefined button styles, each serving its own semantic purpose. Here are some examples:

[1] .btn-primary for primary buttons

[2].btn-secondary for secondary buttons

[3].btn-success for success actions

[4].btn-danger for dangerous actions

[5].btn-warning for warning messages

[6].btn-info for informational buttons

[7].btn-light and .btn-dark for light and dark variations

[8].btn-link for link buttons that resemble hyperlinks

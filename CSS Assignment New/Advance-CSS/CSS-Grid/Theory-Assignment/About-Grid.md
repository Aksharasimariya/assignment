# Q.1. WhatisCSSGrid, and howis it different from Flexbox?

### Ans:-

CSS Grid arranges items in rows and columns (2-Dimension), while Flexbox aligns items in a single row or column (1-Dimension).

CSS Grid Layout, is a two-dimensional grid-based layout system with rows and columns. It makes easier to design web pages without having to use floats and positioning.

- CSS Grid Layout:-

CSS Grid Layout, is a two-dimensional grid-based layout system with rows and columns. It makes easier to design web pages without having to use floats and positioning. Like tables, grid layout allow us to align elements into columns and rows.

To get started, you have to define a container element as a grid with display: grid, set the column and row sizes with grid-template-columns and grid-template-rows, and then place its child elements into the grid with grid-column and grid-row.

```javascript
<!DOCTYPE html>
<html lang="en">

<head>
    <style>
        .main{
            display: grid;
            grid: auto auto / auto auto auto auto;
            grid-gap: 10px;
            background-color: green;
            padding: 10px;
        }
        .gfg {
            background-color: rgb(255, 255, 255);
            text-align: center;
            padding: 25px 0;
            font-size: 30px;
        }
    </style>
</head>

<body>
    <h2 style="text-align: center;">
          Welcome To GeeksForGeeks
      </h2>
    <div class="main">
        <div class="gfg">Home</div>
        <div class="gfg">Read</div>
        <div class="gfg">Write</div>
        <div class="gfg">About Us</div>
        <div class="gfg">Contact Us</div>
        <div class="gfg">Privacy Policy</div>
    </div>
</body>

</html>
```

## Difference Between CSS Grid and Flexbox:-

| Property         | Grid                                                           | Flexbox                                       |
| ---------------- | -------------------------------------------------------------- | --------------------------------------------- |
| Dimension        | Two – Dimensional                                              | One – Dimensional                             |
| ---------        | -----------------                                              | ------------------                            |
| Features         | Can flex combination of items through space-occupying Features | Can push content element to extreme alignment |
| ---------        | -----------------------                                        | --------------                                |
| Support Type     | Layout First                                                   | Content First                                 |
| ------------     | -------------                                                  | ------------                                  |
| Primary Use Case | Creating complex layouts with rows and columns                 | Aligning items in a row or column             |
| ---------------  | --------------------                                           | -------------                                 |
| Performance      | Can be less in performance due to very complex grids           | Generally faster for simple layouts           |
| ------------     | ---------------------                                          | ------------                                  |

# Q.2. Describe the CSS Grid properties grid-template-columns and grid-template-rows.

### Ans:-

### [1] grid-template-columns:-

The grid-template-columns property defines the number and size of columns in a grid container. This property accepts various types of values to create different column layouts.

- Syntax:-

```javascript

 grid-template-columns: <track-size> [ <track-size> ];
```

- Track Sizes:-
  Length Values (e.g., px, em, rem): Specifies fixed sizes for columns.

- Percentage:-
  Specifies the size relative to the grid container's width.
- Fractional Units (fr):-
  Represents a fraction of the available space in the grid container.
- Auto:-
  The size of the column adjusts automatically based on its content.
- Minmax():-
  Allows specifying a minimum and maximum size for columns.
- Repeat():- Simplifies the definition of repeated column sizes.

#### Examples:-

1. Fixed Sizes:-

```javascript
.container {
  display: grid;
  grid-template-columns: 100px 200px 300px;
}
```

2. Fractional Units:-

```javascript
.container {
  display: grid;
  grid-template-columns: 1fr 2fr 1fr;
}
```

3. Minmax():-

```javascript
.container {
  display: grid;
  grid-template-columns: repeat(3, minmax(100px, 1fr));
}
```

4. Repeat():-

```javascript
.container {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
}
```

### [2] grid-template-rows:-

The grid-template-rows property works similarly to grid-template-columns but for rows. It defines the number and size of rows in a grid container.

- Syntax:-

```javascript

 grid-template-rows: <track-size> [ <track-size> ];
```

- Track Sizes:-
- Length Values:-
  Specifies fixed heights for rows.
- Percentage:-
  Specifies the height relative to the grid container's height.
- Fractional Units (fr):-
- Represents a fraction of the available space in the grid container.
- Auto:- The height of the row adjusts automatically based on its content.
- Minmax():- Allows specifying a minimum and maximum height for rows.
- Repeat():- Simplifies the definition of repeated row sizes.

#### Examples:-

1. Fixed Sizes:-

```javascript

.container {
  display: grid;
  grid-template-rows: 50px 100px 150px;
}
```

2. Fractional Units:-

```javascript

.container {
  display: grid;
  grid-template-rows: 2fr 1fr 1fr;
}
```

3. Minmax():-

```javascript
.container {
  display: grid;
  grid-template-rows: repeat(3, minmax(50px, 1fr));
}
```

4. Repeat():-

```javascript
.container {
  display: grid;
  grid-template-rows: repeat(4, 100px);
}
```

# Q.3. Explain the purpose of grid-area and how it is used to create complex layouts.

### Ans:-

The grid-area property specifies a grid item’s size and location in a grid layout. It allows you to define the starting and ending row and column lines for an item, or to assign a name to the item for easy reference in grid templates.

- Syntax:-

```javascript

grid-area: grid-row-start | grid-column-start |
           grid-row-end | grid-column-end | itemname;
```

#### Property Values:-

| Property Value    | Description                                                                  |
| ----------------- | ---------------------------------------------------------------------------- |
| grid-row-start    | It sets the row on which the item is displayed first.                        |
| ----------------  | -----------                                                                  |
| grid-column-start | It sets the column on which the item is displayed first.                     |
| ----------------- | ------------                                                                 |
| grid-row-end      | It specifies the row line to stop displaying the item or span how many rows. |
| ----------------- | -------------                                                                |
| grid-column-end   | It sets the number of columns to span.                                       |
| itemname          | It sets a name for the grid item.                                            |

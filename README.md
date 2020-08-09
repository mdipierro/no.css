# no.css

Minimalistic CSS library sesigned to style pages without need for custom classes. 
headers, paragraphs, buttons, tables, forms, nav menus are styled automatically.
Hence the name NO CSS.

The library does define some anyway, for the following purpose:

```
Grid classes:
  row, col, c25, c33, c50, c66, c75
Colors classes:
  black, white, normal, success, warning, failure, info, transparent
Effect classes:
  accordion, modal
Other classes:
  full, padded, error, close
```

## Page structure

no.css assumes the following page structure

<html>
  <head>
    <link rel="stylesheet" type="text/css" href="no.css">
  </head>
  <body>
    <nav class="black">...</nav>
    <div class="notification">...optional message...</div>
    <div class="row">
      <div class="c75">...main...</div>
      <div class="c25">...sidebar...</div>
    </div>
    <footer>
      ...
    </footer>
  </body>
</html>
```

## The nav block

The nav block assumes a logo or link, and two menus implemented as unordered lists: a left menu and a right menu:

```
<nav>
  <a>LOGO HERE</a>
  <!-- first UL is left menu -->
  <ul>
    <li><a>Link1</a></li>
    <li><a>Link2</a></li>
    <li><a>Link3</a>
      <!-- optional sub menu -->
      <ul>
        <li><a>Link4</a></li>
        <li><a>Link5</a></li>
      </ul>
    </li>
  </ul>
  <!-- second ul is right menu -->
  <ul>
    <li><a>Link6</a>
      <ul>
        <li><a>Link7</a></li>
        <li><a>Link8</a></li>
      </ul>
    </li>
  </ul>
</nav>
```

If the screen widths is less than 600px, the yop level menu items may de displayed vertically.

## Grid

The structure of a grid is the following:

<div class="row">
   <div class="c75">
     ...
   </div>
   <div class="c25">
     ...
   </div>
</div>

This indicates a 75% column and a 25% column. Only predefined column widths are:

- c25 (25%)
- c33 (33%)
- c50 (50%)
- c66 (66%)
- c75 (75%)

Rows can be nested.

If the screen width is less than 600px the columns are displayed as rows.

## Tables

Tables are styled automatically.

## Form

Forms elements are styled automatically.

## Colors

Supported colors are:

- black
- white
- default (blue)
- success (green)
- warning (yellow)
- error (red)
- info (gray)
- transparent

The above classes set the background color of the element they are applied to. They also set the background color to white or black, depending of what is more appropriate.

## Accordion

(UNDOCUMENTED)

## Modal

(UNDOCUMENTED)

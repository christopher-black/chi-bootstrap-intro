# Chi Bootstrap Intro
## What is Bootstrap?

HTML, CSS, and JS framework for developing responsive, mobile first projects on the web.

[Download Bootstrap](http://getbootstrap.com/getting-started/)

## Why Bootstrap?

- Makes developing websites faster
- Responsive
- Components look better

Frameworks decrease overall development time at the cost of looking more 'cookie cutter'. Many clients don't have the budget to build everything from scratch. Bootstrap helps with that.

## Setup

- Download the zip file with [Bootstrap](http://getbootstrap.com/getting-started/)
- Extract zip file
- Copy contents into your vendors folder

```
vendors/
├── css/
│   ├── bootstrap.css
│   ├── bootstrap.css.map
│   ├── bootstrap.min.css
│   ├── bootstrap.min.css.map
│   ├── bootstrap-theme.css
│   ├── bootstrap-theme.css.map
│   ├── bootstrap-theme.min.css
│   └── bootstrap-theme.min.css.map
├── js/
│   ├── bootstrap.js
│   └── bootstrap.min.js
└── fonts/
    ├── glyphicons-halflings-regular.eot
    ├── glyphicons-halflings-regular.svg
    ├── glyphicons-halflings-regular.ttf
    ├── glyphicons-halflings-regular.woff
    └── glyphicons-halflings-regular.woff2
```

- Add jQuery to your vendors folder (required for Bootstrap)

**HTML**
```HTML
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <!-- The above 3 meta tags *must* come first in the head; any other head content must come *after* these tags -->
    <title>Chi Bootstrap Intro</title>

    <!-- Bootstrap -->
    <link href="vendors/css/bootstrap.min.css" rel="stylesheet">

    <!-- Custom styles -->
    <link href="style.css" rel="stylesheet">

    <!-- jQuery (necessary for Bootstrap's JavaScript plugins) -->
    <script src="vendors/jquery.js"></script>
  </head>
  <body>
    <h1>Hello, world!</h1>

    <!-- Include all compiled plugins (below), or include individual files as needed -->
    <script src="vendors/js/bootstrap.min.js"></script>
  </body>
</html>
```

> Additional resources can be found [here](http://getbootstrap.com/css/)

## Containers

Use `.container` for a responsive fixed width container.

```HTML
<div class="container">
  ...
</div>
```

Use `.container-fluid` for a full width container, spanning the entire width of your viewport.

```HTML
<div class="container-fluid">
  ...
</div>
```

## Rows & Columns

Columns must be nested within rows. Columns must add up to 12.

```HTML
<div class="container">
  <div class="row">
    <div class="col-md-8">.col-md-8</div>
    <div class="col-md-4">.col-md-4</div>
  </div>
  <div class="row">
    <div class="col-md-4">.col-md-4</div>
    <div class="col-md-4">.col-md-4</div>
    <div class="col-md-4">.col-md-4</div>
  </div>
  <div class="row">
    <div class="col-md-6">.col-md-6</div>
    <div class="col-md-6">.col-md-6</div>
  </div>
</div>
```

## Tables
```HTML
<div class="container">
  <table class="table">
    ...
  </table>
</div>
```

## Forms
```HTML
<form>
  <div class="form-group">
    <label for="exampleInputEmail1">Email address</label>
    <input type="email" class="form-control" id="exampleInputEmail1" placeholder="Email">
  </div>
  <div class="form-group">
    <label for="exampleInputPassword1">Password</label>
    <input type="password" class="form-control" id="exampleInputPassword1" placeholder="Password">
  </div>
  <button type="submit" class="btn btn-default">Submit</button>
</form>
```

## Buttons
```HTML
<!-- Standard button -->
<button type="button" class="btn btn-default">Default</button>

<!-- Provides extra visual weight and identifies the primary action in a set of buttons -->
<button type="button" class="btn btn-primary">Primary</button>

<!-- Indicates a successful or positive action -->
<button type="button" class="btn btn-success">Success</button>

<!-- Contextual button for informational alert messages -->
<button type="button" class="btn btn-info">Info</button>

<!-- Indicates caution should be taken with this action -->
<button type="button" class="btn btn-warning">Warning</button>

<!-- Indicates a dangerous or potentially negative action -->
<button type="button" class="btn btn-danger">Danger</button>

<!-- Deemphasize a button by making it look like a link while maintaining button behavior -->
<button type="button" class="btn btn-link">Link</button>
```

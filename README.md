jQuery Steps Plugin [![Build Status](https://secure.travis-ci.org/rstaib/jquery-steps.png)](http://travis-ci.org/rstaib/jquery-steps)
============

A powerful jQuery wizard plugin that supports accessibility and HTML5.

## Getting Started

jQuery Steps is a lightweight wizard UI component written for jQuery.

Everything you need to start is:

1. Include *jQuery* and *jQuery Steps* in your HTML code.
2. Then select an element represents the wizard and call the `steps` method.

```html
<!DOCTYPE html>
<html>
    <head>
        <title>Demo</title>
        <meta charset="utf-8">
        <script src="jquery.js"></script> 
        <script src="jquery.steps.js"></script>
    </head>
    <body>
        <script>
            $("#wizard").steps();
        </script>
        <div id="wizard"></div>
    </body>
</html>
```

### How to add initial steps?

There are two ways to add steps and their corresponding content.

1. Add HTML code into the representing wizard element.

```html
<div id="wizard">
    <h1>First Step</h1>
    <div>First Content</div>

    <h1>Second Step</h1>
    <div>Second Content</div>
</div>
```

2. Or use the API to add steps dynamically.

```javascript
// Initialize wizard
var wizard = $("#wizard").steps();

// Add step
wizard.steps("add", {
    title: "HTML code", 
    content: "<strong>HTML code</strong>"
});
```

## License

Copyright (c) 2013 Rafael J. Staib Licensed under the [MIT license](https://github.com/rstaib/jquery-steps/blob/master/LICENSE.txt).
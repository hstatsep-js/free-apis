# Free APIs

This repo makes use of https://github.com/public-apis/public-apis

And its public API: https://api.publicapis.org/

The full list JSON list is at https://api.publicapis.org/entries

Filtered by _no auth_: https://api.publicapis.org/entries?auth=null

# Required code

There are two pieces in the starter code that are required to get the JSON data:

```html
<!-- This jQuery script allows us to easily use $.ajax() -->
<script src="https://code.jquery.com/jquery-3.5.1.min.js" integrity="sha256-9/aliU8dGd2tb6OSsuzixeV4y/faTqgFtohetphbbj0=" crossorigin="anonymous"></script>
```

and

```js
$.ajax({
    url: 'https://api.publicapis.org/entries',
    dataType: 'json',
    success: function(data) {
        console.log(data);
    }
});
```

# Usage

1. Copy the template: `cp template.html newName.html`
2. Simply replace the `url` value with your own URL.  
3. Change `console.log(data)` to whatever you want!
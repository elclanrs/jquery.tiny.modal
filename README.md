# jQuery Tiny Modal

Barebones modal dialogs.

## How to

Create a container with an ID for your modal dialog, then put any markup you want inside.

```html
<div id="mymodal">
  <h2>My Modal</h2>
  <p>Lorem ipsum dolor sit amet consectetur</p>
</div>
```

Trigger your modal on some element, like a button for example and call the plugin:

```javascript
$('button').click(function(){
  $.tinyModal({
    title: 'My Modal',
    html: '#mymodal'
  });
});
```

Tiny Modal comes with a basic theme that you can configure in `styl/jquery.tinymodal.styl`. Make sure to run `npm install` to download the dependencies. After editing don't forget to watch your files for changes and compile with `sh compile.sh`.

## Options

```javascript
_defaults = {
  buttons: ['Ok','Cancel'],
  title: 'Alert',
  html: '<p>Alert</p>', // markup or selector
  Ok: $.noop, // callback for the "Ok" button
  Cancel: $.noop, // callback for the "Cancel" button
  onClose: $.noop, // callback after the dialog closes
  clickOutside: true // close the dialog when clicking outside
};
```

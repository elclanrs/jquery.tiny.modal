# jQuery Tiny Modal

Barebones modeal dialogs.

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

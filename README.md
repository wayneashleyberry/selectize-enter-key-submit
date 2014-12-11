## Selectize Enter Key Submit

[![devDependency Status](https://david-dm.org/wayneashleyberry/selectize-enter-key-submit/dev-status.svg)](https://david-dm.org/wayneashleyberry/selectize-enter-key-submit#info=devDependencies)

This is a little [Selectize](https://github.com/brianreavis/selectize.js)
plugin that will allow you to submit the form when a user hits the enter key.
The plugin triggers a `submit` event which you can listen to and handle how you
will. The event will only be triggered if the input is empty.

Here's a quick example:

```js
$('input').selectize({
  // load the plugin
  plugins: ['enter_key_submit'],
  // listen to submit events
  onInitialize: function (foo) {
    this.on('submit', function () {
      this.$input.closest('form').submit();
    }, this);
  }
});
```

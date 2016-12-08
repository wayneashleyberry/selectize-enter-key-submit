## Selectize Enter Key Submit

> Submit [Selectize](https://github.com/brianreavis/selectize.js) forms using the enter key.

[![Build Status](https://img.shields.io/travis/wayneashleyberry/selectize-enter-key-submit/master.svg?style=flat)](https://travis-ci.org/wayneashleyberry/selectize-enter-key-submit)
[![npm](http://img.shields.io/npm/v/selectize-enter-key-submit.svg?style=flat)](https://www.npmjs.com/package/selectize-enter-key-submit)

This plugin will allow you to submit Selectize forms with the enter key.  The
plugin triggers a `submit` event which you can listen to and handle how you
will. The event will only be triggered if the input is empty.

#### Usage

```js
$('input').selectize({

  // load the plugin
  plugins: ['enter_key_submit'],

  // listen to submit events
  onInitialize: function (foo) {
    this.on('submit', function () {
      this.$input.closest('form').submit()
    }, this)
  }

})
```

#### License

[MIT](https://github.com/wayneashleyberry/selectize-enter-key-submit/blob/master/license) © [Wayne Ashley
Berry](https://wayne.cloud)

### `insertdatetime_timeformat`

This option allows you to override the default formatting rule for times inserted by the `mceInsertTime` command. This defaults to `%H:%M:%S` and where the different `%` variables get replaced with various [date format options](#referencedatetimeformats).

#### Example: Using `insertdatetime_timeformat`

```js
tinymce.init({
  selector: 'textarea',  // change this value according to your HTML
  plugins: 'insertdatetime',
  menubar: 'insert',
  toolbar: 'insertdatetime',
  insertdatetime_timeformat: '%H:%M:%S'
});
```

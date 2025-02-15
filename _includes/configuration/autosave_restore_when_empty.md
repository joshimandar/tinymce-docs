### `autosave_restore_when_empty`

This option enables you to specify if {{site.productname}} should automatically restore the content stored in local storage when the editor is empty on initialization. This can be useful for users who don't know that they can restore lost work if the browser crashed by selecting `Restore last draft` from the `File` menu.

**Type**: `Boolean`

**Default Value**: `false`

**Possible Values**: `true`, `false`

#### Example: Using `autosave_restore_when_empty`

```js
tinymce.init({
  selector: 'textarea',  // change this value according to your HTML
  plugins: 'autosave',
  autosave_restore_when_empty: true
});
```

### `table_tab_navigation`

This option enables you to disable the default tab between table cells feature. By default, when a user presses tab the cursor will move between cells within the table. By setting the `table_tab_navigation` value to `false` the cursor will tab between browser elements (such as the URL bar or form fields, etc).

**Type:** `Boolean`

**Default Value:** `true`

**Possible Values:** `true`, `false`

#### Example: Using `table_tab_navigation`

```js
tinymce.init({
  selector: 'textarea',  // change this value according to your HTML
  plugins: 'table',
  menubar: 'table',
  toolbar: 'table',
  table_tab_navigation: false
});
```

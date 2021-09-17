### `table_appearance_options`

This option allows you to disable some of the options available to a user when inserting or editing a table. When set to `false` the following fields will not appear: Cell spacing, Cell padding, Border and Caption.

**Type:** `Boolean`

**Default Value:** `true`

**Possible Values:**  `true`, `false`

#### Example: Using `table_appearance_options`

```js
tinymce.init({
  selector: 'textarea',  // change this value according to your HTML
  plugins: 'table',
  table_appearance_options: false
});
```

### `table_grid`

This option allows you to disable the grid-like table picker in the Table menu. The grid feature (which is enabled by default) consists of a dragable matrix that a user can interact with to automatically create a table of x-rows by x-columns based upon their input.

However, if `table_grid` is set to `false` the table picker will be replaced by a menu item that opens a dialog that users can use to insert a table. This dialog allows users to set various parameters such as the number of columns and rows, width, height, cell spacing and padding, border width, alignment, and whether to display a caption. There are also advanced style options available if `table_advtab` is set to `true`.

> **Note**: To configure the Table menu to include both the table picker and the table dialog menu items, set `table_grid` to `true` and configure [`menu`]({{ site.baseurl}}/configure/editor-appearance/#menu) to include both the `inserttable` and `inserttabledialog` menu items.

**Type:** `Boolean`

**Default Value:** `true`

**Possible Values:**  `true`, `false`

{{site.differs_for_mobile}}

#### Example: Using `table_grid`

```js
tinymce.init({
  selector: 'textarea',  // change this value according to your HTML
  plugins: 'table',
  menubar: 'table',
  toolbar: 'table',
  table_grid: false
});
```


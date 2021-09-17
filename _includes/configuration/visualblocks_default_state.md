### `visualblocks_default_state`

This option enables you to specify the default state of the Visual Blocks plugin.

**Type:** `Boolean`

**Default Value:** `false`

**Possible Values:** `true`, `false`

#### Example: Using `visualblocks_default_state`

```js
tinymce.init({
  selector: 'textarea',  // change this value according to your HTML
  plugins: 'visualblocks',
  menubar: 'view',
  toolbar: 'visualblocks',
  visualblocks_default_state: true
});
```
### `image_dimensions`

This options allows you disable the image dimensions input field in the image dialog.

**Type:** `Boolean`

**Default Value:** `true`

**Possible Values:** `true`, `false`

#### Example: Using `image_dimensions`

```js
tinymce.init({
  selector: 'textarea',  // change this value according to your HTML
  plugins: 'image',
  menubar: 'insert',
  toolbar: 'image',
  image_dimensions: false
});
```


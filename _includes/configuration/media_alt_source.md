### `media_alt_source`

This options allows you disable the `Alternative source` input field in the media dialog.

**Type:** `Boolean`

**Default Value:** `true`

**Possible Values:** `true`, `false`

#### Example: Using `media_alt_source`

```js
tinymce.init({
  selector: 'textarea',  // change this value according to your HTML
  plugins: 'media',
  menubar: 'insert',
  toolbar: 'media',
  media_alt_source: false
});
```


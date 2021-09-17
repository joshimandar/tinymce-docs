### `image_prepend_url`

This option allows you to specify a URL prefix that will be applied to images when appropriate.

**Type:** `String`

#### Example: Using `image_prepend_url`

```js
tinymce.init({
  selector: 'textarea',  // change this value according to your HTML
  plugins: 'image',
  menubar: 'insert',
  toolbar: 'image',
  image_prepend_url: 'https://www.example.com/images/'
});
```

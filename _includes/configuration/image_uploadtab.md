### `image_uploadtab`

This option adds an "Upload" tab to the image dialog allowing you to upload local images, when the [`images_upload_url`]({{site.baseurl}}/configure/file-image-upload/#images_upload_url) is also configured.

**Type:** `Boolean`

**Default Value:** `true`

**Possible Values:** `true`, `false`

#### Example: Using `image_uploadtab`

```js
tinymce.init({
  selector: 'textarea',  // change this value according to your HTML
  plugins: 'image',
  menubar: 'insert',
  toolbar: 'image',
  image_uploadtab: false
});
```


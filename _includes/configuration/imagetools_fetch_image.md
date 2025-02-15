### `imagetools_fetch_image`

This option can be used to define a custom fetch function, which provides another way to access images in complex situations. The function will be passed the HTML element of the image to be fetched and should return a `Promise` containing a `Blob` representation of the image.

**Type:** `Function`

#### Example: Using `imagetools_fetch_image`

```js
tinymce.init({
  selector: 'textarea',  // change this value according to your HTML
  toolbar: 'image',
  plugins: 'image imagetools',
  imagetools_fetch_image: function (img) {
    return new tinymce.util.Promise(function (resolve) {
      // Fetch the image and return a blob containing the image content
      ...
      resolve(new Blob(...));
    });
  }
});
```


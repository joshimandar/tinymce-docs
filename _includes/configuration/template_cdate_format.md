### `template_cdate_format`

This option allows you to provide a date format that all 'creation' date templates will use.

**Type:** `String`

**Default:** `'%Y-%m-%d'`

#### Example: Using `template_cdate_format`

```js
tinymce.init({
  selector: 'textarea',  // change this value according to your HTML
  plugins: 'template',
  menubar: 'insert',
  toolbar: 'template',
  template_cdate_format: '%m/%d/%Y : %H:%M',
  templates: [
    {title: 'Cdate', description: 'Cdate example', content: '<p class="cdate">This will be replaced with the creation date</p>'}
  ]
});
```

If the creation date is set as 9:00AM on January 15th 2000, then inserting this template will insert the following into the editor:

```html
<p class="cdate">01/15/2000 : 09:00</p>
```

For a list of available date and time formats, see: [Reference Date/Time formats](#referencedatetimeformats).


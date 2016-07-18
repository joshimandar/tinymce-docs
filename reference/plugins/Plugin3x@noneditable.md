---
layout: default
title: noneditable
---

Adds non editable elements support for MSIE and Mozilla/FF. Any element with the "mceNonEditable" class will be blocked from modifications and treated as a single character. This class name is configurable using the "noneditable_noneditable_class". Any elements with the MSIE specific attribute "contenteditable" will be converted into classes instead.

## Initialization Example

```html
tinyMCE.init({
	theme : "advanced",
	mode : "textareas",
	plugins : "noneditable",
	noneditable_leave_contenteditable : true
});

```

HTML contents example:

When you have existing classes that cannot be removed, you may combine MCE classes with the existing class in the following manner:

Non editable div example:

```html
<div class="myclass mceNonEditable">Contents</div>

```

Editable div example:

```html
<div class="myclass mceEditable">Contents</div>

```

Nested editable elements are not currently supported. You would not be able to edit the cell contents in the following table:

```html
<table class="mceNonEditable">
<tr>
<td class="mceEditable">
Contents
</td>
</tr>
</table>

```

## Plugin options

| Name | Summary |
| --- | --- |
| [noneditable_editable_class] | Class name to be used for editable elements, this would be the the same as contenteditable=true, forcing a element to be editable. This option defaults to: "mceEditable". Notice that classes with the mceItem prefix is invisible within TinyMCE. |
| [noneditable_noneditable_class] | Class name to be used for non editable elements, this would be the same as contenteditable=false. This option defaults to: "mceNonEditable". Notice that classes with the mceItem prefix is invisible within TinyMCE. |
| [noneditable_leave_contenteditable] | If the value of this option is set to true, all contenteditable attributes will be left intact. This option is set to false by default, since this attribute is not a valid W3C attribute and the class approach is better. |
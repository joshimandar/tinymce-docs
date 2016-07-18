---
layout: default
title: table
---

This plugin adds table management functionality to TinyMCE.

## Table controls/buttons

| Name | Summary |
| --- | --- |
| tablecontrols | All table control below and some separators between them. |
| table | Insert table control. |
| row_props | Edit row properties (tr). |
| cell_props | Edit cell properties (td). |
| delete_col | Delete column control. |
| delete_row | Delete row control. |
| delete_table | Delete table control. |
| col_after | Column after control. |
| col_before | Column before control. |
| row_after | Row after control. |
| row_before | Row before control. |
| split_cells | Splits a merged cell into rows and columns. |
| merge_cells | Mergers selected cells into one cell. |

## Table commands to use with execCommand

| Name | Summary |
| --- | --- |
| mceInsertTable | Inserts a new table at cursor location the default size is 2x2\. If the value parameter is specified it should contain a name/value array, this array has the following options cols, rows, border, cellspacing, cellpadding. The default border is set to: 0. |
| mceTableInsertRowBefore | Inserts a row before/above the current cursor location. |
| mceTableInsertRowAfter | Inserts a row after/under the current cursor location. |
| mceTableDeleteRow | Deletes the row at the current cursor location. |
| mceTableInsertColBefore | Inserts a column before the current cursor location. |
| mceTableInsertColAfter | Inserts a column after the current cursor location. |
| mceTableDeleteCol | Deletes the column at the current cursor location. |
| mceTableDelete | Deletes the table at the current cursor location. |

## Plugin options

| Name | Summary |
| --- | --- |
| table_styles | This option should contain a semicolon separated list of class titles and class names separated by =. The titles are the ones that get presented to the user in the styles drop down list and and the class names is the classes that gets inserted. |
| table_cell_styles | This option should contain a semicolon separated list of class titles and class names separated by =. The titles are the ones that get presented to the user in the styles drop down list and and the class names is the classes that gets inserted. |
| table_row_styles | This option should contain a semicolon separated list of class titles and class names separated by =. The titles are the ones that get presented to the user in the styles drop down list and and the class names is the classes that gets inserted. |
| table_cell_limit | Enables you to specify the max number of cells for a table. |
| table_row_limit | Enables you to specify the max number of rows for a table. |
| table_col_limit | Enables you to specify the max number of columns for a table. |
| table_default_border | Enables you to specify the default border value. |
| table_default_cellpadding | Enables you to specify the default cellpadding value. |
| table_default_cellspacing | Enables you to specify the default cellspacing value. |

## Installation Instructions

1.  Add plugin to TinyMCE plugin option list example: plugins : "table".
2.  Add the table button names to button list, example: theme_advanced_buttons3_add : "tablecontrols".

## Initialization Example

```html
tinyMCE.init({
	theme : "advanced",
	mode : "textareas",
	plugins : "table",
	theme_advanced_buttons3_add : "tablecontrols",
	table_styles : "Header 1=header1;Header 2=header2;Header 3=header3",
	table_cell_styles : "Header 1=header1;Header 2=header2;Header 3=header3;Table Cell=tableCel1",
	table_row_styles : "Header 1=header1;Header 2=header2;Header 3=header3;Table Row=tableRow1",
	table_cell_limit : 100,
	table_row_limit : 5,
	table_col_limit : 5
});

```
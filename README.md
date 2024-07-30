# termprint

[![PyPI - Version](https://img.shields.io/pypi/v/termprint.svg)](https://pypi.org/project/termprint)
[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/termprint.svg)](https://pypi.org/project/termprint)

-----

**Table of Contents**

- [termprint](#termprint)
  - [Installation](#installation)
  - [License](#license)

## Installation

```console
pipx install termprint
```

## License

`termprint` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.


## Functions Documentation

### `set_color_scheme`

Set the color scheme for printing. Options are: 'truecolor', '256colors', 'basic', 'mono'.


**Args:**

 - **scheme (str)**:  The name of the color scheme to set. If the scheme is not found, it defaults to 'basic' 


### `error`

Print an error message in the color defined by the current color scheme.


**Args:**

 - **msg (str)**:  The error message to print 


### `warning`

Print a warning message in the color defined by the current color scheme.


**Args:**

 - **msg (str)**:  The warning message to print 


### `info`

Print an informational message in the color defined by the current color scheme.


**Args:**

 - **info (str)**:  The main informational message to print. 
 - **msg (str, optional)**:  An additional message to print in a different color 


### `line`

Print a line of a specified length and character in the color defined by the current color scheme.


**Args:**

 - **length (int, optional)**:  The length of the line. Defaults to 80. 
 - **char (str, optional)**:  The character to use for the line. Defaults to '─' 


### `title`

Print a title message in the color defined by the current color scheme.


**Args:**

 - **msg (str)**:  The title message to print. 
 - **length (int, optional)**:  The length of the title line. Defaults to 80. 
 - **line (bool, optional)**:  Whether to print a line under the title. Defaults to True. 
 - **char (str, optional)**:  The character to use for the line. Defaults to '─' 


### `bullet_list`

Print a bullet list of items in the color defined by the current color scheme.


**Args:**

 - **items (list)**:  A list of items to print as a bullet list. 
 - **title (str, optional)**:  The title of the bullet list. Defaults to Non 


### `dict2tree`

Convert a dictionary to a tree structure.


**Args:**

 - **data (dict)**:  The dictionary to convert to a tree. 
 - **tree (rTree)**:  The tree object to add the dictionary to. 
 - **level (int, optional)**:  The level of the tree. Defaults to 1. 
 - **title (str, optional)**:  The title of the tree. Defaults to "Tree" 


### `tree`

Print a tree representation of a nested dictionary.


**Args:**

 - **data_dict (dict)**:  The nested dictionary to be represented as a tree. 
 - **title (str, optional)**:  The title of the tree. If not provided, the title will be the key of the single item in the dictionary, 
 - **or 'root' if the dictionary has multiple items.** 

**Returns:**
 - Non


### `print_tree`

Print a tree representation of a nested dictionary with a specified root name.


**Args:**

 - **tree (dict)**:  The nested dictionary to be represented as a tree. 
 - **name (str, optional)**:  The name of the root of the tree. Defaults to 'root'. 

**Returns:**
 - Non


### `table`

Prints a table with the given columns and lists.


**Args:**

 - **columns (list)**:  A list of column names. 
 - **lists (list)**:  A list of lists representing the rows of the table. 
 - **title (str, optional)**:  The title of the table. Defaults to 'Lists'. 
 - **max_rows (int, optional)**:  The maximum number of rows to display. Defaults to MAX_ROWS. 

**Returns:**
 - Non


### `dictionary`

Prints a dictionary in a tabular format.


**Args:**

 - **data (dict)**:  The dictionary to be printed. 
 - **title (str, optional)**:  The title of the table. Defaults to 'Dictionary'. 
 - **columns (list, optional)**:  The column names for the table. Defaults to ['Key', 'Value']. 
 - **max_rows (int, optional)**:  The maximum number of rows to be displayed. Defaults to MAX_ROWS. 

**Returns:**
 - Non


### `listdicts`

Prints a list of dictionaries in a tabular format.


**Args:**

 - **data (list)**:  A list of dictionaries to be printed. 
 - **title (str, optional)**:  The title of the table. Defaults to 'Dictionaries'. 
 - **columns (list, optional)**:  The column names of the table. Defaults to ['Key', 'Value']. 
 - **max_rows (int, optional)**:  The maximum number of rows to be displayed. Defaults to MAX_ROWS. 

**Returns:**
 - Non


### `delta_schema`

Prints the schema of a delta table.


**Args:**

 - **delta_table**:  The delta table object. 

**Returns:**
 - Non


### `delta_metadata`

Prints the metadata information of a delta sharing dataset in a formatted table.


**Args:**

 - **version (str)**:  The version of the metadata. 
 - **metadata (object)**:  The metadata object containing information like name, description, id, partition columns, created time, and configuration. 

**Returns:**
 - Non


### `delta_history`

Display the delta history of a delta sharing dataset in a table format.


**Args:**

 - **history (dict)**:  A dictionary containing the delta history. 

**Returns:**
 - Non


### `print_share_metadata`

Print the share metadata information of a delta sharing dataset.


**Args:**

 - **table_path (str)**:  The path of the table. 
 - **metadata (dict)**:  The metadata dictionary containing information about the table. 

**Returns:**
 - Non


### `print_ds_metadata`

Prints the metadata and schema information of a delta sharing dataset.


**Args:**

 - **table_path (str)**:  The path of the dataset table. 
 - **metadata (dict)**:  The metadata dictionary containing information about the dataset. 

**Returns:**
 - Non


### `print_request_info`

Print the request information in a formatted table.


**Args:**

 - **method (str)**:  The HTTP method of the request. 
 - **endpoint (str)**:  The endpoint of the request. 
 - **path (str)**:  The resource path of the request. 
 - **headers (dict)**:  The headers of the request. 
 - **params (dict, optional)**:  The parameters of the request. Defaults to {}. 
 - **data (dict, optional)**:  The data of the request. Defaults to {}. 

**Returns:**
 - Non



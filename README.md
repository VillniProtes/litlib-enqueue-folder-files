# litlib-enqueue-folder-files
A function that makes it easier to enqueue a bunch of files from one folder when developing WordPress themes.

## How to use
1. Download the file and import it to your THEME directory
2. In your functions.php file write: "require('_FILE DIRECTORY_/litlib_enqueue_folder_files.php');"
3. Now you are able to call the function within your WordPress theme

## Parameters
The function takes a total of 3 parameters

#### $folder parameter (required)
This is the folder within your theme where the files you want grab is located.
Your current theme folder is considered root since the function uses the 
WordPress function "get_stylesheet_directory()".

##### Folder example

_DO_
$folder = 'js';

_DO NOT_
$folder = '/js/;

The function is already looking for a folder so there is no reason to add the beginning
or ending slashes since the function already adds those for you.

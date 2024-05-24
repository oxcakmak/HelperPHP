# HelperPHP
Helper is a method class that imports the functions in the folder you specify and helps you access them easily.

## Support Me

This software is developed during my free time and I will be glad if somebody will support me.

Everyone's time should be valuable, so please consider donating.

[https://buymeacoffee.com/oxcakmak](https://buymeacoffee.com/oxcakmak)

### Installation
You can create a folder called Helper in the Helper.php file, or you can directly call the function classes you will use in any folder.
```php
require_once 'Helper.php';
```

### Usage
```php
/*
The reason why I always give the variable name is that I see it as a function library,
but you can optionally use it as the default $helper variable.
*/
$hepa = new Helper(__DIR__ . '/classes'); // Customize $helperDirectory if needed

/*
* or you can add multiple directories.
* $hepa = new Helper([__DIR__ . '/classes', __DIR__ . '/functions']);
*/

// Call the isEqual function directly on the loader object

// Math class is the "Math.php" file in the "classes" folder.
echo $hepa->Math->isEqual(4, 5) ? 'true' : 'false';
```

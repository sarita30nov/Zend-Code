Album is a sample Module based zend 2 code 

### Main Setup

1. Clone this project into your `./module/` directory and enable it in your
   `application.config.php` file.

```php
return array(
    'modules' => array(
        'Application',
        'Album',//add this to your configuration
    ),
    'module_listener_options' => array(
        'config_glob_paths'    => array(
            'config/autoload/{,*.}{global,local}.php',
        ),
        'module_paths' => array(
            './module',
            './vendor',
        ),
    ),
);
```

Copy the These files

 * `module/Album/config/database.local.php.dist` to `config/autload/database.local.php`
 * `module/Album/config/global.php.dist` to `config/autload/global.php`

###Database Setup
Import module/Album/data/album.sql into your database


http://localhost/zend/public/album
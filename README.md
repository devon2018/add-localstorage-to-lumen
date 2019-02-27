# Adding laravels flystem to lumen
Adding flysystem support to lumen 


## Installation 

```cli 
    composer require league/flysystem
```

Add the following to bootstrap/app.php
```php
    $app->singleton('filesystem', function ($app) {
        return $app->loadComponent('filesystems', 'Illuminate\Filesystem\FilesystemServiceProvider', 'filesystem'); 
    });
```

add filesystems.php to config/

  - Type some Markdown on the left
  - See HTML in the right
  - Magic

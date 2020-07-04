## Check for an Admin View
```php
/**
 * Check if an view already exists.
 *
 * @since 0.1.0
 * 
 * @param string $slug
 * @return boolean
 */
function hasAdminView(string $slug): bool;

/**
 * Check if this is the current view.
 *
 * @since 0.1.0
 *
 * @param string $slug
 * @return boolean
 */
function isAdminView(string $slug): bool;
```

## Add an Admin View
```php
/**
 * Add an admin view.
 *
 * @since 0.1.0
 *
 * @param string $slug
 * @param string $title
 * @param string $view
 * @param array $data
 * @param array $attributes
 * @return void
 */
function addAdminView(string $slug, string $title, string $view, array $data = [], array $attributes = []);
```

If the view is `CustomPlugin\Views\view.blade.php`, the `$view` should be set as `plugin::CustomPlugin.Views.view`.

Before adding an admin view it is recommended to check that an view doesn't already exist AND that the view you are adding is the current one.

```php
$path = 'path/to/view';

if(!hasAdminView($path) && isAdminView($path))
{
	addAdminView($path, ...);
}
```
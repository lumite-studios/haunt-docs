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

## TODO
```php
/**
 * Get an admin view.
 *
 * @since 0.1.0
 *
 * @param string $slug
 * @return array
 */
function getAdminView(string $slug): array;

/**
 * Get all admin views.
 *
 * @since 0.1.0
 *
 * @return \Illuminate\Support\Collection
 */
function getAdminViews(): \Illuminate\Support\Collection;

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
```php
/**
 * Create a form action.
 *
 * @since 0.1.0
 *
 * @param string $slug
 * @param array $data
 * @param boolean $log
 * @return object
 */
function addFormAction(string $slug, array $data = [], bool $log = true): object;

/**
 * Delete a form action.
 *
 * @since 0.1.0
 * 
 * @param string $slug
 * @param boolean $log
 * @param boolean $force
 * @return boolean
 */
function deleteFormAction(string $slug, bool $log = true, bool $force = false): bool;

/**
 * Get a single form action.
 *
 * @since 0.1.0
 *
 * @param string $slug
 * @return object|null
 */
function getFormAction(string $slug): ?object;

/**
 * Check if a form action exists.
 *
 * @since 0.1.0
 *
 * @param string $slug
 * @return boolean
 */
function hasFormAction(string $slug): bool;
```
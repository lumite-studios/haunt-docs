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
function createApplicationFormAction(string $slug, array $data = [], bool $log = true): object;

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
function deleteApplicationFormAction(string $slug, bool $log = true, bool $force = false): bool;

/**
 * Get a single form action.
 *
 * @since 0.1.0
 *
 * @param string $slug
 * @return object|null
 */
function getApplicationFormAction(string $slug): ?object;

/**
 * Check if a form action exists.
 *
 * @since 0.1.0
 *
 * @param string $slug
 * @return boolean
 */
function hasApplicationFormAction(string $slug): bool;
```
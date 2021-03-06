```php
/**
 * Create a permission.
 *
 * @param string $key
 * @param bool $value
 * @param array $data
 * @param bool $log
 * @return object
 */
function createPermission(string $key, bool $value = false, array $data = [], bool $log = true): object;

/**
 * Delete a permission.
 *
 * @param string $slug
 * @param bool $log
 * @param bool $force
 * @return boolean
 */
function deletePermission(string $key, bool $log = true, bool $force = false): bool;

/**
 * Edit a permission.
 * 
 * @param string $key
 * @param array $data
 * @param bool $log
 * @return object|null
 */
function editPermission(string $key, array $data = [], bool $log = true): ?object;

/**
 * Check if a permission exists.
 *
 * @param string $key
 * @return bool
 */
function hasPermission(string $key): bool;

/**
 * Fetch a single permission.
 *
 * @param string $key
 * @return object
 */
function getPermission(string $key): ?object;
```
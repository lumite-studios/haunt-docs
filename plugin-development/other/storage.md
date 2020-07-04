```php
/**
 * Add a new storage driver.
 *
 * @since 0.1.0
 *
 * @param string $driver
 * @param string $title
 * @param array $options
 * @return boolean
 */
function addStorageDriver(string $driver, string $title, array $options = []): bool;

/**
 * Check if a storage driver exists.
 *
 * @since 0.1.0
 *
 * @param string $driver
 * @return boolean
 */
function hasStorageDriver(string $driver): bool;
```
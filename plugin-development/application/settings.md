```php
/**
 * Create a setting.
 *
 * @since 0.1.0
 *
 * @param string $key
 * @param array $data
 * @param boolean $log
 * @return object
 */
function createSetting(string $key, array $data = [], bool $log = true): object;

/**
 * Delete a setting.
 *
 * @since 0.1.0
 *
 * @param string $key
 * @param boolean $log
 * @return boolean
 */
function deleteSetting(string $key, bool $log = true): bool;

/**
 * Edit a setting.
 * 
 * @since 0.1.0
 *
 * @param string $key
 * @param array $attributes
 * @param boolean $log
 * @return object|null
 */
function editSetting(string $key, array $data = [], bool $log = true): ?object;

/**
 * Fetch a single setting.
 *
 * @since 0.1.0
 *
 * @param string $key
 * @return object
 */
function getSetting(string $key): ?object;

/**
 * Get a setting value.
 *
 * @since 0.1.0
 *
 * @param string $key
 * @return null|string
 */
function getSettingValue(string $key): ?string;

/**
 * Check if a setting exists.
 *
 * @since 0.1.0
 *
 * @param string $key
 * @return bool
 */
function hasSetting(string $key): bool;
```
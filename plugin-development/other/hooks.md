```php
/**
 * Add a hook.
 *
 * @since 0.1.0
 *
 * @param string $location
 * @param Closure $function
 * @return void
 */
function addHook(string $location, \Closure $function);

/**
 * Get the hooks in a location.
 *
 * @since 0.1.0
 *
 * @param string $location
 * @return void
 */
function getHook(string $location);

/**
 * Run the hooks in a location.
 *
 * @since 0.1.0
 *
 * @param string $location
 * @param array $data
 * @return void
 */
function runHook(string $location, array $data = []);

/**
 * Check if a hook location exists.
 *
 * @since 0.1.0
 *
 * @param string $location
 * @return void
 */
function hasHooks(string $location);
```
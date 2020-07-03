```php
/**
 * Create a form.
 *
 * @since 0.1.0
 *
 * @param string $title
 * @param array $data
 * @param boolean $log
 * @return object
 */
function createApplicationForm(string $title, array $data = [], bool $log = true): object;

/**
 * Delete a form.
 *
 * @since 0.1.0
 * 
 * @param string $slug
 * @param boolean $log
 * @param boolean $force
 * @return boolean
 */
function deleteApplicationForm(string $slug, bool $log = true, bool $force = false): bool;

/**
 * Edit a form
 *
 * @since 0.1.0
 *
 * @param string $slug
 * @param array $data
 * @param boolean $log
 * @return object|null
 */
function editApplicationForm(string $slug, array $data = [], bool $log = true): ?object;

/**
 * Get a single form.
 *
 * @since 0.1.0
 *
 * @param string $slug
 * @return object|null
 */
function getApplicationForm(string $slug): ?object;

/**
 * Check if a form exists.
 *
 * @since 0.1.0
 *
 * @param string $slug
 * @return boolean
 */
function hasApplicationForm(string $slug): bool;
```
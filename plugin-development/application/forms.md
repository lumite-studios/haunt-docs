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
function createForm(string $title, array $data = [], bool $log = true): object;

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
function deleteForm(string $slug, bool $log = true, bool $force = false): bool;

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
function editForm(string $slug, array $data = [], bool $log = true): ?object;

/**
 * Get a single form.
 *
 * @since 0.1.0
 *
 * @param string $slug
 * @return object|null
 */
function getForm(string $slug): ?object;

/**
 * Check if a form exists.
 *
 * @since 0.1.0
 *
 * @param string $slug
 * @return boolean
 */
function hasForm(string $slug): bool;
```
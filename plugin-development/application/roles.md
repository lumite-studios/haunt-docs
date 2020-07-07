```php
/**
 * Create a role.
 *
 * @param string $slug
 * @param array $attributes
 * @param boolean $log
 * @return object
 */
function createRole(string $slug, array $attributes = [], bool $log = true): object;

/**
 * Delete a role.
 *
 * @param string $slug
 * @param boolean $log
 * @param boolean $force
 * @return boolean
 */
function deleteRole(string $slug, bool $log = true, bool $force = false): bool;

/**
 * Edit a role.
 * 
 * @param string $slug
 * @param array $attributes
 * @param boolean $log
 * @return object|null
 */
function editRole(string $slug, array $attributes = [], bool $log = true): ?object;

/**
 * Fetch a single role.
 *
 * @param string $slug
 * @return object
 */
function getRole(string $slug): ?object;

/**
 * Check if a role exists.
 *
 * @param string $slug
 * @return bool
 */
function hasRole(string $slug): bool;

/**
 * Set a role state.
 *
 * @param string $column
 * @param boolean $state
 * @return void
 */
function setRoleState(string $column, bool $state);
```
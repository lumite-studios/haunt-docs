```php
/**
 * Add items to a menu.
 *
 * @param integer $id
 * @param array $items
 * @return object
 */
function addMenuItems(int $id, array $items = []): object;

/**
 * Create a menu.
 *
 * @param string $name
 * @param array $items
 * @param boolean $log
 * @return object
 */
function createMenu(string $name, array $items = [], bool $log = true): object;

/**
 * Delete a menu.
 *
 * @param integer $id
 * @param boolean $log
 * @return boolean
 */
function deleteMenu(int $id, bool $log = true): bool;

/**
 * Edit a menu.
 * 
 * @param integer $id
 * @param array $data
 * @param boolean $log
 * @return object|null
 */
function editMenu(int $id, array $data = [], bool $log = true): ?object;

/**
 * Generate a menu.
 *
 * @param string $location
 * @param array $attributes
 * @return string
 */
function generateMenu(string $location, array $attributes = []): ?string;

/**
 * Fetch a single menu.
 *
 * @param integer $id
 * @return object
 */
function getMenu(int $id): ?object;

/**
 * Check if a menu exists.
 *
 * @param integer $id
 * @return bool
 */
function hasMenu(int $id): bool;
```
```php
/**
 * Create a page.
 *
 * @since 0.1.0
 *
 * @param string $title
 * @param string $content 
 * @param array $data
 * @param boolean $log
 * @return object
 */
function createPage(string $title, string $content, array $data = [], bool $log = true): object;

/**
 * Delete a page.
 *
 * @since 0.1.0
 *
 * @param string $slug
 * @param boolean $log
 * @param boolean $force
 * @return boolean
 */
function deletePage(string $slug, bool $log = true, bool $force = false): bool;

/**
 * Edit a page.
 * 
 * @since 0.1.0
 *
 * @param string $slug
 * @param array $data
 * @param boolean $log
 * @return object|null
 */
function editPage(string $slug, array $data = [], bool $log = true): ?object;

/**
 * Fetch a single page.
 *
 * @since 0.1.0
 *
 * @param string $slug
 * @return object|null
 */
function getPage(string $slug): ?object;

/**
 * Check if a page exists.
 *
 * @since 0.1.0
 *
 * @param string $slug
 * @return bool
 */
function hasPage(string $slug): bool;
```
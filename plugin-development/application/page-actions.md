```php
/**
 * Add a page action.
 *
 * @since 0.1.0
 *
 * @param string $page
 * @param Closure $function
 * @return void
 */
function addPageAction(string $page, \Closure $function): void;

/**
 * Get the actions for a page.
 *
 * @since 0.1.0
 *
 * @param string $page
 * @return \Illuminate\Support\Collection
 */
function getPageAction(string $page): \Illuminate\Support\Collection;

/**
 * Run the actions for a page.
 *
 * @since 0.1.0
 *
 * @param string $location
 * @param array $data
 * @return void
 */
function runPageAction(string $page, array $data = []): void;

/**
 * Check if any actions exist.
 *
 * @since 0.1.0
 *
 * @param string $page
 * @return boolean
 */
function hasPageActions(string $page): bool;
```
## Add Plugin Translations
```php
/**
 * Add translations for a plugin.
 *
 * @since 0.1.0
 *
 * @param string $plugin
 * @param string $location
 * @return void
 */
function addPluginTranslations(string $plugin, string $location);
```

## Guide
Translations should be added during the plugins `init` event like so: `addPluginTranslations(PLUGIN_NAMESPACE, PLUGIN_DIRECTORY.'/resources/lang')`. It will then be possible to fetch translations like `__(PLUGIN_NAMESPACE.'::settings/views.title')`.
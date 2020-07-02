## Base Plugin
A plugin must extend the `BasePlugin` class.

```
namespace CustomPlugin;

use Lumite\Haunt\Plugin\BasePlugin;

class Plugin extends BasePlugin
{
	/**
	 * Create a new plugin instance.
	 *
	 * @return void
	 */
	public function __construct();
}
```

### Constructor
To assist with later functions, you can define paths here.

```
/**
 * Create a new plugin instance.
 *
 * @return void
 */
public function __construct()
{
    if(!defined('PLUGIN_NAMESPACE'))
		{
	    	define('PLUGIN_NAMESPACE', basename(__DIR__));
		}

		if(!defined('PLUGIN_DIRECTORY'))
		{
	    	define('PLUGIN_DIRECTORY', dirname(__FILE__));
		}
		
		...
}
```

## plugin.json
Each plugin must include a plugin.json file, this contains the information about the plugin being installed.

```
{
  "name": "My Custom Plugin",
	"slug": "CustomPlugin",
	"main": "Plugin.php",
	"description": "This is a plugin.",
	"version": "1.0",
	"author": "Author Name",
	"author_url": "https://site.site",
	"requires":
	[
			"PluginName"
	]
}
```

name: The name of the plugin.
slug: The slug of the plugin, this should be used as the namespace for the main plugin file. This must be unique
main: The name of the main plugin file.
description [optional]:
version [optional]:
author [optional]:
author_url [optional]:
requires[optional]:
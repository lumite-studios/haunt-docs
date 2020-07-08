## Trait
{% hint style="info" %}
use Lumite\Haunt\Plugin\Traits\Database;
{% endhint %}

This trait allows a plugin to add or change database tables through the use of migrations.

```php
/**
 * The path for where the migrations are located. 
 *
 * @since 0.1.0
 *
 * @var string
 */
public $migration_path;

/**
 * Check if a table exists.
 *
 * @since 0.1.0
 *
 * @param string $table     The name of the table to check.
 * @return boolean
 */
public function hasTable(string $table): bool;

/**
 * Get the migration path.
 * 
 * @since 0.1.0
 *
 * @return string
 */
public function getMigrationPath(): string;

/**
 * Set the migration path.
 * 
 * @since 0.1.0
 *
 * @param string $path
 * @return void
 */
public function setMigrationPath(string $path);
```

## Migrations
A migration is a file used to create or edit a database table, an example of this has been given below. Be sure to include the haunt table prefix with haunt_table_prefix() before the table name.

```php
// 2020_01_01_000000_table_name.php

use Illuminate\Database\Migrations\Migration;
use Illuminate\Database\Schema\Blueprint;
use Illuminate\Support\Facades\Schema;

class TableName extends Migration
{
    /**
     * Run the migrations.
     *
     * @return void
     */
    public function up()
    {
        // create a table
        Schema::create(haunt_table_prefix().'table_name', function(Blueprint $table)
        {
            $table->string('column');
        });
        
        // OR
        
        // edit a table
        Schema::table(haunt_table_prefix().'table_name', function (Blueprint $table)
        {
            $table->string('new_column');
        });
    }

    /**
     * Reverse the migrations.
     *
     * @return void
     */
    public function down()
    {
        // if up creates a table
        Schema::dropIfExists(haunt_table_prefix().'table_name');
        
        // OR
        
        // if up edits a table
        Schema::table(haunt_table_prefix().'table_name', function (Blueprint $table)
        {
            $table->dropColumn('new_column');
        });
    }
}
```

You can look up additional information regarding migrations within the Laravel documentation:
https://laravel.com/docs/master/migrations
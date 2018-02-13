# CDN Loader for WordPress

Simple plugin that will load all public assets from a CDN instead of your local server.

### Usage
1. Install the plugin
2. Define the following constant in your `wp-config.php`
```php
define( 'DVK_CDN_URL', '//cdn.cloudfront.net' );
define("WP_CONTENT_URL", "//cdn.cloudfront.net/wp-content");
define("COOKIE_DOMAIN", "www.cloudfront.net");
define("WP_PLUGIN_URL", "//cdn.cloudfront.net/wp-content/plugins");
```

The plugin won't replace assets when `SCRIPT_DEBUG` is enabled.

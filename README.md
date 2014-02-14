sellwp-updater
==============

Theme and Plugin updater for SellWP.com


To use add this sellwp-updater.php file to the root of your theme or plugin.

Add these line of code to the functions.php in your theme or main file in your plugin:

```

add_action('init', 'YOUR_THEME_OR_PLUGIN_PREFIX_sellwp_updater');

function YOUR_THEME_OR_PLUGIN_PREFIX_sellwp_updater() {
    include( 'sellwp-updater.php' );
    new SellWP_Updater(
	    $license_key, 
	    $current_version,
	    plugin_basename(__FILE__)
    );
}

```



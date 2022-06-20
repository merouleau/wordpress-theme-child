# wordpress-theme-child

Starter files for a WordPress child theme. To install for installed parent
theme foo visit wp-content/themes and, generically:

```
mkdir foo-child
cd foo-child
git clone https://github.com/merouleau/wordpress-theme-child
cp -p wordpress-theme-child/style.css.orig style.css
cp -p wordpress-theme-child/functions.php.orig functions.php
vi style.css
vi functions.php
```

If you want a thumbnail to show on the WP theme selection page, copy the
parent's screenshot.png or create a new screenshot.png. The aspect ratio is 4:3
(e.g. 1200x900), and the bottom sixth of the image will be obscured by the
theme name.

Here's a specific example for child ApoE4Info of parent Twenty Twenty-Two:
```
mkdir apoe4info
cd apoe4info
git clone https://github.com/merouleau/wordpress-theme-child
cp -p wordpress-theme-child/style.css.orig style.css
cp -p wordpress-theme-child/functions.php.orig functions.php
cp -p ../twentytwentytwo/screenshot.png .
```

Preamble for style.css:
```
/*
Theme Name: ApoE4Info
Template: twentytwentytwo
Text Domain: apoe4info
Version: 1.0
Description: ApoE4Info is a child of Twenty Twenty-Two customized for the ApoE4.
Author: Marc Rouleau
*/
```

Changes to functions.php:

1. Comment out function enqueue_parent_styles().
2. Replace child-style with apoe4info.
3. Replace READ_PARENT_functions_php_TO_GET_THE_PARENT_HANDLE with twentytwentytwo-style.

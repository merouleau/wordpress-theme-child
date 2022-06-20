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

Here's a specific example for child ApoE4Info of parent Twenty Twenty-Two:
```
mkdir apoe4info
cd apoe4info
git clone https://github.com/merouleau/wordpress-theme-child
cp -p wordpress-theme-child/style.css.orig style.css
cp -p wordpress-theme-child/functions.php.orig functions.php
```

Preamble for style.css:
```
```

Changes to functions.php:

1. Comment out function enqueue_parent_styles().
2. Replace child-style with apoe4info.
3. Replace READ_PARENT_functions_php_TO_GET_THE_PARENT_HANDLE with twentytwentytwo-style.

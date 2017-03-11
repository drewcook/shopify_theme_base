# Shopify Theme Base
This is a boilerplate starter theme for Shopify. This new build process utilizes the combination of Shopify's **Theme Kit** and Shopify's [Skelaton Theme](https://github.com/Shopify/skeleton-theme).

***

###Upload initial skelaton theme into your shop

1. Go download the [Skelaton Theme](https://github.com/Shopify/skeleton-theme) as a .zip file
2. Navigate to your store's Themes section and click *Upload Theme*
3. Find the *skelaton-theme-master.zip* file you just downloaded and click upload
4. Publish the theme to where it is active on the store


###To initialize a new theme development build:

1. Download this repo's .zip file [Download Here](https://github.com/drewcook/shopify_theme_base/archive/master.zip)
2. Unpack it and move it into your local project directory.
  * You may rename the root to any name of your choice
3. Navigate into local project directory in console
4. Run command `git init` if tracking changes with Git
5. Run command `cp config-sample.yml config.yml` to set up configuration with Shopify store URL
6. Set up a private app in Shopify named *'Store Name - Theme Dev'* and set read and write permissions for *'Theme templates and theme assets'* option. It will yeild a password. Use this password for next step.
7. Replace dummy data in *config.yml* with the correct store URL, generated private app password, and theme ID and save the file. This will link up your local files with your shop.
  * Your store URL will be my-store-name.myshopify.com
  * Your password can be found under the private app you just set up under Authentication
  * Your theme ID can be found by opening up the theme page in the browser by clicking **Edit HTML/CSS**, and it can be found as a set of digits in the web address `my-store-name.myshopify.com/admin/themes/XXXXXXXXX`
  * Make sure that the theme ID is in string format
8. Now that Theme Kit is set up with the store and your working files are configured with the ones that are live, run command `theme watch` to start watching for changes on local repo. These changes will now take place on development store. Make sure to refresh to view the new changes.

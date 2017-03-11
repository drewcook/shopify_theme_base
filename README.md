# shopify_theme_base
This is a boilerplate starter theme for Shopify.  This takes the combination of **Theme Kit** and Shopify's [Skelaton Theme](https://github.com/Shopify/skeleton-theme).

***

###To start a new theme build:

1. Download .zip file
2. Unpack zip into project directory
3. Navigate into project directory in console
4. Run command `git init` if tracking changes with Git
5. Run command `cp config-example.yml config.yml` to set up configuration with Shopify store URL
6. Set up a private app in Shopify named `Store Name - Theme Dev` and set read and write permissions for `Theme templates and theme assets` option. It will yeild a password. Use this password for next step.
7. Replace dummy data in config.yml with the correct store URL, generated private app password, and theme ID.
8. Now that Theme Kit is set up with the store, run command `theme watch` to start watching for changes on local repo. These changes will now take place on development store, make sure to refresh.


# n98-magerun version 1.97.30 by netz98 GmbH

#### Usage:
  command [options] [arguments]

#### Options:
    -h, --help                 Display this help message
    -q, --quiet                Do not output any message
    -V, --version              Display this application version
        --ansi                 Force ANSI output
        --no-ansi              Disable ANSI output
    -n, --no-interaction       Do not ask any interactive question
        --root-dir[=ROOT-DIR]  Force magento root dir. No auto detection
        --skip-config          Do not load any custom config.
        --skip-root-check      Do not check if n98-magerun runs as root
    -v|vv|vvv, --verbose       Increase the verbosity of messages: 1 for normal output, 
     2 for more verbose output and 3 for debug.

#### Available commands:
      help                               Displays help for a command
      install                            Install magento
      list                               Lists commands
      mysql-client                       Opens mysql client by database config from local.xml
      open-browser                       Open current project in browser (experimental)
      script                             Runs multiple n98-magerun commands
      self-update                        Updates n98-magerun.phar to the latest version.
      selfupdate                         Updates n98-magerun.phar to the latest version.
      shell                              Runs n98-magerun as shell
      uninstall                          Uninstall magento (drops database and empties current 
                                         folder or folder set viainstallationFolder)
 
 #### admin
      admin:notifications                Toggles admin notifications
      admin:user:change-password         Changes the password of a adminhtml user.
      admin:user:change-status           Set active status of an adminhtml user. 
                                         If no option is set the status will be toggled.
      admin:user:create                  Create admin user.
      admin:user:delete                  Delete the account of a adminhtml user.
      admin:user:list                    List admin users.
      admin:user:lock                    Enforce a lock on an admin user account. Specify the username and an optional             lifetime parameter in seconds.
      admin:user:lockdown                Lock every admin user account for the optionally specified lifetime (in days).
                                         If not provided, defaults to one month.
      admin:user:unlock                  Release lock on admin user for one or all users
 
 #### cache
  cache:clean                        Clean magento cache
  cache:dir:flush                    Flush (empty) Magento cache directory
  cache:disable                      Disables magento caches
  cache:enable                       Enables magento caches
  cache:flush                        Flush magento cache storage
  cache:list                         Lists all magento caches
  cache:report                       View inside the cache
  cache:view                         Prints a cache entry
 category
  category:create:dummy              Create a dummy category
 cms
  cms:banner:toggle                  Toggle a banner (Enterprise only)
  cms:block:toggle                   Toggle a cms block
  cms:page:publish                   Publish a CMS page revision (Enterprise only)
 composer
  composer:diagnose                  Diagnoses the system to identify common errors.
  composer:init                      Creates a basic composer.json file in current directory.
  composer:install                   Installs the project dependencies from the composer.lock file if present, or falls back on the composer.json.
  composer:require                   Adds required packages to your composer.json and installs them
  composer:search                    Search for packages
  composer:update                    Updates your dependencies to the latest version according to composer.json, and updates the composer.lock file.
  composer:validate                  Validates a composer.json and composer.lock
 config
  config:delete                      Deletes a store config item
  config:dump                        Dump merged xml config
  config:get                         Get a core config item
  config:search                      Search system configuration descriptions.
  config:set                         Set a core config item
 customer
  customer:change-password           Changes the password of a customer.
  customer:create                    Creates a new customer/user for shop frontend.
  customer:create:dummy              Generate dummy customers. You can specify a count and a locale.
  customer:delete                    Delete Customer/s
  customer:info                      Loads basic customer info by email address.
  customer:list                      Lists customers
 db
  db:console                         Opens mysql client by database config from local.xml
  db:create                          Create currently configured database
  db:drop                            Drop current database
  db:dump                            Dumps database with mysqldump cli client according to informations from local.xml
  db:import                          Imports database with mysql cli client according to database defined in local.xml
  db:info                            Dumps database informations
  db:maintain:check-tables           Check database tables
  db:query                           Executes an SQL query on the database defined in local.xml
  db:status                          Shows important server status information or custom selected status values
  db:variables                       Shows important variables or custom selected
 design
  design:demo-notice                 Toggles demo store notice for a store view
 dev
  dev:class:lookup                   Resolves a grouped class name
  dev:code:model:method              Code annotations: Reads the columns from a table and writes the getter and setter methods into the class file for @methods.
  dev:console                        Opens PHP interactive shell with initialized Mage::app() (Experimental)
  dev:email-template:usage           Display database transactional email template usage
  dev:ide:phpstorm:meta              Generates meta data file for PhpStorm auto completion
  dev:log                            Toggle development log (system.log, exception.log)
  dev:log:db                         Turn on/off database query logging
  dev:log:size                       Get size of log file
  dev:merge-css                      Toggles CSS Merging
  dev:merge-js                       Toggles JS Merging
  dev:module:create                  Create and register a new magento module.
  dev:module:dependencies:from       Show list of modules which depend on %s module
  dev:module:dependencies:on         Show list of modules which given module depends on
  dev:module:disable                 Disable a module or all modules in codePool
  dev:module:enable                  Enable a module or all modules in codePool
  dev:module:list                    List all installed modules
  dev:module:observer:list           Lists all registered observers
  dev:module:rewrite:conflicts       Lists all magento rewrite conflicts
  dev:module:rewrite:list            Lists all magento rewrites
  dev:module:update                  Update a Magento module.
  dev:profiler                       Toggles profiler for debugging
  dev:report:count                   Get count of report files
  dev:setup:script:attribute         Creates attribute script for a given attribute code
  dev:symlinks                       Toggle allow symlinks setting
  dev:template-hints                 Toggles template hints
  dev:template-hints-blocks          Toggles template hints block names
  dev:theme:duplicates               Find duplicate files (templates, layout, locale, etc.) between two themes.
  dev:theme:info                     Displays settings of current design on particular store view
  dev:theme:list                     Lists all available themes
  dev:translate:admin                Toggle inline translation tool for admin
  dev:translate:export               Export inline translations
  dev:translate:set                  Adds a translation to core_translate table. Globally for locale
  dev:translate:shop                 Toggle inline translation tool for shop
 eav
  eav:attribute:create-dummy-values  Create a dummy values for dropdown attributes
  eav:attribute:list                 Lists all EAV attributes
  eav:attribute:remove               Removes attribute for a given attribute code
  eav:attribute:view                 View informations about an EAV attribute
 extension
  extension:download                 Download magento-connect package
  extension:install                  Install magento-connect package
  extension:list                     List magento connection extensions
  extension:search                   List magento connection extensions
  extension:upgrade                  Upgrade magento-connect package
  extension:validate                 Reads Magento Connect Config, and checks that installed package files are really there
 giftcard
  giftcard:create                    Create a gift card with a specified amount
  giftcard:info                      Get gift card account information by code
  giftcard:pool:generate             Generate giftcard pool
  giftcard:remove                    Remove a gift card account by code
 index
  index:list                         Lists all magento indexes
  index:list:mview                   Lists all magento mview indexes
  index:reindex                      Reindex a magento index by code
  index:reindex:all                  Reindex all magento indexes
  index:reindex:mview                Reindex a magento index by code using the materialised view functionality
 local-config
  local-config:generate              Generates local.xml config
 media
  media:dump                         Creates an archive with content of media folder.
 script
  script:repo:list                   Lists all scripts in repository
  script:repo:run                    Run script from repository
 sys
  sys:check                          Checks Magento System
  sys:cron:history                   Last executed cronjobs with status.
  sys:cron:list                      Lists all cronjobs
  sys:cron:run                       Runs a cronjob by job code
  sys:info                           Prints infos about the current magento system.
  sys:maintenance                    Toggles maintenance mode.
  sys:modules:list                   List all installed modules
  sys:setup:change-version           Change module setup resource version
  sys:setup:compare-versions         Compare module version with core_resource table.
  sys:setup:incremental              List new setup scripts to run, then runs one script
  sys:setup:remove                   Remove module setup resource entry
  sys:setup:run                      Runs all new setup scripts.
  sys:store:config:base-url:list     Lists all base urls
  sys:store:list                     Lists all installed store-views
  sys:url:list                       Get all urls.
  sys:website:list                   Lists all websites

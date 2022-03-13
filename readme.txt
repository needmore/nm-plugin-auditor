=== Plugin Auditor ===
Contributors: eugenemolari, helloluke, MatheusFD, wholegraindigital
Requires at least: 4.0
Tested up to: 5.1.1
Stable tag: 2.4.3
Tags: plugin audit, audit, security, maintenance, audit trail
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html
The Plugin Auditor plugin records details of who installed and activated each plugin on your website and why.

== Description ==

Have you ever had that situation where you have a bunch of plugins installed and you can't remember why half of them are there?  

It is important to clean out unused plugins and keep your plugins up to date, but this can be difficult if you have forgotten why you installed them in the first place.  This is particularly true for sites with multiple admin users, and for agencies that manage their clients sites.

You don't want to delete an old plugin without being 100% sure why it was installed and therefore know if it is still needed. 

The Plugin Auditor tells you why each plugin was installed and also keeps a record of who installed it so that you know who to ask if you have any questions when performing maintenance on the site.

Plugin Auditor can be installed at any time but to get the most benefit from it, it should be installed as the first plugin that you install on any WordPress site that you manage.

== Installation ==

The Plugin Auditor plugin is really plug and play.  Just upload the plugin and activate.

1. Upload `plugin-audit.php` to the `/wp-content/plugins/` directory

2. Activate the plugin through the 'Plugins' menu in WordPress

To view the logs of plugin activity on your site, simply go to Plugins > Plugin Auditor.

== Frequently Asked Questions ==

= Will it work with all themes? =

Yes, it should work fine with all themes.  If you find a problem, let us know.

= Does it work on multisite installations? =

Yes, we have added basic multisite compatibility. On a mutlisite network, the Plugin Auditor notifications and audit table will only appear under the Network admin area, but will track activity throughout the network. In future, we hope to add more comprehensive multisite functionality.

= What happens if I install this plugin after other plugins? =

The Plugin Auditor has no way of knowing who installed existing plugins or when they were installed. It will therefore assign them to the person who installed the plugin and display. If you know this information, you should manually leave a comment for future reference.  


== Screenshots ==

1. The note field, where you will add your comment saying why did you add a plugin

2. A screenshot of the main table, showing all the content about the plugin

3. If is a multisite installation, you will find all the sites and the plugin within it

== Changelog ==

= v2.4.3 (2017-02-28) =

Bug Fixes:

* Fixed compatibility with WordPress CSS

= v2.4.2 (2017-01-31) =

General:

* Fixed CSS to admin dashboard

= v2.4.1 (2017-01-10) =

General:

* Fixed the export data to CSV and XLS feature

= v2.4.0 (2016-08-06) =

General:

* Fixed the issue of delete comments and loss data ( https://goo.gl/KSLsnS )

= v2.3.1 (2016-05-19) =

General:

* Bug fixes
* Corrected issue in plugin name on multisite list

Enhancements:

* Added the ability to edit note via Ajax, without reload all the page content
* Improved the list style to match the plugin default

= v2.3.0 (2016-05-02) =

General:

* Bug fixes

Enhancements:

* Added the ability to export data into a CSV file
* To all exported files, the default name of the file is "Plugin_Auditor_ + date". ie.: "Plugin_Auditor_2016-05-02"
* To fix users capabilities issue, now only users that can update plugins, that have admin privileges, are able to add comments and see the Audit Table

= v2.2.0 (2016-04-22) =

General:

* Bug fixes

Enhancements:

* If is a multisite installation, added the list of all multisites and the activated plugins within each subsite
* Removed "Manage Comments" column when table is exported to make it clean

= v2.1.0 (2016-04-18) =

General:

* Bug fixes
* Corrects non-object notice

Enhancements:

* Added the ability to export table into a XLS file
* Removed the status bar

= v2.0.1 (2016-04-08) =

General:

* Table styles changed to match with WordPress default
* Table is responsive to allow the user to edit his comments on small screens

= v2.0.0 (2016-04-08) =

General:

* Bug fixes
* Removed Plugin Auditor record to avoid metalanguage

Enhancements:

* Added the ability to translate Plugin Auditor into any language

= v1.1.0 (2016-04-04) =

General:

* Bug fixes
* Table styles changed to match WordPress default
* A heading was added to easily understand the plugin function
* Removed WordPress version from table to make it clean

Enhancements:

* Fixed uninstalled plugin issue, removing record when plugin is deleted
* XSS and SQL injection correction
* Verification if a real user has added a plugin or the plugin was added before Plugin Auditor installation, adding the user to the existing plugin

= v1.0.0 (2016-03-28) =

General:

* Bug fixes

Enhancements:

* Added the ability to know how many plugins need a comment - pagination
* Added the compatibility with WordPress multisites
* Changed the version numbering system
* Simplified the paragraph asking why a plugin was installed

= v0.2.0 (2016-03-03) =

General:

* Bug fixes
* The plugin description was changed to match the real functionality it is doing

Enhancements:

* Added option not to provide a comment about a plugin if the user does not want to
* Added the ability to sort the table info according to user preference
* Added the real name of the user that installed the plugin
* Added a prompt title to let the user to identify the comment box
* Added the ability to edit comments
* Added the functionality of deleting database entries on uninstall (but not on deactivate)
* Added the functionality of ONLY asking the user to describe what a plugin is for when it is installed, not when it is activated/deactivated or updated.
* The table of content is now responsive to let users use the Plugin Auditor table on all devices.
* Changed textarea placeholder (from "add a short comment to explain" to "add comments here")
* Renamed plugin's name in the menu (from "Auditor" to "Plugin Auditor")
* Removed user role from table

= 0.1.0 =
* Initial version

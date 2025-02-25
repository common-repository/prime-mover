=== Prime Mover - Migrate WordPress Website & Backups ===
Contributors: codexonics, freemius
Donate link: https://codexonics.com
Tags: migrate wordpress, multisite migration, clone, backup
Requires at least: 4.9.8
Tested up to: 6.7
Requires PHP: 5.6
Stable tag: 2.0.0
License: GPLv3 or later
License URI: https://codexonics.com

The simplest all-around WordPress migration tool/backup plugin. These support multisite backup/migration or clone WP site/multisite subsite.

== Description ==

= Easily Transfer WordPress Site to New Host/Server/Domain =

*   Move single-site installation to another single site server.
*   Move WP single-site to existing multisite sub-site.
*   Migrate subsite to another multisite sub-site.
*   Migrate multisite sub-site to single-site.
*   Migrate within WordPress admin.
*   WordPress backup and restore packages within single-site or multisite.
*   Backup WordPress subsite (in multisite).
*   You can backup the WordPress database within admin before testing something and restore it with one click.
*   Cross-platform compatible (Nginx / Apache / Litespeed / Microsoft IIS / Localhost).
*   Clone single site and restore it to any server.
*   Clone subsite in multisite and restore it as single-site or multisite.
*   Supports legacy multisites.
*   Debug package.
*   Supports backup of the non-UTF8 single-site or multisite database.

https://youtu.be/QAVVXcoQU8g

= PRO Features =

*   Scheduled backups: Automatic backup support for multisite and single-site.
*   Save tons of time during migration with the direct site to site package transfer.
*   Move the backup location outside WordPress public directory for better security.
*   Migrate or backup WordPress multisite main site.
*   Encrypt WordPress database in backups for maximum data privacy.
*   Encrypt WordPress upload files inside backup for better security.
*   Encrypt plugin and theme files inside the backup/package for protection.
*   Export and restore the backup package from Dropbox.
*   Save and restore packages from and to Google Drive.
*   Exclude plugins from the backup (or network activated plugins if multisite).
*   Exclude upload directory files from the backup to reduce the package size.
*   Create a new multisite subsite with a specific blog ID.
*   Disable network maintenance in multisite so only affected subsite is in maintenance mode.
*   Configure migration parameters to optimize and tweak backup/migration packages.
*   It includes all complete restoration options at your own choice and convenience.
*   Full access to settings screen to manage all basic and plugin advanced configurations.
*   Migrate non-UTF8 database charset to standard UTF8 database charset (utf8mb4).
*   Migrate UTF8 database charset (utf8mb4) to non-UTF8 database charset (edge case scenario).

= Documentation =

*	[Prime Mover Documentation](https://codexonics.com/prime_mover/prime-mover/)

== Installation ==

1. Upload to the `/wp-content/plugins/` directory
2. Activate the plugin through the 'Plugins' menu in WordPress
3. Optionally, opt in to security & feature updates notification including non-sensitive diagnostic tracking with freemius.com. If you skip this, that's okay! Prime Mover will still work just fine.
4. You should see the Prime Mover Control Panel. Click "Go to Migration Tools" to start migrating sites.

== Frequently Asked Questions ==

= What makes Prime Mover unique to other existing migration and backup plugins? =
	
* The free version has no restriction on package size, number of websites or mode of migration (single-site or multisite will work). (Note: Exporting/Restoring a multisite main site is a PRO feature)
* The free version supports WordPress multisite migration on any number of subsites except that exporting/restoring the multisite main site is a PRO feature.
* It can backup WordPress multisite sub-sites or migrate multisite.
* No need to delete your WordPress installation, create/delete the database, and all other technical stuff. It will save you a lot of time.
* This is not hosting-dependent. Prime Mover is designed to work with any hosting companies you want to work with.
* The free version has full multisite migration functionality. This feature is usually missing in most migration plugins free version.
* Full versatility - migrating from your localhost, dev site, or from a live site to another live site.
* You will be doing the entire migration inside the WordPress admin. Anyone with administrator access can do it. There is no need to hire a freelancer to do the job - saves you money.
* No messing with complicated migration settings, the free version has built-in settings. Only choose a few options to export and migrate, that's it. 
* You can save, download, delete, and migrate packages using the management page.
* No need to worry about PHP configuration and server settings. Compatible with most default PHP server settings even in limited shared hosting. 
* Prime Mover works with modern PHP versions 5.6 to 8.3+ (Google Drive feature requires at least PHP 7.4).
* The code is following PHP-fig coding standards (standard PHP coding guidelines).
* The free version supports backup and restoration of non-UTF8 sites. However, you need the PRO version to migrate non-UTF8 to the UTF8 (utf8mb4) database charset and vice versa.
* You don't need to worry about setting up users or changing user passwords after migration. It does not overwrite existing site users after migration.

For more common questions, please read the [plugin FAQ listed in the developer site](https://codexonics.com/prime_mover/prime-mover/faq/).

== Screenshots ==

1. Single-site Migration Tools
2. Export options dialog
3. Export to single-site format example
4. Export to multisite subsite with blog ID of 23 example
5. Restore package via browser upload
6. Single-site package manager
7. Prime Mover network control panel
8. Export and restore package from Network Sites
9. Multisite network package manager

== Upgrade Notice ==

Update now to get all the latest bug fixes, improvements and features!

== Changelog ==

= 2.0.0 =

* Feature: Support for automated and scheduled backups.
* Compatibility: Tested for WordPress 6.7 compatibility.
* Fixed: Updated Freemius SDK library to latest version 2.9.0.
* Fixed: Google Drive API session is not global when already connected.
* Fixed: Issues with parallel exports.
* Fixed: Runtime error when restoring database to unsupported collation type.
* Fixed: Helpful errors when Prime Mover has issues writing to an archive.
* Fixed: Runtime errors associated with database tables names containing allowed special characters.
* Fixed: Runtime error on export if site uses database names with allowed special characters on it.
* Fixed: Normalize paths for packages for Windows server.
* Fixed: Missing administrator capabilities when migrating from multisite to single-site.
* Fixed: Broken migration if site uses relative wp-content URLs.
* Fixed: Runtime error during migration if site enables WP_DEBUG_DISPLAY + WP_DEBUG mode to true.

= 1.9.9 =

* Fixed: Incompatibility issues with database servers using ANSI_QUOTE SQL mode.
* Fixed: Unable to rename tables, please check that your database is not empty or these tables exists.
* Fixed: Removed support for sites that have empty database prefix set.
* Fixed: Updated Freemius SDK to version 2.7.2.
* Fixed: Uncaught Exception: Unable to locate placement anchor.
* Fixed: Added PHP 8.3 as the latest supported PHP version.

= 1.9.8 =

* Fixed: Bug on missing entries on user equivalence data during import.
* Fixed: Memory limit error on import when max post author ID is an extremely large number.
* Fixed: Limit readme tags as per guidelines.
* Fixed: Compatibility issues with newer version of BuddyBoss plugin.
* Fixed: Edge case issue of missing BuddyPress avatar / member images in uploads directory.

See the previous changelogs in changelog.txt.

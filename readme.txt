=== WP Job Manager - Custom Management Role ===
Contributors: macbookandrew
Tags: job listing, job board, job, jobs, company, hiring, employment, employees, candidate, freelance, internship, custom manager
Requires at least: 3.8
Tested up to: 4.1
Stable tag: 1.0

Allows a user who has the 'edit_others_job_applications' capability to edit job applications posted by anyone.

== Description ==

Typically, only the user who posted a job can manage the applications. This plugin allows any user with the 'edit_others_job_applications' capability to manage applications.

= Documentation =

Documentation for the core plugin and add-ons can be found [on the docs site here](https://wpjobmanager.com/documentation/).

= Contributing and reporting bugs =

You can contribute code to this plugin via GitHub: [https://github.com/Pressed-Solutions/WP-Job-Manager](https://github.com/Pressed-Solutions/WP-Job-Manager)

== Installation ==

= Automatic installation =

Automatic installation is the easiest option as WordPress handles the file transfers itself and you don't even need to leave your web browser. To do an automatic install, log in to your WordPress admin panel, navigate to the Plugins menu and click Add New.

In the search field type "WP Job Manager - Customized Management Role" and click Search Plugins. Once you've found the plugin you can view details about it such as the the point release, rating and description. Most importantly of course, you can install it by clicking _Install Now_.

= Manual installation =

The manual installation method involves downloading the plugin and uploading it to your webserver via your favourite FTP application.

* Download the plugin file to your computer and unzip it
* Using an FTP program, or your hosting control panel, upload the unzipped plugin folder to your WordPress installation's `wp-content/plugins/` directory.
* Activate the plugin from the Plugins menu within the WordPress admin.

= Getting started =

Once installed, grant your user(s) the `edit_others_job_applications` capability.

1. Using the [Members](https://wordpress.org/plugins/members/) plugin, you can create a new role and click a checkbox to grant the capability.
2. Add this code to your `functions.php` file:
`$user = new WP_User( $user_id );`
`$user->add_cap( 'can_edit_posts' );`


== Changelog ==

= 1.0 =
* Basic plugin

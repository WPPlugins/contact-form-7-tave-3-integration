=== Plugin Name ===
Contributors: Ryan Rowell
Tags: contact form 7, Táve
Requires at least: 4.2
Tested up to: 4.4
Stable tag: 2014.12.04
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

This adds Táve integration to all Contact Form 7 forms on a blog.

== Description ==

This plugin adds Táve integration to all Contact Form 7 forms on your blog. This allows you to create forms that will enter details directly into Táve.

You can find a more detailed explanation and walkthrough here: http://www.rowellphoto.com/tave-contact-form-plugin/

== Installation ==

Install [Contact Form 7] (http://wordpress.org/extend/plugins/contact-form-7/) v3.9+ and set up a form.

Install the plugin as per usual. Add your Táve Studio Secret key and Táve Studio Alias info to the settings page.
Check your Contact Form 7 forms to ensure they use fields with these names below. All field
names should be available in your Settings>Data Administration>Integrations>New Lead API section of Táve, if they
are not there, they will be created from the form and you may not want this. Also everything is case sensitive.

FirstName, LastName, Email, HomePhone, MobilePhone, WorkPhone, Source, EventDate, JobType, Message

Then any custom fields you create through the Táve custom fields in the settings.

You can find a more detailed explanation and walkthrough here: http://www.rowellphoto.com/tave-contact-form-plugin/

== Frequently Asked Questions ==

= Does this work with the forms from ProPhoto template  =

No.

== Changelog ==

= 2014.12.03 =
* Changed the name from Táve 3 to just Táve, less confusion this way. 
* Also updated the links inside the plugin to the new lead api page in the settings. 

= 2014.12.03 =
* Removed the error logging to a file, no need to have that. 
* Bug fix, wasn't looking for the space after the comma in the separate fields to be ignored. So now all fields (not just the first one) added to this list will be ignored and left un-sent to tave. 

= 2014.11.13 =
* stupid bug. linked two checkboxes by accident. all fixed. (Thanks Eve Prime)

= 2014.11.12 =
* Minimum requirements set for WordPress 4 (makes it mandatory to update so you can see the new Contact Forms 7)
* added: error log checkbox to log all uses of the form to a txt file, only contains info needed to debug, no form data.
* added: at the bottom of the settings page you can now see the same details the log file would contain but only from the last message sent.
* removed set CURLOPT_FOLLOWLOCATION => true
* sorry to report this wont fix current connection issues, but it will you let me know whats happening

= 2014.11.11 =
* Bug fix

= 2014.11.10 =
* DO NOT UPDATE UNLESS YOUR RUNNING TAVE 4 AS THIS WILL BREAK T3
* set CURLOPT_FOLLOWLOCATION => true in anticipation of Táve 4 (sorry to those with safe_mode turned on).
* Changed the endpoint for the lead for t4 updates

= 2014.07.17 =
* Corrected code for changes in Contact Form 7. CF7 3.9 now works with this plugin.

= 2014.03.10 =
* Fixed an incorrect comparison for the check boxes in the admin. now if you check them they will function as expected.

= 2014.03.10 =
* Feature: Added another checkbox to disable the email sent from Táve.
* Settings update message added to the admin/settings page.
* More code comments, and stuff that doesn't need to be mentioned here but is.

= 2014.02.26 =
* Feature: added a checkbox to choose if you want the contact form 7 form to be emailed to you, or only receive the Táve form. (Thanks Shay Nartker)
* Updates to FAQ
* Small code cleanup and layout adjustments to the options page.

= 2014.02.24 = 
* set CURLOPT_FOLLOWLOCATION => false, it conflicts with users who have safe_mode turned on. (Thanks Carston Leishman)

= 2012.03.06 =
* Spelling Corrections
* extra lines for debugging no working changes

= 2011.06.02 =
* Initial release

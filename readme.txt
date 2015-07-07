=== Woocommerce Abandoned Cart Lite ===
Contributors: ashokrane, pinal.shah, mansishah, dharakothari
Tags: abandon cart, shopping cart abandonment
Requires at least: 1.3
Tested up to: 4.2.2
Stable tag: trunk
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html
Donate link: http://www.tychesoftwares.com/

This easy-to-use plugin gives store owners the ability to recover sales that are lost to abandoned shopping carts by logged-in customers. 

== Description ==

Abandoned Cart plugin works in the background, sending email notifications to your customers, reminding them about their abandoned orders.

The Abandoned Cart plugin allows you to recover orders that were just a step away from closing. It enables you to create automatic & well-timed email reminders to be sent to your customers who have added your products to their cart, but did not complete the order. As a result, with this plugin you will start recovering at least 30% or more of your lost sales. Why let this 30% revenue go unclaimed?

Abandoned Cart plugin enables Customers to:
<ol>
<li>Recover their abandoned carts in a single click</li>
<li>Automatically logs in registered customers</li>
</ol>

Abandoned Cart plugin enables Admin to:
<ol>
<li>Identify the Abandoned Orders information, including the products that were abandoned</li>
<li>Offer incentives to customers to return and complete their checkout with discounts and coupons.</li>
<li>Create unlimited email templates to be sent at intervals that you set</li>
<li>Add custom variables like Customer Name, Product Information, Coupons, etc. in the email template</li>
<li>Embed Woocommerce coupons in the emails being sent to customers</li>
<li>Copy HTML from anywhere & create templates using the powerful Rich Text Editor</li>
<li>Track whether expired coupons are causing cart abandonment</li>
<li>You are notified by email when an order is recovered</li>
<li>Track abandoned orders value v/s recovered orders value</li>
<li>Track emails sent, emails opened, links clicked for each template/email</li>
<li>Automatically stops email notifications when a customer makes a purchase or uses the cart recovery link</li>
</ol>

Note: Some features are available in the PRO version only.

**Pro Version:**

**[WooCommerce Abandoned Cart Pro 2.3.8](http://www.tychesoftwares.com/store/premium-plugins/woocommerce-abandoned-cart-pro "WooCommerce Abandoned Cart Pro")** - The PRO version allows you to track products in abandoned carts, create unlimited email templates, track coupons, keep a track of sent emails & much more.


**Email Sending Setup:**

From version 1.3, it is not mandatory to set a cron job via CPanel for the abandoned cart email notifications to be sent. We are now using WP-Cron that sends the emails automatically whenever a page is requested.

Abandoned Cart Plugin relies on a function called WP-Cron, and this function only runs when there is a page requested. So, if there are no visits to your website, then the scheduled jobs are not run. Generally this method of sending the abandoned cart notification emails is reliable. However, if you are not very confident about the traffic volume of your website, then you can set a manual cron job via Cpanel or any other control panel that your host provides. 

== Installation ==

1. Ensure you have latest version of Woocommerce plugin installed
2. Unzip and upload contents of the plugin to your /wp-content/plugins/ directory
3. Activate the plugin through the 'Plugins' menu in WordPress
4. The plugin will start working as per the settings entered.


== Frequently Asked Questions ==

= Can the plugin track carts abandoned by guest users? =

Currently there is no provision for tracking guest carts. This is planned in a future release.

= Why are abandoned cart notification emails not getting sent? =

Please ensure you have followed the instructions in "Email Sending Setup" right above this FAQ. Additionally, if you have the PRO version, please verify that you have selected "Enable abandoned cart notifications" option in Settings. With this option turned off, the abandoned carts are recorded, but emails are not sent.

== Screenshots ==

1. Lists all Abandoned Orders.

2. Lists all email templates.

3. Abandoned Cart Settings.

4. Lists Recovered Orders.

== Changelog ==

= 1.7 =
* Merge fields like {{products.cart}}, {{customer.firstname}}, etc. will be replaced with dummy data in the test emails that are sent from the template add / edit page. This ensures that you get a very close approximation of the actual email that will be delivered to your customers.
* Product image size in the abandon cart notification emails is set to a fixed height & width now.
* On WordPress Multisite, incorrect table prefix was used due to which the plugin was not functioning correctly on multisite installs. This is fixed now.

= 1.6 = 
* We have included .po, .pot and .mo files in the plugin. The plugin strings can now be translated to any language using these files.

= 1.5 =
* A shortcode {{products.cart}} can now be added in the abandoned cart notification emails. It will add the product information in the email like Product image, Product name, Quantity, Price & Total. The shortcode needs to be added from the AC menu from the template editor.
* The default value of the field "Cart abandoned cut-off time" in Settings tab was blank when the plugin is installed. This is now set to 60 minutes upon plugin activation.

= 1.4 =
* The abandoned cart emails were being sent multiple times for a single email template due to a bug. This is fixed.
* The plugin will now work on WordPress Multisite too.

= 1.3 =
* The abandoned cart email notifications are now sent out automatically without the necessity of having to set up a cron job manually.

= 1.2 =
* The test emails were not getting sent.
* Warnings fixed for some of the plugin setting pages.
* The image urls in the email were coming broken, this is fixed.

= 1.1 =
* Compatibility with WooCommerce 2.x versions
* Fixed 404 errors with images & other files

= 1.0 =
* Initial release.


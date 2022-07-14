Mod Monero for WooCommerce
==========================

This is a simple git repository containing a template which goes inside of [Monero Integrations MoneroWP](https://github.com/monero-integrations/monerowp) replacing their order template. My version works without Javascript and is tested. It simply uses HTML noscript tags containing echo statements that show the values inside several variables related to XMR orders. The change is very simple and does not effect the display for users using Javascript.

I have in my time passed on feature requests to the Monero integrations people to allow the checkout to work without Javascript. Strangely an option in the settings for the plugin exists to disable Javascript, but it stopped having an effect. I have finally decided to change that once and for all. My version changes only the template used to show orders, just replace theirs with mine.

You will see in this repo a file called order-page.php and it goes to the following location within Wordpress...

```/wp-content/plugins/monero-woocommerce-gateway/templates/monero-gateway/customer/order-page.php```

Once that is done the checkout will display enough information for users to pay XMR without Javascript and the changes were quite simple. It also still works with Javascript and uses AJAX updates.

If you install this template into the Monero gateway it will work without JS regardless of the option set in settings. While working on this I never noticed anything that would make that option work. They do not want you to have such an option because they know it appeals toward darkweb vending.

At some point the plugin did indeed work without JS and they got cold feet.

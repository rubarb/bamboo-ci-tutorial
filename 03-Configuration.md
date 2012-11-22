Configuring the Bamboo Sauce OnDemand plugin
=============

After the Sauce plugin has been installed, the username and access key of the Sauce OnDemand user account must be entered within the Bamboo administration interface.

To configure the authentication, click the `Administration` link.

![Admin](##admin.png##)

Click on the `Sauce OnDemand` link within the `Communication` section.

![Sauce Admin Link](##admin-sauce-link.png##)

This section contains the fields required to configure how the authentication for the Sauce plugin.  Enter the values of the username and access key you wish the Sauce plugin to use in the `Username` and `API Access Key fields`.

If the tests being executed will use Sauce Connect, then enter `localhost` and `4445` in the `Host` and `Port` fields.  If not, then enter `ondemand.saucelabs.com` and `4444` in the `Host` and `Port` fields.
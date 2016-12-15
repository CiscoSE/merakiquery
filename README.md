## merakiquery.py

####Description
This code will leverage python to query the Meraki Dashboard for information about the clients attached to the meraki cloud


####Configuraiton
All Configuration is done via the package_config.ini file.   This file currently has three configuration items:

* serveraddress - The IP or DNS name for the meraki dashboard.   This should normally be *dashboard.meraki.com*
* merakiAPIkey - This item is the meraki API Key.  Within the Meraki dashboard, select organization->settings and enable the "Dashboard API access"
* organization - This item is the organization id that the queries will be executed from.   You can leave this item blank the first time you run it, the application will display all the organization ids associated with the above merakiAPIkey

  
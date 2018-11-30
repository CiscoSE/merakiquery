# merakiquery.py

## Description
This code will leverage python to query the Meraki Dashboard for information about the clients attached to the Meraki cloud for a particular organization

## Requirements and Prerequisites

### Meraki API Access
For more information on the Meraki API, you can consult https://create.meraki.io/.   You will need to generate an API Key in your dashboard so that the information can be accessible from the calls to the API.

For more infomation on creating a API key, go to the following: https://documentation.meraki.com/zGeneral_Administration/Other_Topics/The_Cisco_Meraki_Dashboard_API

### package_config.ini
The code uses a file called the package_config.ini to house the information about the connection to meraki application uses.     In the repository, there is a ```package_config.ini.sample``` that you should rename to ```package_config.ini```.   Then modify the package_config.ini to reflect the following information

* serveraddress - The IP or DNS name for the meraki dashboard.   This should normally be *dashboard.meraki.com*
* merakiAPIkey - This item is the meraki API Key.  Within the Meraki dashboard, select organization->settings and enable the "Dashboard API access"
* organization - This item is the organization id that the queries will be executed from.   You can leave this item blank the first time you run it, the application will display all the organization ids associated with the above merakiAPIkey

### python
This demo example is based on Python 2.7 and was tested successfully under that version.

There are two main requirements for external libraries:
* requests
* configparser

You can install these prerequisites by the following commands:
```
pip install requests
pip install configparser
```
  
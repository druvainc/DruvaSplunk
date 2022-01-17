# OVERVIEW



# REQUIREMENTS

* Druva Add-on For Splunk
* Splunk version 7.x.x 
* This application should be installed on Search Head.

# Release Notes

* Version: 1.0.1
  * Fixed eventtype extraction issue

# RECOMMENDED SYSTEM CONFIGURATION

* Standard Splunk configuration of Search Head.

# Test your Install
The main app dashboard can take some time before the data is returned which will populate some of the panels. A good test is to run following query

```search `druva_get_index` ```

If you don't see these sourcetypes, run following query to find out if any alert with egnyte was executed.

```index="_internal"```

# Support
Customers can file issues by sending emails to : splunk.support@druva.com
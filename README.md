# RSA SecurID

Tested RSA SecurID 8

This content pack provides

## Dashboard
* Authentication Failure view / count
* Authenticaiton Success view / count
* SecurID Appliances Authenticating view / count
* Authentication sources view / count
* Self Service User Audit view / count

## Includes

* RSA Syslog input
* Passcode Error Stream
* Critical Events Stream
* Lockout Events Stream
* Authentication Failed Stream
* Configuration Changes Stream


## Requirements

* SYSLOG from RSA to Graylog

Configure syslog on RSA to send to local Syslog.

SSH into RSA Appliance and edit /etc/syslog-ng/syslog-ng.conf

destination logserver { udp("xxx.xxx.xxx.xxx" port(xxx) time-zone(-00:00)); };

This will send the syslog information, using UTC as the timezone of the graylog server.

Then restart the service  /etc/init.d/syslog restart

*** Have to provide information regarding the sylog configuraiton regarding time and syslog-ng.

## Screenshots


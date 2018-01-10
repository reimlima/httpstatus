# httpstatus
--------------------------------------------------------------------------------

Simple "Check HTTP Status" for Monitoring purposes

# Notice
--------------------------------------------------------------------------------

* This script was tested and work well in Python 2.7.6

# Changelog
--------------------------------------------------------------------------------
* **10/01/2018 - v1**
First Stable Release

# How to use it
--------------------------------------------------------------------------------

Example:

```sh

# Usage

$ python httpstatus 
Error:
        Usage: httpstatus -u <url> -o <output type>
Example:
        httpstatus -u https://google.com -o nagios

Output Type Options: nagios, xml, json

# Nagios output

$ python httpstatus -u reinaldo.site -o nagios
HTTP OK: reinaldo.site 301 Found

# Json output

$ python httpstatus -u reinaldo.site -o json
{
        "httpstatus": {
                "timestamp": "1515606054",
                "exitmessage": "HTTP OK: reinaldo.site 301 Found"
        }
}

# XML output

$ python httpstatus -u reinaldo.site -o xml
<?xml version="1.0" encoding="UTF-8"?>
<httpstatus>
        <timestamp>1515606057</timestamp>
        <exitmessage>HTTP OK: reinaldo.site 301 Found</exitmessage>
</httpstatus>

```

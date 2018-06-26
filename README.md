## Exploit Demo for CVE-2017-5638

Completely based on https://github.com/piesecurity/apache-struts2-CVE-2017-5638

### Usage:
Pre-requisites: have python, docker, maven and a jdk installed

1. clone this repo
1. run mvn clean package in project root
1. run docker build -t hack \.
1. run docker run -d -p 8080:8080 hack
1. once container comes online - verify by running in browser

To begin testing RCE - run the exploit.py file. 

1. python exploit.py http://myserver:8080/orders/3 "CMD" 




README.txt - Rest Showcase Webapp

Rest Showcase is a simple example of REST app build with the REST plugin.

For more on getting started with Struts, see 

* http://cwiki.apache.org/WW/home.html

I18N:
=====
Please note that this project was created with the assumption that it will be run
in an environment where the default locale is set to English. This means that
the default messages defined in package.properties are in English. If the default
locale for your server is different, then rename package.properties to package_en.properties
and create a new package.properties with proper values for your default locale.

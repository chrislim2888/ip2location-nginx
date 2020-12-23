# IMPORTANT:
# THIS PROJECT WILL NO LONGER BE MAINTAINED. PLEASE VISIT https://github.com/ip2location/ip2location-nginx FOR THE LATEST UPDATE.

# IP2Location Nginx

IP2Location Nginx module enables user to easily perform client's IP to geographical location lookup by using IP2Location database.

Supported IPv4 and IPv6 address.

For more details, please visit:
[https://www.ip2location.com/developers/nginx](https://www.ip2location.com/developers/nginx)

# Installation
1. Download IP2location C library from https://www.ip2location.com/developers/c
2. Change the path to IP2Location library in "ngx_http_ip2location_module.c".
3. Re-compile Nginx from source to include this module. Add the below directive into the compile of Nginx:
   ./configure --add-module=/absolute/path/to/nginx-ip2location-1.0
4. make
5. make install


# Usage
Change your Nginx config file to include the 'ip2location_database' directive:

    ip2location_database /absolute/path/to/IP2LOCATION-LITE-DB1.BIN;


The following variables will be made available in Nginx:

    $ip2location_country_code
    $ip2location_country_name

# Sample BIN Databases
* Download free IP2Location LITE databases at [https://lite.ip2location.com](https://lite.ip2location.com)  
* Download IP2Location sample databases at [https://www.ip2location.com/developers](https://www.ip2location.com/developers)

# Support
Email: support@ip2location.com.  
URL: [https://www.ip2location.com](https://www.ip2location.com)


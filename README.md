# NGINX Proxy to subdomains
This is how to proxy requests to subdomains on the same server using nginx

## Requirements



 - Add the following to /etc/hosts (Reload not needed)
 
```bash
127.0.0.1       app1.localhost
127.0.0.1       app2.localhost
```
Where app1.localhost is the first server and app2.localhost is the second
as defined in `my_sites.conf` `server_name` directive.


 - Update `my_sites.conf` with the actual ip addresses and ports where they are actually running
 - Optionally add more headers!
 
     `...`
     
 - please add ssl
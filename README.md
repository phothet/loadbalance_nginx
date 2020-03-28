Nginx Loadbalancing

* 1 x loadbalancer
* 2 x nginx web servers

Update /etc/nginx/sites-enabled/default to enable an alias https://url/link to serve the contents under /var/www/html/test.
```
        location /link{
          alias /var/www/html/test/;
          autoindex on;
        }
```

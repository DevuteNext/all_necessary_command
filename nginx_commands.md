
# nginx codes/commands




## apache mod_rewrite alternative for nginx

apache mod_rewrite alternative.needed for sendy

```bash
location / {
        if (!-f $request_filename){
                rewrite ^/([a-zA-Z0-9-]+)$ /$1.php last;
        }
}

location /l/ {
        rewrite ^/l/([a-zA-Z0-9/]+)$ /l.php?i=$1 last;
}

location /t/ {
        rewrite ^/t/([a-zA-Z0-9/]+)$ /t.php?i=$1 last;
}

location /w/ {
        rewrite ^/w/([a-zA-Z0-9/]+)$ /w.php?i=$1 last;
}

location /unsubscribe/ {
        rewrite ^/unsubscribe/(.*)$ /unsubscribe.php?i=$1 last;
}

location /subscribe/ {
        rewrite ^/subscribe/(.*)$ /subscribe.php?i=$1 last;
}

location ~* \.(ico|css|js|gif|jpe?g|png)(\?[0-9]+)?$ {
        expires max;
        log_not_found off;
}
```
    
## Sendy install guide

https://vpsfix.com/5920/install-sendy-vps-virtualmin-nginx/
  

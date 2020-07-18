# nginx-brotli-pagespeed for ubuntu focal

[Learn more here about building and configuration](https://codefaq.org/server/how-to-install-pagespeed-brotli-php-7-4-2-http2-on-nginx-server-using-ubuntu/)


to configure pagespeed
---

sudo mkdir -p /var/ngx_pagespeed_cache  
sudo chown -R www-data:www-data /var/ngx_pagespeed_cache  

micro /etc/nginx/nginx.conf  

pagespeed on;  
pagespeed FileCachePath /var/ngx_pagespeed_cache;  

sudo service nginx restart  

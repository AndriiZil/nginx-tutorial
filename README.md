# NGINX Tutorial

1. Serving Static Files
2. Mime Types
3. Location Context
4. Rewrites & Redirects
5. Load Balancer

### We will be working with NGINX using Docker
```bash
  docker run --name my-nginx -d -p 8080:80 nginx
  
  docker exec -it my-nginx /bin/bash
```
- Configuration file `/etc/nginx/conf.d/default.conf`
- Bu default
```bash
  docker cp ./index.html my-nginx:/usr/share/nginx/html
```

### Copy conf file (from specific folder)
- Previously create website folder inside of docker NGINX container
```bash
  docker cp ./default.conf my-nginx:/etc/nginx/conf.d/default.conf
  
  docker cp ./index.html my-nginx:/usr/share/nginx/website
```
### Restart NGINX container
```bash
  docker restart my-nginx
```

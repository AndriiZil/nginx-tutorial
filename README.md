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
- Configuration file `/etc/nginx/nginx.conf`
### Copy conf file
```bash
  docker cp ./some_file CONTAINER:/work
```

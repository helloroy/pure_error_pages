![404 Not Found](https://raw.githubusercontent.com/helloroy/pure_error_pages/refs/heads/main/404_demo.png "404 Not Found")

## Clean, minimalist error pages for Nginx

### 1. Download conf file:
```
sudo mkdir -p /etc/nginx/snippets/ && \
sudo wget "https://raw.githubusercontent.com/helloroy/pure_error_pages/main/pure_error_pages.conf" \
     -O /etc/nginx/snippets/pure_error_pages.conf
```

### 2. Include to Nginx conf:
```
server {
    include snippets/pure_error_pages.conf;
}
```

### 3. Verify and apply:
```
sudo nginx -t && sudo systemctl reload nginx
```

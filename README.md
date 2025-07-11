# IS402.P21-Resource-Monitoring-App
  helm install my-monitoring-app oci://ghcr.io/tranchucthien/helm-charts/resource-monitoring-app --version 0.1.0
  
  docker run -dp 5000:5000 chucthien03/resource-monitoring-app
  sudo apt install nginx
  cd /etc/nginx/sites-available/
  sudo nano nginx.chucthien.id.vn # replace domain
  cd sites-enabled/
  sudo ln -s /etc/nginx/sites-available/nginx.chucthien.id.vn /etc/nginx/sites-enabled/
  sudo nginx -t
  sudo systemctl reload nginx


### Cert
  sudo apt install certbot python3-certbot-nginx -y
  sudo certbot --nginx -d nginx.chucthien.id.vn

free subdomain register

https://freedns.afraid.org/ 

add subdomain.

acepanel.subdomain.com a record server ip adress

jellyfin.subdomain.com a record server ip adress

install cloudpanel.
curl -sS https://dploy.cloudpanel.io/dploy -o /usr/local/bin/dploy; \
echo "8809e9eb63483487f16b0a2e4075a8b18350a02470405e2f786bf82fd7e5fb53 /usr/local/bin/dploy" | \
sha256sum -c && chmod +x /usr/local/bin/dploy

install nginx password.

sudo sh -c "echo -n 'admin:' >> /etc/nginx/.htpasswd"
sudo sh -c "openssl passwd -apr1 >> /etc/nginx/.htpasswd"
sudo nginx -t
sudo systemctl reload nginx

Cloud panel login

Sites to Add site to Create a reserve proxy

acepanel.subdomain.com  port http://local ip adress:8000

cloudpanel sites to acepanel.subdomain.com  Manage to VHOST

# HTTP Basic Authentication
  auth_basic "Restricted Access";
  auth_basic_user_file /etc/nginx/.htpasswd;


if ($schema != "https") {
rewrite ^ https://$host$request_uri permanent;
}

add code for this.
save 

SSL/TLS ACTION  New Let's Encrypt Certificate

Create and install

--------------------------------------------------------------------------------  


Here we got a free subdomain with cloud panel and redirected it with a reverse proxy. Then we got an SSL certificate. Now we will install Acestream.

 sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin

git clone https://github.com/blackcode06/acestream-scraper-arm64.git

cd acestream-scraper-arm64

unzip acestream-scraper_11.zip

cd acestream-scraper_11

docker compose up -d --build

okey docker install complate to web

https://acepanel.subdomain.com 

login to nginx username passwords

install Acestream Scraper panel

http://localhost ip:8080/ace/getstream?id=

ace engine http://acestream-engine:6878

okey panel.

jellyfin install to https://jellyfin.subdomain.com 

setup  to jellyfin. tv install m3u link download. 





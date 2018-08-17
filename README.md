Integration API for Instapage, DialogFlow and Odoo CRM

For Instapage:

docker build -t api:flask /root/docker-flask/integration-api/

docker run -d -p 5151:443 -v /root/docker-flask/docker-flask-master/integration-api/docker-volume/:/var/www/integration-api/docker-volume api:flask

For DialogFlow:

docker build -t api:flask /root/docker-integration/integration-api/

docker run -d -p 5252:443 -v /root/docker-integration/docker-flask-master/integration-api/docker-volume/:/var/www/integration-api/docker-volume api:flask

docker exec -it [image_id] bash# integration-api

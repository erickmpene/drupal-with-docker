![Capture d’écran 2023-09-24 210610](https://github.com/erickmpene/drupal-with-docker/assets/138575584/05726430-5d84-4329-a1e1-6750b789d085)

## How To Install Drupal with Docker Compose
Drupal is a content management system (CMS) written in PHP and distributed under the open-source GNU General Public License. 

You must install the latest version of Docker Compose.

##### I assume you already have the certificates for your domain related to your public IP address.

#### 1. Certificats
At the root, create the key folder
```sh
mkdir key
```
Copy your certificates to this folder
```sh
cp fullchain.pem ./key && cp privkey.pem ./key
```
You need to be sure that your certificates have been generated correctly and that they match the domain name and public IP address.

#### 2. adapt the nginx.conf file to your situation
#### 3. Run Docker compose 
In the root folder, run : 
```sh
docker compose up -d 
```
If everything is okay, you should connect via https to your site with the domain name related to the certificate

#### Enjoy d(-_-)b 

# path-based-webapp
Geo Redundant Path Based Routing

## Global = Behind CDN

## Commands For Main Server Farm
#!/bin/bash
sudo apt update -y
sudo apt install apache2 -y

## Commands for Images Server Farm
#!/bin/bash
sudo apt update -y
sudo apt install apache2 -y
echo "<html><h2>This is images farmed page</h2></html>" > images.html
sudo cp images.html /var/www/html/
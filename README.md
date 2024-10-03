# fix-wifi-ubuntu

If the wifi stops working on Ubuntu 20.04, 22.04 or 24.04 run in terminal:

sudo systemctl restart NetworkManager.service

ifconfing --> sign down the name of the network, like ipv6leakintrf0 and pvpnksintrf0

sudo ifconfig ipv6leakintrf0 down
sudo ifconfig pvpnksintrf0 down 
sudo ifconfig pvpnksintrf0 up
sudo ifconfig ipv6leakintrf0 up
sudo systemctl restart NetworkManager.service

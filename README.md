

Install 
```
sudo curl -fL -o /etc/systemd/system/dumb-home-sync.service https://raw.githubusercontent.com/johanneswuerbach/dumb-home/master/dumb-home-sync.service
sudo chmod 664 /etc/systemd/system/dumb-home-sync.service
sudo systemctl daemon-reload
sudo systemctl restart dumb-home-sync.service
```

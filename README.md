# ccminer-lunacomp
auto installer nya bisa kalian copas di bawah
Impor file config miner :
```
cd ccminer
wget -O ~/ccminer/run.sh https://raw.githubusercontent.com/lunacomp/ccminer-lunacomp/main/config-share && chmod +x run.sh
cd
curl -o start.sh -k https://raw.githubusercontent.com/lunacomp/ccminer-lunacomp/main/start.sh && chmod +x start.sh
````
Membuat mining autorun pada saat boot
```
nano /etc/systemd/system/ccminer.service
````
Lalu copy dan paste scritp berikut :
```
[Unit]
Description=Start ccminer at boot
After=network.target

[Service]
ExecStart=/root/start.sh
Restart=always
User=root

[Install]
WantedBy=multi-user.target
```
Kemudian aktifkan dan mulai layanan
```
systemctl enable ccminer.service
systemctl start ccminer.service
````

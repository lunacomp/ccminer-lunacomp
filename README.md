# ccminer-lunacomp
auto installer nya bisa kalian copas di bawah
Impor file config miner share:
```
cd ccminer
wget -O ~/ccminer/run.sh https://raw.githubusercontent.com/lunacomp/ccminer-lunacomp/main/config-share && chmod +x run.sh
cd
curl -o start.sh -k https://raw.githubusercontent.com/lunacomp/ccminer-lunacomp/main/start.sh && chmod +x start.sh
cd /etc/systemd/system
curl -o ccminer.service -k https://raw.githubusercontent.com/lunacomp/ccminer-lunacomp/main/ccminer.service && chmod +x ccminer.service
````
Config miner-solo sebagai berikut :
```
cd ccminer
wget -O ~/ccminer/run.sh https://raw.githubusercontent.com/lunacomp/ccminer-lunacomp/main/config-share](https://raw.githubusercontent.com/lunacomp/ccminer-lunacomp/main/config-solo && chmod +x run.sh
cd
curl -o start.sh -k https://raw.githubusercontent.com/lunacomp/ccminer-lunacomp/main/start.sh && chmod +x start.sh
```
Membuat mining autorun pada saat boot
Kemudian aktifkan dan mulai layanan
```
sudo systemctl daemon-reload
systemctl enable ccminer.service
systemctl start ccminer.service
````

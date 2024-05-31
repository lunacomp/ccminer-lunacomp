# ccminer-lunacomp
auto installer nya bisa kalian copas di bawah
Impor file config miner share:
```
cd ccminer
wget -O ~/ccminer/run.sh https://raw.githubusercontent.com/lunacomp/ccminer-lunacomp/main/config-share && chmod +x run.sh
cd
curl -o start.sh -k https://raw.githubusercontent.com/lunacomp/ccminer-lunacomp/main/start.sh && chmod +x start.sh
````
Config miner-solo sebagai berikut :
```
cd ccminer
wget -O ~/ccminer/run.sh https://raw.githubusercontent.com/lunacomp/ccminer-lunacomp/main/config-share](https://raw.githubusercontent.com/lunacomp/ccminer-lunacomp/main/config-solo && chmod +x run.sh
cd
curl -o start.sh -k https://raw.githubusercontent.com/lunacomp/ccminer-lunacomp/main/start.sh && chmod +x start.sh
```
# Cara otomatis Ganti Wallet
```
cd
curl -o ganti-wallet-pool -k https://raw.githubusercontent.com/lunacomp/ccminer-lunacomp/main/ganti-wallet-pool && chmod +x ganti-wallet-pool
```
Nantinya kalo mau ganti wallet tinggal ketikan perintah berikut
```
./ganti-wallet-pool
```

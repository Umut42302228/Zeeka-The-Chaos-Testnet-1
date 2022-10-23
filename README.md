<h1 align="center"> Zeeka Network | The Chaos Testnet 1 </h1>

![image](https://user-images.githubusercontent.com/101149671/196880084-be318e37-979b-4c9e-bb14-5765ddcfc901.png)


### [Zeeka Network Discord](https://discord.gg/TezxNjB8)

![image](https://user-images.githubusercontent.com/101149671/196889312-d1edc9bc-c0e3-4fd2-a3d1-15167c712dca.png)

 
## Gereksinimler:

 * Minimum sistem gereksinimleri;
```
 2 CPU
 4 RAM
```

## Kurulum
```
sudo su
```
```
sudo apt-get update && sudo apt-get upgrade
```
```
sudo apt install -y build-essential libssl-dev cmake
```
```
apt install screen
```

## Rust toolunu kuruyoruz:

 * Kurulum esnasında 1'i seçiyoruz.

```
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

![image](https://user-images.githubusercontent.com/101149671/196891892-ef3bb9b4-12f8-44fc-a062-7e008fa6c77a.png)


## Bazukayı yüklüyoruz:
```
apt install git
git clone https://github.com/zeeka-network/bazuka
```
```
source "$HOME/.cargo/env"
```
## path'ı kuruyoruz:
```
cd bazuka
cargo install --path .
```
## Burdan sonrası dikkatli okuyalım:

 * Bu kısımda SEED yazan kısma kurtarma kelimenizi yazacaksınız
 * Nodu taşımak isterseniz`SEED` ile nodu taşıyabilecek ve yeniden kurmak istediğiniz zaman kurabileceksiniz.

```
bazuka init --seed SEED --network chaos --node 127.0.0.1:8765
```

## Nodumuzu farklı screende çalıştıralım:

```
screen -S bazuka
```

 * Burada 2 kısım değiştirelecek external ip adresiniz ve discord isminiz.
 
```
bazuka node --listen 0.0.0.0:8765 \
--external "İp Adresiniz":8765 \
--network chaos --db ~/.bazuka-chaos \
--bootstrap 144.91.101.166:8765 \
--bootstrap 45.67.228.84:8765 \
--bootstrap 152.228.155.120:8765 \
--bootstrap 80.87.202.42:8765 \
--bootstrap 148.251.1.124:8765 \
--discord-handle "Discord"
```

## Çıktınız aşağıdaki gibi olmalı.

 
![image](https://user-images.githubusercontent.com/101149671/196894807-5a3b4890-b45c-46eb-9f5b-9c75be02c278.png)

## Zeeka hakkında:

  * [Explorer linki](http://152.228.155.120:8000/)
  * [Web Site](https://zeeka.network/)
  * [Twitter](https://twitter.com/ZeekaNetwork)

# Not: Alıntıdır.




# <h1 align="center"> Exorde </h1>


![image](https://user-images.githubusercontent.com/101149671/201298361-b48bc53b-7858-42c2-b6ab-5cf7270e3429.png)

<h1 align="center"> Selamlar, Coinlist tarafından desteklenen ExordeLabs testnet rehberi, aşağıda gerekli linkler ve rehber mevcut:
</h1>

### Linkler:

 * [Exorde Türkiye Kanalı](https://t.me/ExordeTurkish)
 * [Exorde Discord Kanalı](https://discord.gg/44KzbSWB)
 * [Sıralama](https://explorer.exorde.network/leaderboard) ve [Explorer](https://explorer.exorde.network/)
 * Video rehberi gün içinde gelecek
 * Sohbet ve sorular için [Discord](discord.gg/ruescommunity) ve [Telegram](https://t.me/RuesChat) kanallarımız

## NOT (ilk defa node kuranlar):

 * Bu nodeları bilgisayarınıza kurabilirisniz ancak tavsiye etmem asla
 * Sanal sunucu kullanıyoruz, ücretli/ücretsiz sunucular mevcut.
 * Discord kanalımda sunucu nedir, node nedir, nasıl bağlanılır bu 3 temel konu hakkında video ve makale mevcut
 * Bunları anladığınız anda tüm nodeları kendiniz kurabilirsiniz, sorularınız için discord kanalı mevcut.
 * Rehberler ve sorular için: [Discord kanalı](discord.gg/ruescommunity)

## Gerekli notlar:

 * Bugün node kuranlar Kasım 22'e kadar %5 fazla ödül alacak
 * Testnet Şubat ayına kadar sürecek. (ekibin söylediği)
 * Hala ağ stabil çalışmıyor "Please try restarting your application." gibi hatalar alırsanız endişe etmeyin, tekrar deneyin.
 * Skale Network'ü bilirsiniz, (BlockPI ile Klaynt gibi düşünebilirsiniz..) ona bağlı olduğu için tek tük hatalar olur.

## Sistem gereksinimi:

 * Net bilgi yok, kendim test ettim:

```
CPU : 2 cores
RAM: 4Gb
SSD: 20Gb
```
## Docker ve güncellemeler::

```
sudo apt update -y && sudo apt install apt-transport-https ca-certificates curl software-properties-common -y && curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add - && sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu focal stable" && sudo apt install docker-ce
```

## Screen:
```
sudo apt install -y build-essential libssl-dev libffi-dev git curl screen
```

## Git clone çekiyoruz
```
git clone https://github.com/exorde-labs/ExordeModuleCLI.git
```

## Burası uzun bir yükleme sürecek:
```
cd ExordeModuleCLI
docker build -t exorde-cli .
```

## Bir screen açıyoruz:
```
screen -S exorde
```

## Metamask yazdığım yere 0xli başlayan metamask adresi giriyoruz:

 * Testnet cüzdanı kullanın

```
docker run -it exorde-cli -m 0x98E7332289E131C489b7504ef40521daCC0D1DaE -l 2
```

## Ve gördüğünüz gibi çalışıyor:

 
 * [Notlar](https://github.com/ruesandora/ExordeLabs#gerekli-notlar) kısmında belirttiğim hatayı alırsanız tekrar denemekten başka çare yok.
 * Çalıştığı zaman ctrl a d ile çıkın ve dokunmayın, arada kontrol edersiniz.
 * Çalıştığını nasıl anlayacağız? Notlar kısmında ki hatayı vermeyip node calısıyorsa işlem tamamdır. 

![image](https://user-images.githubusercontent.com/101149671/201302924-3d6c7127-6343-47fc-853b-353715b3e018.png)


## Gerekli komutlar:

 * Screen açma:

```
screen -S screenadı
```

 * Screen içersine girme:

```
screen -r screenadı
```

 * Screenleri görme:

```
screen -ls
```

 * Screen silme:

```
screen -XS screenadı quit
```

 * Tüm screenleri silme:

```
pkill screen
```

## Böylede bir tokenomics var, detaylı incelemedim:

![image](https://user-images.githubusercontent.com/101149671/201303557-755bcdc8-47f6-4a3e-a1a1-941e62342a37.png)






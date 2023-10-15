## Description

![image](https://github.com/erenozdeN12/STEMCTF-23-WriteUps/assets/88983987/ffbe9344-e3be-4f8c-b6e6-3b797eaf7e90)

## Solution

Siteye ulaşıldığında, site bizi gece rüyaya girecek tarzdan bir tekerlemeyle karşılamaktadır.

![image](https://github.com/erenozdeN12/STEMCTF-23-WriteUps/assets/88983987/ffa8b48d-db34-418f-8649-f7df9402b389)

HTML kodları incelendiğinde "şuan için" yararsız bir Base32 kodu dışında hiçbir şeye rastlanmamaktadır.

![image](https://github.com/erenozdeN12/STEMCTF-23-WriteUps/assets/88983987/7aa690a3-c4de-46a1-b611-e23c2bedbffa)

![image](https://github.com/erenozdeN12/STEMCTF-23-WriteUps/assets/88983987/e01a1fce-48ed-4fd5-9868-c6d47aef2389)

Klasik enumeration işlemlerinden biri olan robots kontrolünü yapmak için "robots.txt" dosyası ziyaret edilir.

![image](https://github.com/erenozdeN12/STEMCTF-23-WriteUps/assets/88983987/74c38a30-2d0a-42f5-a6ef-0020bf664266)

Üç adet girdiyle karşılaşılır. İlgimizi çekmesi gereken nokta şu, 1. yazılı dizinde zaten bir Base32 kodu bulmuştuk.
Buda diğer dizinlerde de benzer bir kod bulabileceğimiz anlamına geliyor. İlk denemede mymap.xml dizinini ziyaret etmeyi denesekte başarısız oluyoruz.

![image](https://github.com/erenozdeN12/STEMCTF-23-WriteUps/assets/88983987/1702d167-35a1-4eac-8bff-c84bafbf601d)

Bu ipucundan ilerleyerek sitelerin normal durumlarda map'lerini tuttuğu dosya olan "sitemap.xml" dosyasını ziyaret ediyoruz.

![image](https://github.com/erenozdeN12/STEMCTF-23-WriteUps/assets/88983987/a4449393-9a9a-4be1-a332-28494e19a576)

Bulduğumuz Base32 kodunu not ediyoruz. Son olarak dns uç noktasını ziyaret etmeye çalışıyoruz ama başarısız oluyoruz. Dns ipucundan yola çıkarak subdomainin dns kayıtlarını kontrol ediyoruz.

![image](https://github.com/erenozdeN12/STEMCTF-23-WriteUps/assets/88983987/28235c77-392b-4f7e-8506-de7becc8d045)

Bulduğumuz 3 Base32 kodunu arka arkaya koyup decode ediyoruz.

![image](https://github.com/erenozdeN12/STEMCTF-23-WriteUps/assets/88983987/66e7e335-e250-4757-ac5a-c25d609064a8)

Bir kodlanmış değer ile daha karşılaşıyoruz... Base64'den decode ediyoruz.

![image](https://github.com/erenozdeN12/STEMCTF-23-WriteUps/assets/88983987/d4d8e404-457e-40f0-801b-71915fdb76e7)

Flag içerisindeki değeri de decode ediyoruz..

![image](https://github.com/erenozdeN12/STEMCTF-23-WriteUps/assets/88983987/1a9aa065-9f6c-473b-ac6f-7018e5a64ed4)

## Flag

STEMCTF{C0k_G1zLi_B4yRaK_D3m1}






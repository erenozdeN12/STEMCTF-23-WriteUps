## Description
![image](https://github.com/erenozdeN12/STEMCTF-23-WriteUps/assets/88983987/6ad22528-b2ed-46a0-8d53-86dadbfc08f6)

## Solution
Siteye girildiğinde aşağıdaki görüntü ile karşılaşılır.
![image](https://github.com/erenozdeN12/STEMCTF-23-WriteUps/assets/88983987/5fcdd12a-66b9-4d75-8ac0-b6be4ee2db4b)

Sol üstte "Besle Beni" tuşu ve onun altında "Şuana kadar 0 kez besledin." yazısı bulunmaktadır. Butona her tıklandığında değer 1 artmaktadır.

![image](https://github.com/erenozdeN12/STEMCTF-23-WriteUps/assets/88983987/910e3ef9-1e72-4f25-87df-13190fd160a9)

Subdomain isminden (kurabiye) yola çıkarak cookie'den şüphelenilir ve cookieler incelenir.

![image](https://github.com/erenozdeN12/STEMCTF-23-WriteUps/assets/88983987/9cd2e5b4-dc1e-4307-b6e5-6257f35e71ee)

"feedcount" adlı cookie değeri yüksek bir değerle değiştirilir.

![image](https://github.com/erenozdeN12/STEMCTF-23-WriteUps/assets/88983987/862e3025-7893-492f-bda0-cb49d6489313)

Sayfa yenilenir ve cookie değeri tekrardan kontrol edilir.

![image](https://github.com/erenozdeN12/STEMCTF-23-WriteUps/assets/88983987/43646ac1-e375-4f41-bf83-d3dd43c59b9d)

Çıkan değer manuel olarak veya "URL Decoder" araçları ile decode edilir.

![image](https://github.com/erenozdeN12/STEMCTF-23-WriteUps/assets/88983987/5852027d-fb30-450d-853b-4c5bcb9a80b1)

## Flag

STEMCTF{D0ydUm_Y3tH3r}

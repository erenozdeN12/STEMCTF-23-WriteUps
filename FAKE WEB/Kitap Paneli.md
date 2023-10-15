## Description
![image](https://github.com/erenozdeN12/STEMCTF-23-WriteUps/assets/88983987/485721d5-1663-4efc-abc9-3f97b6f3f9a9)

## Solution

İlgili siteye erişildiğinde aşağıdaki gibi bir input ekranı ile karşılaşılıyor.

![image](https://github.com/erenozdeN12/STEMCTF-23-WriteUps/assets/88983987/46a6d188-71a3-4a43-acfe-7aa402427bd8)

10 kez rastgele değerler girerek deneme yapıldığında aşağıdaki hata ile karşılaşılıyor.

![image](https://github.com/erenozdeN12/STEMCTF-23-WriteUps/assets/88983987/796ee427-c561-49ac-951d-7e14b090c30f)

SQL Komutu çalıştırmamız gerektiğini anlıyoruz. 

`SELECT * from secrets` komutunu çalıştırıyoruz. "secrets" CTF'lerde sık karşılaşılan bir tablo ismidir. Deneme yanılma yöntemi ile bulunabilir.

![image](https://github.com/erenozdeN12/STEMCTF-23-WriteUps/assets/88983987/0dfd65d3-bdb9-48ef-937e-e2a2136aae20)

## FLAG

STEMCTF{As1l4Nd1N_D0sTum}

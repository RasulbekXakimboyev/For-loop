## For tsikli bo'yicha amaliy masalalar (1-qism)

#### **Masala 1: 1 dan 10 gacha sonlarni chiqarish**

**Masala tavsifi:**

Bu masalada sizning vazifangiz `for` tsikli yordamida 1 dan boshlab 10 gacha bo'lgan barcha natural sonlarni ekranga chiqarishdir. Bu eng oddiy va asosiy tsikl masalalaridan biridir.

**Nima qilish kerak:**

1. `for` tsikli yordamida 1 dan 10 gacha bo'lgan sonlarni ketma-ket oling
2. Har bir sonni alohida qatorda ekranga chiqaring
3. Natijada barcha sonlar ketma-ketlikda ko'rinishi kerak

**Muhim eslatmalar:**

- 1 va 10 ham natijaga kiritilishi kerak
- Har bir son yangi qatorda chiqishi kerak
- `range()` funksiyasidan foydalanish mumkin

**Kutilayotgan natija:**
```
1 dan 10 gacha sonlar:
1
2
3
4
5
6
7
8
9
10
```

---

#### **Masala 2: Listdagi barcha ismlarni chiqarish**

**Masala tavsifi:**

Bu masalada sizga ismlar ro'yxati berilgan. Sizning vazifangiz bu ro'yxatdagi har bir ismni `for` tsikli yordamida ekranga chiqarishdir. Har bir ism uchun "Salom" so'zi bilan birga chiqarilishi kerak.

**Berilgan ma'lumotlar:**

```python
ismlar = ["Ali", "Vali", "Hasan", "Malika", "Zuhra"]
```

**Nima qilish kerak:**

1. `for` tsikli yordamida ro'yxatdagi har bir ismni oling
2. Har bir ism uchun "Salom, [ism]!" formatida matn tuzing
3. Har bir salomni alohida qatorda ekranga chiqaring
4. Boshida "Do'stlarim:" deb yozing

**Muhim eslatmalar:**

- Ro'yxatdagi barcha ismlar chiqarilishi kerak
- Har bir ism uchun alohida salom yozilishi kerak
- f-string yoki formatlash usullaridan foydalanish mumkin

**Kutilayotgan natija:**
```
Do'stlarim:
Salom, Ali!
Salom, Vali!
Salom, Hasan!
Salom, Malika!
Salom, Zuhra!
```

---

#### **Masala 3: 1 dan 100 gacha juft sonlarni topish**

**Masala tavsifi:**

Bu masalada sizning vazifangiz 1 dan boshlab 100 gacha bo'lgan barcha juft sonlarni topish va ekranga chiqarishdir. Juft sonlar — bu 2 ga qoldiqsiz bo'linadigan sonlar (2, 4, 6, 8, 10 va hokazo).

**Nima qilish kerak:**

1. 1 dan 100 gacha bo'lgan barcha sonlarni ko'rib chiqing
2. Har bir sonni tekshiring — u juft sonmi?
3. Agar son juft bo'lsa, uni ekranga chiqaring
4. Barcha juft sonlarni bir qatorda yoki alohida qatorlarda ko'rsating

**Muhim eslatmalar:**

- Juft sonni aniqlash uchun `%` (qoldiq) operatoridan foydalanish mumkin
- Juft son: `son % 2 == 0` sharti bajarilishi kerak
- `range()` funksiyasida qadam (step) parametridan ham foydalanish mumkin

**Kutilayotgan natija:**
```
1 dan 100 gacha juft sonlar:
2 4 6 8 10 12 14 16 18 20 22 24 26 28 30 32 34 36 38 40 42 44 46 48 50 52 54 56 58 60 62 64 66 68 70 72 74 76 78 80 82 84 86 88 90 92 94 96 98 100
```

---

#### **Masala 4: Sonlar yig'indisini hisoblash**

**Masala tavsifi:**

Bu masalada sizning vazifangiz 1 dan boshlab 50 gacha bo'lgan barcha natural sonlarning yig'indisini hisoblashdir. Ya'ni, 1 + 2 + 3 + 4 + ... + 50 qo'shilmalarining natijasini topishingiz kerak.

**Nima qilish kerak:**

1. Yig'indi uchun o'zgaruvchi yarating va uni 0 ga tenglang
2. `for` tsikli yordamida 1 dan 50 gacha bo'lgan har bir sonni oling
3. Har bir sonni yig'indiga qo'shing
4. Oxirida umumiy yig'indini ekranga chiqaring

**Muhim eslatmalar:**

- Yig'indi o'zgaruvchisini boshida 0 ga tenglang
- Har bir tsikl qadamida sonni yig'indiga qo'shing
- Oxirida natijani chiroyli formatda ko'rsating

**Kutilayotgan natija:**
```
1 + 2 + 3 + ... + 50 = 1275
```

---

#### **Masala 5: Matnning uzunligini topish**

**Masala tavsifi:**

Bu masalada sizning vazifangiz foydalanuvchidan matn olish va uning nechta belgidan iborat ekanligini aniqlashdir. Muhim shart shuki, `len()` funksiyasidan foydalanmasdan, `for` tsikli yordamida matn uzunligini hisoblashingiz kerak.

**Nima qilish kerak:**

1. Foydalanuvchidan `input()` funksiyasi yordamida matn so'rang
2. Matn uzunligini hisoblash uchun o'zgaruvchi yarating (boshlang'ich qiymati 0)
3. `for` tsikli yordamida matndagi har bir belgini ko'rib chiqing
4. Har bir belgi uchun hisoblagichni 1 ga oshiring
5. Oxirida matn uzunligini ekranga chiqaring

**Misol kiritish:**
```
Matn kiriting: Salom dunyo
```

**Muhim eslatmalar:**

- Bo'shliqlar ham belgi sifatida hisoblanadi
- Har bir belgi (harf, raqam, belgi, bo'shliq) uchun hisoblagich oshadi
- `len()` funksiyasidan foydalanmang — faqat `for` tsikli bilan

**Kutilayotgan natija:**
```
Matn uzunligi: 11 belgi
```

**Tushuntirish:** "Salom dunyo" matnida 5 harf + 1 bo'shliq + 5 harf = 11 belgi mavjud.

---

#### **Masala 6: 1–50 oralig'idagi 3 ga bo'linadigan sonlar**

**Masala tavsifi:**

Bu masalada sizning vazifangiz 1 dan boshlab 50 gacha bo'lgan barcha sonlarni ko'rib chiqib, ular orasidan 3 ga qoldiqsiz bo'linadigan sonlarni topish va chiqarishdir. Shuningdek, nechta bunday son borligini ham aniqlashingiz kerak.

**Nima qilish kerak:**

1. 1 dan 50 gacha bo'lgan barcha sonlarni ko'rib chiqing
2. Har bir sonni 3 ga bo'lib, qoldiqni tekshiring
3. Agar son 3 ga qoldiqsiz bo'linsa (qoldiq 0 bo'lsa), uni ekranga chiqaring
4. Barcha topilgan sonlarni sanang
5. Oxirida jami nechta son topilganini ko'rsating

**Muhim eslatmalar:**

- 3 ga bo'linadigan son: `son % 3 == 0` sharti bajarilishi kerak
- Sanoq o'zgaruvchisini boshida 0 ga tenglang
- Har bir topilgan son uchun sanoqni 1 ga oshiring

**Kutilayotgan natija:**
```
1 dan 50 gacha 3 ga bo'linadigan sonlar:
3 6 9 12 15 18 21 24 27 30 33 36 39 42 45 48

Jami: 16 ta son
```

---

#### **Masala 7: Matndan unli harflar sonini topish**

**Masala tavsifi:**

Bu masalada sizning vazifangiz foydalanuvchi kiritgan matndan unli harflarni topish va ularning sonini hisoblashdir. Unli harflar — lotin alifbosida: a, e, i, o, u; kirill alifbosida: а, е, ё, и, о, у, ы, э, ю, я.

**Nima qilish kerak:**

1. Foydalanuvchidan matn so'rang
2. Unli harflar ro'yxatini yarating
3. Hisoblagich o'zgaruvchisini yarating (boshlang'ich qiymati 0)
4. `for` tsikli yordamida matndagi har bir belgini ko'rib chiqing
5. Agar belgi unli harf bo'lsa, hisoblagichni 1 ga oshiring
6. Oxirida jami unli harflar sonini ekranga chiqaring

**Misol kiritish:**
```
Matn kiriting: Python dasturlash
```

**Muhim eslatmalar:**

- Bosh va kichik harflarni farqlash kerak emas (`.lower()` yoki `.upper()` dan foydalanish mumkin)
- Faqat unli harflar sanaladi, undosh harflar va boshqa belgilar sanalmaydi
- Bo'shliqlar va boshqa belgilar hisobga olinmaydi

**Kutilayotgan natija:**
```
Jami unli harflar: 4 ta
```

**Tushuntirish:** "Python dasturlash" matnida unli harflar: o, a, u, a — jami 4 ta.

---

#### **Masala 8: Listdagi eng katta sonni topish**

**Masala tavsifi:**

Bu masalada sizga sonlar ro'yxati berilgan. Sizning vazifangiz bu ro'yxatdagi eng katta sonni topishdir. Muhim shart shuki, `max()` funksiyasidan foydalanmasdan, `for` tsikli yordamida eng katta sonni topishingiz kerak.

**Berilgan ma'lumotlar:**

```python
sonlar = [23, 67, 12, 89, 45, 34, 91, 56, 78]
```

**Nima qilish kerak:**

1. Eng katta sonni saqlash uchun o'zgaruvchi yarating
2. Boshlang'ich qiymat sifatida ro'yxatdagi birinchi sonni oling
3. `for` tsikli yordamida ro'yxatdagi har bir sonni ko'rib chiqing
4. Agar joriy son eng katta sondan katta bo'lsa, uni yangi eng katta son qiling
5. Oxirida eng katta sonni ekranga chiqaring

**Muhim eslatmalar:**

- `max()` funksiyasidan foydalanmang
- Boshlang'ich qiymat sifatida ro'yxatdagi birinchi sonni olish mumkin
- Har bir sonni solishtirib, eng kattasini toping

**Kutilayotgan natija:**
```
Listdagi eng katta son: 91
```

---

#### **Masala 9: Sonning raqamlari yig'indisi**

**Masala tavsifi:**

Bu masalada sizning vazifangiz foydalanuvchi kiritgan sonning barcha raqamlarini ajratib olish va ularning yig'indisini hisoblashdir. Masalan, 1234 soni uchun: 1 + 2 + 3 + 4 = 10.

**Nima qilish kerak:**

1. Foydalanuvchidan son so'rang
2. Sonni matnga aylantiring (har bir raqamni ajratish uchun)
3. Yig'indi uchun o'zgaruvchi yarating (boshlang'ich qiymati 0)
4. `for` tsikli yordamida matndagi har bir raqamni oling
5. Har bir raqamni songa aylantirib, yig'indiga qo'shing
6. Oxirida sonning raqamlari yig'indisini ekranga chiqaring

**Misol kiritish:**
```
Son kiriting: 1234
```

**Muhim eslatmalar:**

- Sonni matnga aylantirish uchun `str()` funksiyasidan foydalanish mumkin
- Har bir raqamni songa aylantirish uchun `int()` funksiyasidan foydalanish mumkin
- Manfiy sonlar uchun ham ishlashi kerak (faqat raqamlarni hisobga oling)

**Kutilayotgan natija:**
```
1234 sonining raqamlari yig'indisi: 10
```

**Tushuntirish:** 1234 sonining raqamlari: 1, 2, 3, 4. Ularning yig'indisi: 1 + 2 + 3 + 4 = 10.

---

#### **Masala 10: Faktorial hisoblash**

**Masala tavsifi:**

Bu masalada sizning vazifangiz berilgan sonning faktorialini hisoblashdir. Faktorial — bu sonni 1 gacha bo'lgan barcha natural sonlarga ko'paytirishdir. Masalan, 5! (besh faktorial) = 5 × 4 × 3 × 2 × 1 = 120.

**Nima qilish kerak:**

1. Foydalanuvchidan son so'rang
2. Agar son manfiy bo'lsa, xabar chiqaring (faktorial manfiy sonlar uchun aniqlanmagan)
3. Agar son 0 yoki 1 bo'lsa, faktorial 1 ga teng
4. Agar son 1 dan katta bo'lsa, `for` tsikli yordamida 1 dan boshlab shu songacha bo'lgan barcha sonlarni ko'paytiring
5. Oxirida faktorial natijasini ekranga chiqaring

**Misol kiritish:**
```
Son kiriting: 5
```

**Muhim eslatmalar:**

- Faktorial uchun o'zgaruvchi yarating va uni 1 ga tenglang
- `for` tsikli yordamida 1 dan boshlab son gacha bo'lgan har bir sonni ko'paytiring
- 0! = 1 (maxsus holat)
- Manfiy sonlar uchun faktorial aniqlanmagan

**Kutilayotgan natija:**
```
5! = 120
```

**Eslatmalar:** 
- 0! = 1
- Manfiy sonlar uchun faktorial aniqlanmagan

---

#### **Masala 11: Multiplikatsiya jadvali (1–10)**

**Masala tavsifi:**

Bu masalada sizning vazifangiz 1 dan 10 gacha bo'lgan sonlar uchun to'liq multiplikatsiya (ko'paytirish) jadvalini yaratishdir. Jadval 10×10 formatida bo'lishi kerak, ya'ni har bir son (1 dan 10 gacha) boshqa har bir songa ko'paytiriladi va natijalar chiroyli formatda ko'rsatiladi.

**Nima qilish kerak:**

1. Jadval sarlavhasini chiqaring
2. Ustun sarlavhalarini chiqaring (1 dan 10 gacha)
3. Ichma-ich `for` tsiklidan foydalaning:
   - Tashqi tsikl — satrlar uchun (1 dan 10 gacha)
   - Ichki tsikl — ustunlar uchun (1 dan 10 gacha)
4. Har bir katakda satr va ustun sonlarini ko'paytiring
5. Natijalarni chiroyli formatda (bir xil kenglikda) chiqaring

**Muhim eslatmalar:**

- Ichma-ich tsikl (nested loop) ishlatishingiz kerak
- Har bir sonni bir xil kenglikda ko'rsatish uchun formatlashdan foydalaning
- Jadval chiroyli va tushunarli ko'rinishda bo'lishi kerak

**Kutilayotgan natija:**
```
MULTIPLIKATSIYA JADVALI
============================================================
   |    1    2    3    4    5    6    7    8    9   10
————————————————————————————————————————————————————————————
 1 |    1    2    3    4    5    6    7    8    9   10
 2 |    2    4    6    8   10   12   14   16   18   20
 3 |    3    6    9   12   15   18   21   24   27   30
 4 |    4    8   12   16   20   24   28   32   36   40
 5 |    5   10   15   20   25   30   35   40   45   50
 6 |    6   12   18   24   30   36   42   48   54   60
 7 |    7   14   21   28   35   42   49   56   63   70
 8 |    8   16   24   32   40   48   56   64   72   80
 9 |    9   18   27   36   45   54   63   72   81   90
10 |   10   20   30   40   50   60   70   80   90  100
```

---

#### **Masala 12: Yulduzchalar bilan piramida**

**Masala tavsifi:**

Bu masalada sizning vazifangiz foydalanuvchi kiritgan balandlikda yulduzchalar (*) yordamida piramida chizishdir. Piramida markazlashgan bo'lishi kerak, ya'ni har bir qatorda yulduzchalar oldida bo'sh joylar bo'lishi kerak.

**Nima qilish kerak:**

1. Foydalanuvchidan piramida balandligini so'rang
2. Har bir qator uchun:
   - Avval bo'sh joylarni chiqaring (markazlash uchun)
   - Keyin yulduzchalarni chiqaring
3. Birinchi qatorda 1 ta yulduz, ikkinchi qatorda 3 ta, uchinchi qatorda 5 ta va hokazo bo'lishi kerak
4. Har bir qatordan keyin yangi qatorga o'ting

**Misol kiritish:**
```
Piramida balandligi: 5
```

**Muhim eslatmalar:**

- Har bir qatordagi yulduzchalar soni: 2 × qator_raqami - 1
- Har bir qatordagi bo'sh joylar soni: balandlik - qator_raqami
- Ichma-ich tsikl ishlatishingiz kerak (bo'sh joylar uchun va yulduzchalar uchun)

**Kutilayotgan natija:**
```
⭐ YULDUZLI PIRAMIDA ⭐

    *
   ***
  *****
 *******
*********
```

**Tushuntirish:** 
- 1-qator: 4 bo'sh joy + 1 yulduz
- 2-qator: 3 bo'sh joy + 3 yulduz
- 3-qator: 2 bo'sh joy + 5 yulduz
- 4-qator: 1 bo'sh joy + 7 yulduz
- 5-qator: 0 bo'sh joy + 9 yulduz

---

#### **Masala 13: Fibonachchining dastlabki 10 ta soni**

**Masala tavsifi:**

Bu masalada sizning vazifangiz Fibonachchi ketma-ketligining birinchi 10 ta sonini chiqarishdir. Fibonachchi ketma-ketligi — bu har bir son oldingi ikkita sonning yig'indisiga teng bo'lgan ketma-ketlikdir. Ketma-ketlik 0 va 1 dan boshlanadi.

**Fibonachchi ketma-ketligi qoidasi:**

- F(0) = 0
- F(1) = 1
- F(n) = F(n-1) + F(n-2) (n ≥ 2 uchun)

**Nima qilish kerak:**

1. Dastlabki ikkita sonni belgilang: a = 0, b = 1
2. 10 marta takrorlanadigan `for` tsikli yarating
3. Har bir tsikl qadamida:
   - Joriy sonni (a) ekranga chiqaring
   - Keyingi sonni hisoblang: yangi_a = b, yangi_b = a + b
   - a va b ni yangilang
4. Oxirida barcha sonlarni bir qatorda ko'rsating

**Muhim eslatmalar:**

- Birinchi son 0, ikkinchi son 1
- Har bir keyingi son oldingi ikkitasining yig'indisi
- Python'da `a, b = b, a + b` yozuvi qisqa va qulay

**Kutilayotgan natija:**
```
Fibonachchining birinchi 10 ta soni:
0 1 1 2 3 5 8 13 21 34
```

**Tushuntirish:** 
- 0 (boshlang'ich)
- 1 (boshlang'ich)
- 1 (0 + 1)
- 2 (1 + 1)
- 3 (1 + 2)
- 5 (2 + 3)
- 8 (3 + 5)
- 13 (5 + 8)
- 21 (8 + 13)
- 34 (13 + 21)

---

#### **Masala 14: Tub sonlarni topish**

**Masala tavsifi:**

Bu masalada sizning vazifangiz 1 dan boshlab 100 gacha bo'lgan barcha tub sonlarni topish va chiqarishdir. Tub son — bu faqat 1 ga va o'ziga bo'linadigan son. Masalan, 2, 3, 5, 7, 11, 13 va hokazo tub sonlardir.

**Tub son nima?**

Tub son — bu 1 dan katta va faqat ikkita bo'luvchiga ega bo'lgan son: 1 va o'zi. Masalan:
- 2 — tub son (faqat 1 va 2 ga bo'linadi)
- 3 — tub son (faqat 1 va 3 ga bo'linadi)
- 4 — tub emas (1, 2, 4 ga bo'linadi)
- 5 — tub son (faqat 1 va 5 ga bo'linadi)

**Nima qilish kerak:**

1. 2 dan boshlab 100 gacha bo'lgan har bir sonni ko'rib chiqing (1 tub son emas)
2. Har bir son uchun uning tub ekanligini tekshiring:
   - 2 dan boshlab (son - 1) gacha bo'lgan barcha sonlarga bo'lib ko'ring
   - Agar hech bo'lmaganda bitta songa qoldiqsiz bo'linsa, demak tub emas
   - Agar hech bir songa bo'linmasa, demak tub son
3. Agar son tub bo'lsa, uni ekranga chiqaring yoki ro'yxatga qo'shing
4. Oxirida barcha tub sonlarni va ularning sonini ko'rsating

**Muhim eslatmalar:**

- 1 tub son emas (maxsus holat)
- 2 dan boshlash kerak
- Har bir sonni 2 dan (son - 1) gacha bo'lgan sonlarga bo'lib ko'rish kerak
- Agar biror songa bo'linsa, `break` yordamida tsiklni to'xtatish mumkin

**Kutilayotgan natija:**
```
1 dan 100 gacha tub sonlar:
2 3 5 7 11 13 17 19 23 29 31 37 41 43 47 53 59 61 67 71 73 79 83 89 97

Jami: 25 ta tub son
```

---

#### **Masala 15: Raqamli soat simulyatori**

**Masala tavsifi:**

Bu masalada sizning vazifangiz raqamli soat simulyatorini yaratishdir. Dastur 00:00:00 (yarim tun) dan boshlab 23:59:59 (tun yarimdan bir soniya oldin) gacha bo'lgan barcha vaqtlarni ko'rsatishi kerak. Har bir vaqt soat:daqiqa:sekund formatida bo'lishi kerak.

**Nima qilish kerak:**

1. Ichma-ich uchta `for` tsikli yarating:
   - Birinchi tsikl — soatlar uchun (0 dan 23 gacha)
   - Ikkinchi tsikl — daqiqalar uchun (0 dan 59 gacha)
   - Uchinchi tsikl — sekundlar uchun (0 dan 59 gacha)
2. Har bir kombinatsiya uchun vaqtni formatlang (masalan, 05:03:07)
3. Har bir vaqtni ekranga chiqaring
4. Oxirida jami nechta vaqt ko'rsatilganini hisoblang va chiqaring

**Muhim eslatmalar:**

- Soatlar: 0 dan 23 gacha (jami 24 ta)
- Daqiqalar: 0 dan 59 gacha (jami 60 ta)
- Sekundlar: 0 dan 59 gacha (jami 60 ta)
- Vaqtni chiroyli formatda ko'rsatish uchun 2 xonali formatdan foydalaning (masalan, 05, 03, 07)
- Jami vaqtlar soni: 24 × 60 × 60 = 86,400 ta

**Kutilayotgan natija:**
```
RAQAMLI SOAT SIMULYATORI
========================================
00:00:00
00:00:01
00:00:02
00:00:03
...
23:59:57
23:59:58
23:59:59

Jami: 86400 ta vaqt
```

**Eslatma:** Bir kunda jami 24 × 60 × 60 = 86,400 ta vaqt mavjud (har bir sekund uchun alohida vaqt).

---

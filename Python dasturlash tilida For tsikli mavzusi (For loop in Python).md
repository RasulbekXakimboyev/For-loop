## For tsikli bo'yicha amaliy masalalar (2-qism)

#### Masala 1: 1 dan 10 gacha sonlarni chiqarish

**Tavsif:** Sizning vazifangiz 1 dan boshlab 10 gacha bo'lgan barcha natural sonlarni ekranga chiqarishdir. Buning uchun for tsikli va range() funksiyasidan foydalaning. Sonlar bir qatorda, bir-biridan bo'sh joy bilan ajratilgan holda chiqarilishi kerak. Masalan, 1, keyin bo'sh joy, keyin 2, keyin bo'sh joy va hokazo. Oxirgi son 10 bo'lishi kerak.

**Kutilayotgan natija:**
```
1 2 3 4 5 6 7 8 9 10
```

---

#### Masala 2: Matndagi harflarni chiqarish

**Tavsif:** Sizga "Python" so'zi berilgan. Sizning vazifangiz bu so'zdagi har bir harfni alohida qatorda chiqarishdir. Har bir harf oldida tire belgisi (-) va bo'sh joy bo'lishi kerak. Masalan, birinchi qatorda "  - P", ikkinchi qatorda "  - y" va hokazo chiqarilishi kerak. Buning uchun for tsikli yordamida matndagi har bir belgini takrorlang va har birini alohida qatorda ko'rsating.

**Kutilayotgan natija:**
```
  - P
  - y
  - t
  - h
  - o
  - n
```

---

#### Masala 3: Listdagi ismlarni chiqarish

**Tavsif:** Sizga ismlar ro'yxati berilgan. Sizning vazifangiz bu ro'yxatdagi har bir ismni tartib raqami bilan chiqarishdir. Birinchi ism 1-raqam bilan, ikkinchi ism 2-raqam bilan va hokazo ko'rsatilishi kerak. Har bir ism alohida qatorda, raqam va nuqta (.) belgisi bilan chiqarilishi kerak. Masalan, "1. Ali", "2. Vali" va hokazo. Buning uchun for tsikli va enumerate() funksiyasidan foydalanishingiz mumkin.

**Berilgan ma'lumotlar:**
```python
ismlar = ["Ali", "Vali", "Dilnoza", "Madina", "Sobir"]
```

**Kutilayotgan natija:**
```
1. Ali
2. Vali
3. Dilnoza
4. Madina
5. Sobir
```

---

#### Masala 4: Juft sonlarni topish

**Tavsif:** Sizning vazifangiz 1 dan boshlab 20 gacha bo'lgan barcha juft sonlarni topish va ekranga chiqarishdir. Juft son deb 2 ga qoldiqsiz bo'linadigan sonlarga aytiladi. Buning uchun for tsikli yordamida 1 dan 20 gacha bo'lgan barcha sonlarni ko'rib chiqing va har bir sonni 2 ga bo'lganda qoldiq 0 bo'lsa (ya'ni son % 2 == 0), bu sonni chiqaring. Barcha juft sonlar bir qatorda, bir-biridan bo'sh joy bilan ajratilgan holda chiqarilishi kerak.

**Kutilayotgan natija:**
```
2 4 6 8 10 12 14 16 18 20
```

---

#### Masala 5: 1 dan n gacha sonlar yig'indisi

**Tavsif:** Sizning vazifangiz 1 dan boshlab 50 gacha bo'lgan barcha natural sonlarning yig'indisini hisoblashdir. Buning uchun avval yig'indi o'zgaruvchisini 0 ga tenglashtiring. Keyin for tsikli yordamida 1 dan 50 gacha bo'lgan har bir sonni yig'indiga qo'shing. Oxirida natijani ekranga chiqaring. Masalan, 1 + 2 + 3 + ... + 50 = 1275 bo'lishi kerak. Natija quyidagi formatda chiqarilishi kerak: "1 dan 50 gacha yig'indi: 1275".

**Kutilayotgan natija:**
```
1 dan 50 gacha yig'indi: 1275
```

---

#### Masala 6: 1-100 oralig'ida 3 ga bo'linadigan sonlar

**Tavsif:** Sizning vazifangiz 1 dan boshlab 100 gacha bo'lgan barcha sonlar orasidan 3 ga qoldiqsiz bo'linadigan sonlarni topish va ularning umumiy sonini hisoblashdir. Buning uchun for tsikli yordamida 1 dan 100 gacha bo'lgan har bir sonni ko'rib chiqing. Agar son 3 ga bo'lganda qoldiq 0 bo'lsa (ya'ni son % 3 == 0), bu sonni chiqaring va sanagichni birga oshiring. Barcha topilgan sonlar bir qatorda, bir-biridan bo'sh joy bilan ajratilgan holda chiqarilishi kerak. Oxirida yangi qatorda jami nechta son topilganini ko'rsating. Masalan, "Jami: 33 ta son topildi".

**Kutilayotgan natija:**
```
3 6 9 12 15 18 21 24 27 30 33 36 39 42 45 48 51 54 57 60 63 66 69 72 75 78 81 84 87 90 93 96 99

Jami: 33 ta son topildi
```

---

#### Masala 7: Unli harflarni sanash

**Tavsif:** Sizga matn berilgan. Sizning vazifangiz bu matndagi unli harflar sonini aniqlashdir. Unli harflar deb quyidagi harflarga aytiladi: a, e, i, o, u (kichik va katta harflar). Buning uchun avval unli harflar to'plamini yarating. Keyin for tsikli yordamida matndagi har bir belgini ko'rib chiqing. Agar belgi unli harf bo'lsa, sanagichni birga oshiring. Oxirida asl matnni va unli harflar sonini ekranga chiqaring. E'tibor bering, katta va kichik harflar farqi yo'q, ikkalasi ham hisobga olinishi kerak.

**Berilgan ma'lumotlar:**
```python
matn = "Python dasturlash juda qiziqarli va foydali"
```

**Kutilayotgan natija:**
```
Matn: Python dasturlash juda qiziqarli va foydali
Unli harflar soni: 14
```

---

#### Masala 8: Eng katta elementni topish

**Tavsif:** Sizga sonlar ro'yxati berilgan. Sizning vazifangiz bu ro'yxatdagi eng katta sonni topishdir. Buning uchun for tsikli yordamida ro'yxatdagi har bir sonni ko'rib chiqing. Avval eng katta son sifatida ro'yxatdagi birinchi sonni oling. Keyin for tsikli yordamida qolgan barcha sonlarni tekshiring. Agar joriy son eng katta sondan katta bo'lsa, eng katta sonni yangilang. Oxirida topilgan eng katta sonni ekranga chiqaring. Eslatma: max() funksiyasidan foydalanmang, faqat for tsikli va taqqoslash operatorlaridan foydalaning.

**Berilgan ma'lumotlar:**
```python
sonlar = [45, 12, 89, 34, 67, 23, 91, 56, 78]
```

**Kutilayotgan natija:**
```
Eng katta son: 91
```

---

#### Masala 9: Yig'indi, maksimum, minimum

**Tavsif:** Sizga sonlar ro'yxati berilgan. Sizning vazifangiz bu ro'yxatdagi barcha sonlarning yig'indisini, eng katta sonini (maksimum), eng kichik sonini (minimum) va o'rtacha qiymatini topishdir. Buning uchun for tsikli yordamida ro'yxatdagi har bir sonni ko'rib chiqing. Har bir iteratsiyada sonni yig'indiga qo'shing, agar son maksimumdan katta bo'lsa maksimumni yangilang, agar son minimumdan kichik bo'lsa minimumni yangilang. Oxirida o'rtacha qiymatni yig'indini sonlar soniga bo'lish orqali hisoblang. Barcha natijalarni ekranga chiqaring. Eslatma: sum(), max(), min() funksiyalaridan foydalanmang, faqat for tsikli va asosiy amallardan foydalaning.

**Berilgan ma'lumotlar:**
```python
sonlar = [34, 12, 89, 5, 67, 23, 91, 45]
```

**Kutilayotgan natija:**
```
Sonlar: [34, 12, 89, 5, 67, 23, 91, 45]
Yig'indi: 366
Maksimum: 91
Minimum: 5
O'rtacha: 45.75
```

---

#### Masala 10: Matnni teskari o'qish

**Tavsif:** Sizga matn berilgan. Sizning vazifangiz bu matnni teskari tartibda chiqarishdir. Masalan, "Python" so'zi "nohtyP" ko'rinishida chiqarilishi kerak. Buning uchun for tsikli yordamida matndagi har bir harfni ko'rib chiqing va har bir harfni yangi matnning boshiga qo'shing. Avval bo'sh matn yarating. Keyin for tsikli yordamida har bir harfni oling va uni mavjud matnning boshiga qo'shing. Oxirida asl matnni va teskari matnni ekranga chiqaring. Eslatma: reversed() funksiyasidan yoki [::-1] slice notatsiyasidan foydalanmang, faqat for tsikli va string qo'shish amalidan foydalaning.

**Berilgan ma'lumotlar:**
```python
matn = "Python"
```

**Kutilayotgan natija:**
```
Asl matn: Python
Teskari: nohtyP
```

---

#### Masala 11: Multiplikatsiya jadvali 1-10

**Tavsif:** Sizning vazifangiz 1 dan 10 gacha bo'lgan barcha sonlarning to'liq ko'paytirish jadvalini yaratishdir. Buning uchun ichma-ich for tsikllardan foydalaning. Tashqi tsikl 1 dan 10 gacha bo'lgan sonlar uchun, ichki tsikl esa har bir son uchun 1 dan 10 gacha bo'lgan sonlar bilan ko'paytirish uchun. Avval jadval sarlavhasini chiqaring. Keyin har bir son uchun (masalan, 1, keyin 2 va hokazo) uning ko'paytirish jadvalini chiqaring. Har bir ko'paytma quyidagi formatda bo'lishi kerak: "  1 ×  2 =   2" (sonlar o'ngdan tekislangan). Har bir sonning jadvali alohida bo'lim sifatida ko'rsatilishi kerak.

**Kutilayotgan natija:**
```
======================================================================
           TO'LIQ KO'PAYTIRISH JADVALI (1-10)
======================================================================

1 ning jadvali:
------------------------------
  1 ×  1 =   1
  1 ×  2 =   2
  1 ×  3 =   3
  ...
  1 × 10 =  10

2 ning jadvali:
------------------------------
  2 ×  1 =   2
  2 ×  2 =   4
  ...
  (va hokazo 10 gacha)
```

---

#### Masala 12: Yulduzcha piramida

**Tavsif:** Sizning vazifangiz yulduzcha (*) belgisidan piramida shakli yaratishdir. Piramida 7 qatordan iborat bo'lishi kerak. Birinchi qatorda 1 ta yulduzcha, ikkinchi qatorda 3 ta, uchinchi qatorda 5 ta va hokazo bo'lishi kerak. Har bir qatordagi yulduzchalar soni 2×qator_raqami - 1 formula bilan hisoblanadi. Yulduzchalar markazda joylashgan bo'lishi kerak, ya'ni har bir qatorda chapdan bo'sh joylar bo'lishi kerak. Bo'sh joylar soni piramida balandligi minus joriy qator raqami bo'lishi kerak. Buning uchun ichma-ich for tsikllardan foydalaning: tashqi tsikl qatorlar uchun, birinchi ichki tsikl bo'sh joylar uchun, ikkinchi ichki tsikl yulduzchalar uchun.

**Kutilayotgan natija:**
```
      *
     ***
    *****
   *******
  *********
 ***********
*************
```

---

#### Masala 13: Fibonachchi 10 ta son

**Tavsif:** Sizning vazifangiz Fibonachchi ketma-ketligining birinchi 10 ta sonini chiqarishdir. Fibonachchi ketma-ketligi quyidagicha ishlaydi: birinchi son 0, ikkinchi son 1, keyingi har bir son oldingi ikkita sonning yig'indisiga teng. Ya'ni: 0, 1, 1 (0+1), 2 (1+1), 3 (1+2), 5 (2+3), 8 (3+5), 13 (5+8), 21 (8+13), 34 (13+21) va hokazo. Buning uchun avval ikki o'zgaruvchini 0 va 1 ga tenglashtiring. Birinchi sonni chiqaring. Keyin for tsikli yordamida qolgan 9 ta sonni hisoblang va chiqaring. Har bir iteratsiyada yangi sonni hisoblang (oldingi ikkita sonning yig'indisi), chiqaring va o'zgaruvchilarni yangilang. Barcha sonlar bir qatorda, bir-biridan bo'sh joy bilan ajratilgan holda chiqarilishi kerak.

**Kutilayotgan natija:**
```
0 1 1 2 3 5 8 13 21 34
```

---

#### Masala 14: So'zlar sonini topish

**Tavsif:** Sizga gap (matn) berilgan. Sizning vazifangiz bu gapdagi so'zlar sonini aniqlashdir. So'zlar bo'sh joylar bilan ajratilgan. Buning uchun for tsikli yordamida gapdagi har bir belgini ko'rib chiqing. Agar belgi bo'sh joy bo'lmasa, uni joriy so'zga qo'shing. Agar belgi bo'sh joy bo'lsa va joriy so'z bo'sh bo'lmasa, bu so'zni chiqaring, so'zlar sonini birga oshiring va joriy so'zni tozalang. Gap oxirida ham so'z bo'lishi mumkin, shuning uchun tsikl tugagandan keyin agar joriy so'z bo'sh bo'lmasa, uni ham chiqaring va sanagichni oshiring. Har bir topilgan so'zni tartib raqami bilan chiqaring. Oxirida jami so'zlar sonini ko'rsating. Eslatma: split() funksiyasidan foydalanmang, faqat for tsikli va asosiy amallardan foydalaning.

**Berilgan ma'lumotlar:**
```python
gap = "Python dasturlash tili juda qiziqarli va kuchli"
```

**Kutilayotgan natija:**
```
So'zlar:
  1. Python
  2. dasturlash
  3. tili
  4. juda
  5. qiziqarli
  6. va
  7. kuchli

Jami so'zlar soni: 7
```

---

#### Masala 15: Murakkab naqsh

**Tavsif:** Sizning vazifangiz ichma-ich for tsikllar yordamida romb shaklini yaratishdir. Romb ikki qismdan iborat: yuqori qism (piramida) va pastki qism (teskari piramida). Yuqori qism 5 qatordan iborat bo'lib, har bir qatorda yulduzchalar soni ortib boradi (1, 3, 5, 7, 9). Pastki qism 4 qatordan iborat bo'lib, har bir qatorda yulduzchalar soni kamayib boradi (7, 5, 3, 1). Har bir qatorda yulduzchalar markazda joylashgan bo'lishi kerak, ya'ni chapdan bo'sh joylar bo'lishi kerak. Buning uchun uchta for tsikli kerak: birinchi tsikl qatorlar uchun, ikkinchi tsikl bo'sh joylar uchun, uchinchi tsikl yulduzchalar uchun. Yuqori qism uchun qatorlar 1 dan 5 gacha, pastki qism uchun qatorlar 4 dan 1 gacha (teskari tartibda) bo'lishi kerak.

**Kutilayotgan natija:**
```
    *
   ***
  *****
 *******
*********
 *******
  *****
   ***
    *
```

---

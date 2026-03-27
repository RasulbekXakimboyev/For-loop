# Python dasturlash tilida For tsikli mavzusi (For loop in Python)


### For tsikli nima?

**For tsikli** — bu Pythonning eng kuchli va eng ko'p ishlatiladigan takrorlanish vositasidir. For tsikli ma'lum bir to'plam (list, string, range va boshqalar) ustida ketma-ket harakat qilish uchun ishlatiladi.

Oddiy qilib aytganda: **For tsikli — bu biror ishni bir necha marta takrorlash uchun mo'ljallangan maxsus buyruq.**

### Nima uchun for tsikli juda muhim?

Dasturlashda biz ko'pincha:
- Ro'yxatdagi har bir elementni ko'rib chiqishimiz kerak
- 1 dan 100 gacha sonlarni chiqarishimiz kerak
- Matn ichidagi har bir harfni tekshirishimiz kerak
- Bir xil ishni ko'p marta takrorlashimiz kerak

Agar for tsikli bo'lmasa, biz har safar qo'lda yozishimiz kerak edi:

```python
# For tsiklisiz (juda noqulay!)
print(1)
print(2)
print(3)
print(4)
print(5)
# ... 100 gacha davom etadi!

# For tsikli bilan (qulay!)
for i in range(1, 101):
    print(i)
```

### Real hayotdagi analogiya

For tsiklini quyidagi holatlar bilan solishtirish mumkin:

**Maktabda davomatni o'qish:**
Ustoz sinfdagi har bir o'quvchini ketma-ket chaqiradi:
- "Ali?"
- "Vali?"
- "Dilnoza?"
- "Madina?"

Bu xuddi for tsikli kabi — ro'yxatdagi har bir elementga navbat bilan murojaat qilish.

**Oshxonada idishlarni yuvish:**
Siz lavaboda 10 ta idish bor. Har birini navbat bilan yuvib chiqasiz:
- 1-idish → yuv
- 2-idish → yuv
- 3-idish → yuv
- ...

**Zinapoyadan chiqish:**
Birinchi qavatdan beshinchi qavatga chiqish uchun har bir zinapoya pog'onasiga qadam qo'yasiz. Bu ham for tsikli kabi ketma-ketlikdir.

### For tsikli while'dan qanday farq qiladi?

| **For tsikli** | **While tsikli** |
|----------------|------------------|
| Ma'lum sondagi takrorlanish uchun | Shart bajarilgunga qadar takrorlanish uchun |
| Ro'yxat, string kabi kolleksiyalar ustida ishlash oson | Shart asosida ishlaydi |
| Takrorlanish soni oldindan ma'lum | Takrorlanish soni noma'lum bo'lishi mumkin |
| Sintaksisi qisqaroq va tushunarli | Ko'proq nazorat, lekin murakkab |

**Misol:**

```python
# FOR tsikli - takrorlanish soni ma'lum
for i in range(5):
    print(i)

# WHILE tsikli - shart bajarilgunga qadar
i = 0
while i < 5:
    print(i)
    i += 1
```

---

## 2. For tsiklining asosiy sintaksisi

### To'liq sintaksis

```python
for loop_o'zgaruvchi in iteratsiya_obyekt:
    # Kod bloki (body)
    # Bu yerda takrorlanadigan amallar yoziladi
```

### Har bir qismni batafsil tushuntiramiz

#### 1️⃣ `for` kalit so'zi

`for` — bu Pythonga "men takrorlash tsiklini boshlamoqchiman" degan signal. Bu maxsus so'z (keyword) bo'lib, Python uni taniydi va tsikl boshlanishini tushunadi.

```python
for  # Bu yerda tsikl boshlanadi
```

#### 2️⃣ Loop o'zgaruvchisi (masalan, `i`)

Loop o'zgaruvchisi — bu har bir takrorlanishda yangi qiymat oladigan vaqtinchalik o'zgaruvchi.

```python
for i in range(5):
    print(i)

# i — loop o'zgaruvchisi
# Har safar yangi qiymat oladi: 0, 1, 2, 3, 4
```

**Muhim:** Loop o'zgaruvchisining nomi ixtiyoriy:
- `i` — eng keng tarqalgan
- `son`, `element`, `harf`, `x` — hammasi to'g'ri

```python
for son in range(3):
    print(son)  # 0, 1, 2

for harf in "salom":
    print(harf)  # s, a, l, o, m
```

#### 3️⃣ `in` operatori

`in` operatori — "ichidan", "dan" ma'nosini bildiradi. U loop o'zgaruvchisini iteratsiya obyekti bilan bog'laydi.

```python
for i in range(5):
    # "i" "range(5)" ichidan qiymat oladi
```

#### 4️⃣ Iteratsiya obyekti

Iteratsiya obyekti — bu for tsikli ustida harakat qila oladigan har qanday to'plam:
- `range()` — sonlar ketma-ketligi
- `list` — ro'yxat
- `string` — matn
- `tuple` — o'zgarmas ro'yxat
- `dictionary` — lug'at
- va boshqalar

```python
# range bilan
for i in range(3):
    print(i)

# list bilan
for meva in ["olma", "banan", "olcha"]:
    print(meva)

# string bilan
for harf in "Python":
    print(harf)
```

#### 5️⃣ Kolon (`:`)

Kolon — tsikl sarlavhasining oxiriga qo'yiladi va "endi kod bloki boshlanadi" degan ma'noni bildiradi.

```python
for i in range(5):  # Kolon shart!
    print(i)
```

**Xato:** Agar kolonni unutsangiz:
```python
for i in range(5)  # SyntaxError!
    print(i)
```

#### 6️⃣ Kod bloki (body)

Kod bloki — tsiklda takrorlanadigan buyruqlar. Python'da kod bloki **4 ta bo'sh joy (indent)** yoki **1 ta Tab** bilan boshlanadi.

```python
for i in range(3):
    print("Bu birinchi buyruq")    # tsikl ichida
    print("Bu ikkinchi buyruq")    # tsikl ichida
print("Bu tsikldan tashqarida")     # tsikl tugadi
```

**Natija:**
```
Bu birinchi buyruq
Bu ikkinchi buyruq
Bu birinchi buyruq
Bu ikkinchi buyruq
Bu birinchi buyruq
Bu ikkinchi buyruq
Bu tsikldan tashqarida
```

### To'liq misol va har bir qatori izohli

```python
# 0 dan 4 gacha sonlarni chiqaramiz
for i in range(5):              # i: 0, 1, 2, 3, 4 qiymatlarini oladi
    print(f"Hozirgi son: {i}")  # Har bir iteratsiyada i ni chiqaradi
    print("Bu tsikl ichida")     # Bu ham har safar chiqadi

print("Tsikl tugadi!")           # Bu faqat 1 marta, oxirida chiqadi
```

**Natija:**
```
Hozirgi son: 0
Bu tsikl ichida
Hozirgi son: 1
Bu tsikl ichida
Hozirgi son: 2
Bu tsikl ichida
Hozirgi son: 3
Bu tsikl ichida
Hozirgi son: 4
Bu tsikl ichida
Tsikl tugadi!
```

---

## 3. range() funksiyasi

`range()` — bu for tsikli bilan eng ko'p ishlatiladigan funksiya. U sonlar ketma-ketligini yaratadi.

### 3.1. `range(stop)` — faqat tugash nuqtasi

**Sintaksis:**
```python
range(stop)
```

**Ma'nosi:** 0 dan boshlab `stop` gacha (stop ichiga kirmaydi) sonlar ketma-ketligini yaratadi.

```python
# 0 dan 5 gacha (5 kirmaydi)
for i in range(5):
    print(i)  # 0, 1, 2, 3, 4
```

**Izoh:**
- `range(5)` — 0, 1, 2, 3, 4 (jami 5 ta son)
- `range(10)` — 0, 1, 2, 3, 4, 5, 6, 7, 8, 9 (jami 10 ta son)

**Nega `stop` ichiga kirmaydi?**

Bu Python'ning standart qoidasi. Ko'pchilik dasturlash tillarida indekslar 0 dan boshlanadi, shuning uchun `range(5)` 5 ta element hosil qiladi (0 dan 4 gacha).

**Misol:**
```python
# 1 dan 10 gacha sonlar yig'indisini topamiz
yigindi = 0                  # Boshlang'ich qiymat 0
for son in range(1, 11):     # 1 dan 10 gacha (11 kirmaydi)
    yigindi += son           # Har bir sonni qo'shamiz
print(f"Yig'indi: {yigindi}") # Natija: 55
```

### 3.2. `range(start, stop)` — boshlanish va tugash

**Sintaksis:**
```python
range(start, stop)
```

**Ma'nosi:** `start` dan boshlab `stop` gacha (stop ichiga kirmaydi) sonlar ketma-ketligi.

```python
# 5 dan 10 gacha
for i in range(5, 10):
    print(i)  # 5, 6, 7, 8, 9
```

**Izohli misol:**
```python
# 10 dan 20 gacha juft sonlarni chiqaramiz
print("10 dan 20 gacha sonlar:")
for son in range(10, 21):        # 10 dan 20 gacha (21 kirmaydi)
    print(son, end=" ")          # Gorizontal chiqarish
# Natija: 10 11 12 13 14 15 16 17 18 19 20
```

### 3.3. `range(start, stop, step)` — qadam bilan

**Sintaksis:**
```python
range(start, stop, step)
```

**Ma'nosi:** 
- `start` — boshlang'ich son
- `stop` — tugash nuqtasi (kirmaydi)
- `step` — qadam (har necha sondan keyin)

```python
# 0 dan 10 gacha 2 qadam bilan (juft sonlar)
for i in range(0, 11, 2):
    print(i)  # 0, 2, 4, 6, 8, 10
```

**Batafsil misollar:**

```python
# 1 dan 20 gacha 3 qadam bilan
for son in range(1, 21, 3):
    print(son, end=" ")
# Natija: 1 4 7 10 13 16 19

print()  # Yangi qator

# 5 dan 50 gacha 5 qadam bilan
for son in range(5, 51, 5):
    print(son, end=" ")
# Natija: 5 10 15 20 25 30 35 40 45 50
```

### 3.4. `range()` bilan teskari sanash — manfiy step

**Sintaksis:**
```python
range(start, stop, -step)
```

**Ma'nosi:** Katta sondan kichik songa qarab sanash.

```python
# 10 dan 1 gacha (teskari)
for i in range(10, 0, -1):
    print(i)  # 10, 9, 8, 7, 6, 5, 4, 3, 2, 1
```

**Muhim qoidalar:**
- `start` > `stop` bo'lishi kerak
- `step` manfiy bo'lishi kerak
- `stop` yana ham ichiga kirmaydi

**Misollar:**

```python
# Raketa uchirish hisoblashi (countdown)
print("Raketa uchirish:")
for son in range(10, 0, -1):     # 10 dan 1 gacha
    print(f"{son}...")            # Har bir sonni chiqaramiz
print("Uchdi!")                # Oxirida xabar

# Natija:
# 10...
# 9...
# 8...
# ...
# 1...
# Uchdi!
```

```python
# 100 dan 0 gacha 10 qadam bilan
for son in range(100, -1, -10):
    print(son, end=" ")
# Natija: 100 90 80 70 60 50 40 30 20 10 0
```

### 3.5. `range()` qanday obyekt qaytaradi?

`range()` maxsus "range" obyektini qaytaradi. Bu list emas, lekin list'ga o'xshash ishlaydi.

```python
# range obyekti
r = range(5)
print(r)           # range(0, 5)
print(type(r))     # <class 'range'>

# Listga o'tkazish mumkin
print(list(r))     # [0, 1, 2, 3, 4]
```

**Nima uchun range alohida obyekt?**

Sabab: **Xotirani tejash**. Agar `range(1000000)` yaratilsa, Python barcha 1 million sonni xotirada saqlamaydi. Faqat zarur bo'lganda yaratadi.

```python
# Katta range — lekin kam xotira
for i in range(1000000):
    # Python faqat i kerak bo'lganda yaratadi
    pass
```

---

## 4. For tsikli list bilan ishlashi

List — bu Python'da eng ko'p ishlatiladigan ma'lumot tuzilmasi. For tsikli list bilan juda qulay ishlaydi.

### 4.1. Listdagi har bir elementni o'qish

```python
# Mevalar ro'yxati
mevalar = ["olma", "banan", "olcha", "uzum", "nok"]

# Har bir mevani chiqaramiz
for meva in mevalar:                    # meva — har bir element
    print(f"Men {meva} yaxshi ko'raman") # Har bir meva uchun

# Natija:
# Men olma yaxshi ko'raman
# Men banan yaxshi ko'raman
# Men olcha yaxshi ko'raman
# Men uzum yaxshi ko'raman
# Men nok yaxshi ko'raman
```

**Qanday ishlaydi:**
1. For tsikli `mevalar` listining birinchi elementi `"olma"` ni oladi
2. `meva` o'zgaruvchisiga `"olma"` qiymatini beradi
3. Kod blokini bajaradi
4. Keyingi element `"banan"` ga o'tadi
5. Jarayon tugagunga qadar davom etadi

### 4.2. Listdagi elementlarni indeks bilan chiqarish

Ba'zan bizga elementning o'zi ham, uning indeksi (tartibi) ham kerak bo'ladi.

```python
# Talabalar ro'yxati
talabalar = ["Ali", "Vali", "Dilnoza", "Madina", "Sobir"]

# Indeks bilan chiqarish (usul 1 - range va len)
print("=== Usul 1: range(len()) ===")
for i in range(len(talabalar)):                  # i: 0, 1, 2, 3, 4
    print(f"{i+1}. {talabalar[i]}")             # Indeks + 1 (odamlar 1 dan boshlaydi)

# Natija:
# 1. Ali
# 2. Vali
# 3. Dilnoza
# 4. Madina
# 5. Sobir
```

**Izoh:**
- `len(talabalar)` — listning uzunligi (5)
- `range(len(talabalar))` — `range(5)` — 0, 1, 2, 3, 4
- `talabalar[i]` — i-indeksdagi element

### 4.3. Listdagi stringlarni qayta ishlash

```python
# Ismlar ro'yxati
ismlar = ["ali", "vali", "dilnoza", "madina"]

# Har bir ismni katta harf bilan chiqarish
print("Katta harf bilan:")
for ism in ismlar:                            # Har bir ism uchun
    katta_ism = ism.capitalize()              # Birinchi harfni katta qilish
    print(katta_ism)                          # Chiqarish

# Natija:
# Ali
# Vali
# Dilnoza
# Madina
```

**Murakkab misol — stringlarni tahlil qilish:**

```python
# So'zlar ro'yxati
sozlar = ["Python", "dasturlash", "FOR", "tsikli", "MUHIM"]

# Har bir so'z haqida ma'lumot
for soz in sozlar:                                    # Har bir so'z uchun
    uzunlik = len(soz)                                # So'z uzunligi
    katta_harflar = sum(1 for h in soz if h.isupper()) # Katta harflar soni
    
    print(f"So'z: {soz}")                             # So'zning o'zi
    print(f"  Uzunligi: {uzunlik} harf")             # Uzunligi
    print(f"  Katta harflar: {katta_harflar}")       # Katta harflar
    print("-" * 30)                                   # Ajratuvchi chiziq

# Natija:
# So'z: Python
#   Uzunligi: 6 harf
#   Katta harflar: 1
# ------------------------------
# So'z: dasturlash
#   Uzunligi: 10 harf
#   Katta harflar: 0
# ... va hokazo
```

### 4.4. Listdagi sonlarni qayta ishlash

```python
# Sonlar ro'yxati
sonlar = [12, 45, 7, 89, 23, 56, 34, 91, 6]

# Barcha sonlarning yig'indisi
yigindi = 0                           # Boshlang'ich qiymat
for son in sonlar:                    # Har bir son uchun
    yigindi += son                    # Sonni qo'shish
    print(f"{son} qo'shildi. Hozirgi yig'indi: {yigindi}")

print(f"\nJami yig'indi: {yigindi}")  # Yakuniy natija

# Natija:
# 12 qo'shildi. Hozirgi yig'indi: 12
# 45 qo'shildi. Hozirgi yig'indi: 57
# 7 qo'shildi. Hozirgi yig'indi: 64
# ...
# Jami yig'indi: 363
```

---

## 5. For tsikli string bilan ishlashi

String (matn) ham iteratsiya obyekti — ya'ni for tsikli har bir harfga alohida murojaat qila oladi.

### 5.1. Har bir harfni alohida chiqarish

```python
# Matn
matn = "Python"

# Har bir harfni alohida chiqaramiz
for harf in matn:                     # Har bir harf uchun
    print(harf)                       # Harfni chiqarish

# Natija:
# P
# y
# t
# h
# o
# n
```

**Gorizontal chiqarish:**

```python
matn = "Dasturlash"

# Har bir harfni bo'sh joy bilan
for harf in matn:
    print(harf, end=" ")              # end=" " — yangi qator emas, bo'sh joy
print()  # Oxirida yangi qator

# Natija: D a s t u r l a s h
```

### 5.2. Stringdagi belgilarni sanash

```python
# Matn
gap = "Python dasturlash tili juda qiziqarli"

# Bo'sh joylar sonini topamiz
bosh_joylar = 0                          # Hisoblagich
for belgi in gap:                        # Har bir belgi uchun
    if belgi == " ":                     # Agar bo'sh joy bo'lsa
        bosh_joylar += 1                 # Hisoblagichni oshiramiz

print(f"Bo'sh joylar soni: {bosh_joylar}")
# Natija: Bo'sh joylar soni: 4
```

**Katta harflar sonini topish:**

```python
matn = "Python Dasturlash Tili"

# Katta harflar
katta_harflar = 0
for harf in matn:                        # Har bir harf uchun
    if harf.isupper():                   # Agar katta harf bo'lsa
        katta_harflar += 1               # Sanagich oshadi
        print(f"Katta harf topildi: {harf}")

print(f"\nJami katta harflar: {katta_harflar}")

# Natija:
# Katta harf topildi: P
# Katta harf topildi: D
# Katta harf topildi: T
# Jami katta harflar: 3
```

### 5.3. Unli va undosh harflarni ajratish

```python
# Matn
matn = "Dasturlash juda qiziqarli"

# Unli harflar
unli_harflar = "aeiouAEIOU"

# Sanagichlar
unli_soni = 0
undosh_soni = 0

# Har bir harfni tekshiramiz
for belgi in matn:                       # Har bir belgi uchun
    if belgi.isalpha():                  # Faqat harflar
        if belgi in unli_harflar:        # Agar unli bo'lsa
            unli_soni += 1
        else:                            # Aks holda undosh
            undosh_soni += 1

print(f"Unli harflar: {unli_soni}")
print(f"Undosh harflar: {undosh_soni}")

# Natija:
# Unli harflar: 9
# Undosh harflar: 11
```

### 5.4. Stringni teskari o'girish (manual)

```python
# Matn
matn = "Python"

# Teskari matn (bo'sh string)
teskari = ""

# Har bir harfni boshiga qo'shamiz
for harf in matn:                        # Har bir harf uchun
    teskari = harf + teskari             # Harfni boshiga qo'shish
    print(f"Hozirgi teskari: {teskari}") # Jarayonni ko'rsatish

print(f"\nYakuniy teskari: {teskari}")

# Natija:
# Hozirgi teskari: P
# Hozirgi teskari: yP
# Hozirgi teskari: tyP
# Hozirgi teskari: htyP
# Hozirgi teskari: ohtyP
# Hozirgi teskari: nohtyP
# Yakuniy teskari: nohtyP
```

---

## 6. for + if birgalikda ishlatish

For va if birgalikda ishlatilsa, juda kuchli imkoniyatlar paydo bo'ladi. Biz elementlarni filtrlay olamiz, shartlarga mos ravishda qayta ishlay olamiz.

### 6.1. Juft sonlarni topish

```python
# 1 dan 20 gacha juft sonlar
print("Juft sonlar:")
for son in range(1, 21):                 # 1 dan 20 gacha
    if son % 2 == 0:                     # Agar 2 ga qoldiqsiz bo'linsa
        print(son, end=" ")              # Juft son chiqarish

# Natija: 2 4 6 8 10 12 14 16 18 20
```

**Izoh:**
- `son % 2` — sonni 2 ga bo'lgandagi qoldiq
- Agar qoldiq 0 bo'lsa — son juft
- Agar qoldiq 1 bo'lsa — son toq

### 6.2. Toq sonlarni topish

```python
# 1 dan 15 gacha toq sonlar
print("\nToq sonlar:")
for son in range(1, 16):                 # 1 dan 15 gacha
    if son % 2 != 0:                     # Agar 2 ga qoldiq bilan bo'linsa
        print(son, end=" ")              # Toq son chiqarish

# Natija: 1 3 5 7 9 11 13 15
```

### 6.3. Unli harflarni sanash

```python
# Matn
matn = "Python dasturlash tili"

# Unli harflar to'plami
unli_harflar = "aeiouAEIOU"

# Sanagich
unli_soni = 0

# Har bir harfni tekshirish
for harf in matn:                        # Har bir harf uchun
    if harf in unli_harflar:             # Agar unli harf bo'lsa
        unli_soni += 1                   # Sanagichni oshirish
        print(f"Unli topildi: '{harf}'") # Topilgan harfni ko'rsatish

print(f"\nJami unli harflar: {unli_soni}")

# Natija:
# Unli topildi: 'o'
# Unli topildi: 'a'
# Unli topildi: 'u'
# Unli topildi: 'a'
# Unli topildi: 'i'
# Unli topildi: 'i'
# Jami unli harflar: 6
```

### 6.4. Katta harflarni ajratish

```python
# Aralash matn
matn = "Python Dasturlash Tilida FOR Tsikli"

# Faqat katta harflarni chiqaramiz
print("Katta harflar:")
for harf in matn:                        # Har bir harf
    if harf.isupper():                   # Agar katta harf bo'lsa
        print(harf, end="")              # Bo'sh joysiz chiqarish

# Natija: PDTFT
```

### 6.5. Musbat va manfiy sonlarni ajratish

```python
# Aralash sonlar ro'yxati
sonlar = [12, -5, 8, -3, 15, -7, 20, -1, 9, -11]

# Alohida ro'yxatlar
musbat_sonlar = []                       # Musbat sonlar uchun
manfiy_sonlar = []                       # Manfiy sonlar uchun

# Har bir sonni tekshirish
for son in sonlar:                       # Har bir son uchun
    if son > 0:                          # Agar musbat bo'lsa
        musbat_sonlar.append(son)        # Musbatga qo'shamiz
    elif son < 0:                        # Agar manfiy bo'lsa
        manfiy_sonlar.append(son)        # Manfiyga qo'shamiz

print(f"Musbat sonlar: {musbat_sonlar}")
print(f"Manfiy sonlar: {manfiy_sonlar}")

# Natija:
# Musbat sonlar: [12, 8, 15, 20, 9]
# Manfiy sonlar: [-5, -3, -7, -1, -11]
```

### 6.6. Murakkab shart — 3 ga ham, 5 ga ham bo'linadigan sonlar

```python
# 1 dan 50 gacha 3 ga ham, 5 ga ham bo'linadigan sonlar
print("3 ga ham, 5 ga ham bo'linadigan sonlar:")
for son in range(1, 51):                 # 1 dan 50 gacha
    if son % 3 == 0 and son % 5 == 0:    # Ikkalasiga ham bo'linadi
        print(son, end=" ")

# Natija: 15 30 45
```

---

## 7. break va continue — Tsiklni boshqarish

`break` va `continue` — tsikl oqimini boshqarish uchun maxsus buyruqlar.

### 7.1. `break` — tsiklni to'xtatish

`break` tsiklni to'liq to'xtatadi va undan chiqib ketadi.

**Sodda misol:**

```python
# 1 dan 10 gacha, lekin 5 da to'xta
for son in range(1, 11):                 # 1 dan 10 gacha
    if son == 5:                         # Agar son 5 bo'lsa
        print("5 topildi! To'xtayapman.")
        break                            # Tsiklni to'xtatish
    print(son)

# Natija:
# 1
# 2
# 3
# 4
# 5 topildi! To'xtayapman.
```

**Real hayot analogiyasi:**

Siz do'konda qalam qidiryapsiz. Har bir javonni ko'rib chiqyapsiz. Qalam topilgandan keyin ko'rishni to'xtatasiz — bu `break`.

**Murakkab misol — biror elementni qidirish:**

```python
# Talabalar ro'yxati
talabalar = ["Ali", "Vali", "Dilnoza", "Madina", "Sobir"]

# Dilnozani qidiramiz
qidiriladigan = "Dilnoza"
topildi = False                          # Bayroq (flag)

for i, talaba in enumerate(talabalar):   # Indeks va ism bilan
    print(f"{i+1}. {talaba} tekshirilmoqda...")
    if talaba == qidiriladigan:          # Agar topilsa
        print(f"✅ {qidiriladigan} topildi! {i+1}-o'rinda.")
        topildi = True
        break                            # Qidiruvni to'xtatish

if not topildi:
    print(f"❌ {qidiriladigan} topilmadi.")

# Natija:
# 1. Ali tekshirilmoqda...
# 2. Vali tekshirilmoqda...
# 3. Dilnoza tekshirilmoqda...
# ✅ Dilnoza topildi! 3-o'rinda.
```

### 7.2. `continue` — keyingi iteratsiyaga o'tish

`continue` joriy iteratsiyani o'tkazib yuboradi va keyingisiga o'tadi.

**Sodda misol:**

```python
# 1 dan 10 gacha, lekin 5 ni o'tkazib yubor
for son in range(1, 11):                 # 1 dan 10 gacha
    if son == 5:                         # Agar son 5 bo'lsa
        continue                         # 5 ni o'tkazib yuboramiz
    print(son)

# Natija:
# 1
# 2
# 3
# 4
# 6  (5 yo'q!)
# 7
# 8
# 9
# 10
```

**Real hayot analogiyasi:**

Siz sinfdagi o'quvchilarni chaqiryapsiz, lekin bitta o'quvchi bugun yo'q (kasal). Uni o'tkazib, keyingisiga o'tasiz — bu `continue`.

**Murakkab misol — faqat juft sonlarni chiqarish:**

```python
# 1 dan 20 gacha sonlar, lekin faqat juft sonlarni chiqarish
print("Juft sonlar (continue yordamida):")
for son in range(1, 21):                 # 1 dan 20 gacha
    if son % 2 != 0:                     # Agar toq bo'lsa
        continue                         # O'tkazib yuboramiz
    print(son, end=" ")                  # Faqat juft sonlar chiqadi

# Natija: 2 4 6 8 10 12 14 16 18 20
```

### 7.3. `break` va `continue` farqi

| `break` | `continue` |
|---------|-----------|
| Tsiklni to'liq to'xtatadi | Faqat joriy iteratsiyani o'tkazadi |
| Tsikldan chiqib ketadi | Keyingi iteratsiyaga o'tadi |
| Qolgan elementlar ko'rib chiqilmaydi | Qolgan elementlar davom etadi |

**Taqqoslash misoli:**

```python
print("=== BREAK ===")
for son in range(1, 6):
    if son == 3:
        break
    print(son)
# Natija: 1, 2

print("\n=== CONTINUE ===")
for son in range(1, 6):
    if son == 3:
        continue
    print(son)
# Natija: 1, 2, 4, 5 (3 o'tkazildi)
```

### 7.4. Real amaliy misol — parol tekshirish

```python
# Parolni 3 marta kiritish imkoniyati
maksimal_urinish = 3                     # Maksimal urinishlar soni
to'g'ri_parol = "python123"              # To'g'ri parol

for urinish in range(1, maksimal_urinish + 1):  # 1 dan 3 gacha
    print(f"\nUrinish {urinish}/{maksimal_urinish}")
    parol = input("Parol kiriting: ")    # Foydalanuvchidan parol
    
    if parol == to'g'ri_parol:           # Agar to'g'ri bo'lsa
        print("✅ Parol to'g'ri! Tizimga kirdingiz.")
        break                            # Tsiklni to'xtatamiz
    else:
        print("❌ Parol noto'g'ri.")
        qolgan = maksimal_urinish - urinish
        if qolgan > 0:
            print(f"Yana {qolgan} urinish qoldi.")
else:
    # Agar break ishlamasa (hech bir urinish to'g'ri bo'lmasa)
    print("\nUrinishlar tugadi. Hisobingiz bloklandi.")
```

---

## 8. Ichma-ich FOR Tsikli (Nested Loop)

Ichma-ich tsikl — bu bir for tsikli ichida boshqa for tsikli.

### 8.1. Oddiy ichma-ich tsikl

```python
# Tashqi tsikl 1 dan 3 gacha
for i in range(1, 4):                    # i: 1, 2, 3
    print(f"\nTashqi tsikl: i = {i}")
    
    # Ichki tsikl 1 dan 3 gacha
    for j in range(1, 4):                # j: 1, 2, 3
        print(f"  Ichki tsikl: j = {j}")

# Natija:
# Tashqi tsikl: i = 1
#   Ichki tsikl: j = 1
#   Ichki tsikl: j = 2
#   Ichki tsikl: j = 3
# Tashqi tsikl: i = 2
#   Ichki tsikl: j = 1
#   Ichki tsikl: j = 2
#   Ichki tsikl: j = 3
# ... va hokazo
```

**Qanday ishlaydi:**
1. Tashqi tsikl `i=1` ni oladi
2. Ichki tsikl to'liq ishlaydi (`j=1, 2, 3`)
3. Tashqi tsikl `i=2` ga o'tadi
4. Ichki tsikl yana to'liq ishlaydi
5. Va hokazo...

### 8.2. Multiplikatsiya jadvali

```python
# Ko'paytirish jadvali 1 dan 5 gacha
print("KO'PAYTIRISH JADVALI")
print("=" * 40)

for i in range(1, 6):                    # Tashqi: 1 dan 5 gacha
    print(f"\n{i} ning ko'paytirish jadvali:")
    for j in range(1, 11):               # Ichki: 1 dan 10 gacha
        natija = i * j                   # Ko'paytirish
        print(f"  {i} × {j} = {natija}")

# Natija:
# 1 ning ko'paytirish jadvali:
#   1 × 1 = 1
#   1 × 2 = 2
#   ...
#   1 × 10 = 10
# 2 ning ko'paytirish jadvali:
#   2 × 1 = 2
#   2 × 2 = 4
#   ...
```

### 8.3. Jadval shaklida ko'paytirish jadvali

```python
# Jadval shaklida
print("\n" + "=" * 60)
print("JADVAL SHAKLIDAGI KO'PAYTIRISH JADVALI (1-10)")
print("=" * 60)

# Sarlavha qatori
print("   |", end="")
for i in range(1, 11):
    print(f"{i:4}", end="")
print("\n" + "-" * 60)

# Har bir qator
for i in range(1, 11):                   # Qatorlar
    print(f"{i:2} |", end="")            # Qator raqami
    for j in range(1, 11):               # Ustunlar
        print(f"{i*j:4}", end="")        # Ko'paytma
    print()                              # Yangi qator

# Natija - jadval:
#    |   1   2   3   4   5   6   7   8   9  10
# ------------------------------------------------------------
#  1 |   1   2   3   4   5   6   7   8   9  10
#  2 |   2   4   6   8  10  12  14  16  18  20
#  3 |   3   6   9  12  15  18  21  24  27  30
# ...
```

### 8.4. Yulduzcha piramida

```python
# Yulduzcha piramida (5 qator)
n = 5                                    # Piramida balandligi

for i in range(1, n + 1):                # Har bir qator uchun
    # Bo'sh joylar
    for j in range(n - i):               # Chapdan bo'sh joylar
        print(" ", end="")
    
    # Yulduzchalar
    for k in range(2 * i - 1):           # Har qatorda yulduzchalar
        print("*", end="")
    
    print()                              # Yangi qator

# Natija:
#     *
#    ***
#   *****
#  *******
# *********
```

**Izoh:**
- 1-qator: 4 bo'sh joy, 1 yulduz
- 2-qator: 3 bo'sh joy, 3 yulduz
- 3-qator: 2 bo'sh joy, 5 yulduz
- 4-qator: 1 bo'sh joy, 7 yulduz
- 5-qator: 0 bo'sh joy, 9 yulduz

### 8.5. Teskari piramida

```python
# Teskari piramida
n = 5

for i in range(n, 0, -1):                # 5 dan 1 gacha
    # Bo'sh joylar
    for j in range(n - i):
        print(" ", end="")
    
    # Yulduzchalar
    for k in range(2 * i - 1):
        print("*", end="")
    
    print()

# Natija:
# *********
#  *******
#   *****
#    ***
#     *
```

### 8.6. To'rtburchak

```python
# Yulduzchadan to'rtburchak
kenglik = 10
balandlik = 5

for i in range(balandlik):               # Qatorlar
    for j in range(kenglik):             # Har qatorda yulduzchalar
        print("*", end="")
    print()                              # Yangi qator

# Natija:
# **********
# **********
# **********
# **********
# **********
```

---

## 9. For tsikli + Dictionary (Lug'at)

Dictionary — bu kalit-qiymat juftliklaridan iborat ma'lumot tuzilmasi. For tsikli dictionary bilan ham ishlaydi.

### 9.1. Faqat kalitlar bo'yicha

Dictionary ustida for tsikli standart ravishda faqat kalitlarni qaytaradi.

```python
# Talaba ma'lumotlari
talaba = {
    "ism": "Ali",
    "yosh": 20,
    "kasb": "Talaba",
    "shahar": "Toshkent"
}

# Faqat kalitlarni chiqarish
print("Kalitlar:")
for kalit in talaba:                     # Standart - faqat kalitlar
    print(f"  - {kalit}")

# Natija:
# Kalitlar:
#   - ism
#   - yosh
#   - kasb
#   - shahar
```

**Alternativ — `.keys()` metodi:**

```python
# .keys() bilan
for kalit in talaba.keys():              # To'g'ridan-to'g'ri kalitlar
    print(kalit)
```

### 9.2. Faqat qiymatlar bo'yicha

`.values()` metodi faqat qiymatlarni qaytaradi.

```python
# Talaba ma'lumotlari
talaba = {
    "ism": "Ali",
    "yosh": 20,
    "kasb": "Talaba",
    "shahar": "Toshkent"
}

# Faqat qiymatlarni chiqarish
print("Qiymatlar:")
for qiymat in talaba.values():           # Faqat qiymatlar
    print(f"  - {qiymat}")

# Natija:
# Qiymatlar:
#   - Ali
#   - 20
#   - Talaba
#   - Toshkent
```

### 9.3. `.items()` bilan kalit va qiymatni birga

`.items()` — eng foydali usul. Kalit va qiymatni birga qaytaradi.

```python
# Talaba ma'lumotlari
talaba = {
    "ism": "Ali",
    "yosh": 20,
    "kasb": "Talaba",
    "shahar": "Toshkent"
}

# Kalit va qiymat birga
print("Talaba haqida:")
for kalit, qiymat in talaba.items():     # Kalit va qiymat
    print(f"  {kalit}: {qiymat}")

# Natija:
# Talaba haqida:
#   ism: Ali
#   yosh: 20
#   kasb: Talaba
#   shahar: Toshkent
```

**Izoh:**
- `.items()` har bir juftlikni tuple shaklida qaytaradi: `("ism", "Ali")`
- Biz uni ikkita o'zgaruvchiga ajratamiz: `kalit, qiymat`

### 9.4. Dictionary ichida dictionary

```python
# Talabalar ma'lumotlar bazasi
talabalar = {
    "ali": {
        "yosh": 20,
        "kurs": 2,
        "fakultet": "IT"
    },
    "vali": {
        "yosh": 21,
        "kurs": 3,
        "fakultet": "Matematika"
    },
    "dilnoza": {
        "yosh": 19,
        "kurs": 1,
        "fakultet": "Fizika"
    }
}

# Har bir talaba haqida
for ism, malumot in talabalar.items():   # Ism va ichki dict
    print(f"\n{ism.capitalize()} haqida:")
    for kalit, qiymat in malumot.items():  # Ichki dict ustida
        print(f"  {kalit}: {qiymat}")

# Natija:
# Ali haqida:
#   yosh: 20
#   kurs: 2
#   fakultet: IT
# Vali haqida:
#   yosh: 21
#   kurs: 3
#   fakultet: Matematika
# ...
```

### 9.5. Amaliy misol — mahsulotlar narxi

```python
# Mahsulotlar va narxlari
mahsulotlar = {
    "Non": 2000,
    "Tuxum": 12000,
    "Sut": 8000,
    "Yog'": 15000,
    "Shakar": 10000
}

# Jami narxni hisoblash
jami = 0                                 # Boshlang'ich qiymat

print("Do'kon ro'yxati:")
print("-" * 40)
for mahsulot, narx in mahsulotlar.items():  # Har bir mahsulot
    print(f"{mahsulot:15} - {narx:,} so'm")
    jami += narx                         # Jami narxga qo'shamiz

print("-" * 40)
print(f"{'JAMI':15} - {jami:,} so'm")

# Natija:
# Do'kon ro'yxati:
# ----------------------------------------
# Non             - 2,000 so'm
# Tuxum           - 12,000 so'm
# Sut             - 8,000 so'm
# Yog'            - 15,000 so'm
# Shakar          - 10,000 so'm
# ----------------------------------------
# JAMI            - 47,000 so'm
```

---

## 10. For tsikli + enumerate()

`enumerate()` — bu list (yoki boshqa iteratsiya obyekti) ustida ishlashda indeks va qiymatni birga olish uchun juda qulay funksiya.

### 10.1. enumerate() nima?

`enumerate()` har bir elementga indeks (tartib raqami) qo'shadi.

**Sintaksis:**
```python
enumerate(iteratsiya_obyekti, start=0)
```

- `iteratsiya_obyekti` — list, string, tuple va h.k.
- `start` — boshlang'ich indeks (standart 0)

### 10.2. enumerate() nega kerak?

**Muammo — enumerate() siz:**

```python
mevalar = ["olma", "banan", "olcha"]

# Indeks va elementni olish uchun murakkab
for i in range(len(mevalar)):
    print(f"{i}: {mevalar[i]}")
```

**Yechim — enumerate() bilan:**

```python
mevalar = ["olma", "banan", "olcha"]

# Oddiy va tushunarli
for i, meva in enumerate(mevalar):
    print(f"{i}: {meva}")
```

### 10.3. enumerate() bilan misollar

**Boshlang'ich misol:**

```python
# Rang list
ranglar = ["qizil", "yashil", "ko'k", "sariq"]

# Indeks va qiymat bilan
for indeks, rang in enumerate(ranglar):  # enumerate() ishlatish
    print(f"{indeks}. {rang}")

# Natija:
# 0. qizil
# 1. yashil
# 2. ko'k
# 3. sariq
```

**1 dan boshlab indekslash:**

```python
# Talabalar ro'yxati
talabalar = ["Ali", "Vali", "Dilnoza", "Madina"]

# 1 dan boshlaymiz
for raqam, ism in enumerate(talabalar, start=1):  # start=1
    print(f"{raqam}. {ism}")

# Natija:
# 1. Ali
# 2. Vali
# 3. Dilnoza
# 4. Madina
```

### 10.4. Amaliy misol — menu yaratish

```python
# Ovqatlar menyu
ovqatlar = [
    "Osh",
    "Lag'mon",
    "Manti",
    "Shashlik",
    "Somsa"
]

# Menyu chiqarish
print("=" * 40)
print("         OVQATLAR MENYUSI")
print("=" * 40)

for raqam, ovqat in enumerate(ovqatlar, start=1):  # 1 dan boshlab
    print(f"  {raqam}. {ovqat}")

print("=" * 40)

# Natija:
# ========================================
#          OVQATLAR MENYUSI
# ========================================
#   1. Osh
#   2. Lag'mon
#   3. Manti
#   4. Shashlik
#   5. Somsa
# ========================================
```

### 10.5. enumerate() va if birgalikda

```python
# So'zlar ro'yxati
sozlar = ["python", "dasturlash", "FOR", "tsikli", "enumerate"]

# Faqat katta harfli so'zlarni ko'rsatish
print("Katta harfli so'zlar:")
for indeks, soz in enumerate(sozlar):    # Har bir so'z
    if soz.isupper():                    # Agar katta harf bo'lsa
        print(f"  {indeks}-indeksda: {soz}")

# Natija:
# Katta harfli so'zlar:
#   2-indeksda: FOR
```

### 10.6. enumerate() ichki strukturasi

```python
# enumerate() aslida tuple qaytaradi
mevalar = ["olma", "banan", "olcha"]

for element in enumerate(mevalar):
    print(element)  # Tuple: (indeks, qiymat)

# Natija:
# (0, 'olma')
# (1, 'banan')
# (2, 'olcha')
```

---

## 11. For tsikli bilan keng tarqalgan xatolar

### Xato 1: range() noto'g'ri ishlatish

**❌ Noto'g'ri:**
```python
# Xato: range(5, 1) bo'sh ketma-ketlik
for i in range(5, 1):  # Hech narsa chiqmaydi
    print(i)
```

**✅ To'g'ri:**
```python
# To'g'ri: manfiy step kerak
for i in range(5, 0, -1):  # 5, 4, 3, 2, 1
    print(i)
```

### Xato 2: Indeksda chiqib ketish

**❌ Noto'g'ri:**
```python
sonlar = [10, 20, 30]

for i in range(4):  # 0, 1, 2, 3 (3 xato!)
    print(sonlar[i])  # IndexError: list index out of range
```

**✅ To'g'ri:**
```python
sonlar = [10, 20, 30]

for i in range(len(sonlar)):  # 0, 1, 2
    print(sonlar[i])
```

### Xato 3: Stringni list deb o'ylash

**❌ Noto'g'ri:**
```python
matn = "Python"
matn[0] = "J"  # TypeError: 'str' object does not support item assignment
```

**✅ To'g'ri:**
```python
matn = "Python"
yangi_matn = "J" + matn[1:]  # "Jython"
```

### Xato 4: Tsikl ichida listni o'zgartirish

**❌ Noto'g'ri:**
```python
sonlar = [1, 2, 3, 4, 5]

for son in sonlar:
    sonlar.remove(son)  # Xavfli! Natija kutilmaganda bo'ladi

print(sonlar)  # [2, 4] (Nima bo'ldi?!)
```

**✅ To'g'ri:**
```python
sonlar = [1, 2, 3, 4, 5]
yangi_sonlar = []  # Yangi list

for son in sonlar:
    if son % 2 == 0:  # Faqat juftlarni qoldirish
        yangi_sonlar.append(son)

sonlar = yangi_sonlar
print(sonlar)  # [2, 4]
```

### Xato 5: Indent (bo'sh joy) xatolari

**❌ Noto'g'ri:**
```python
for i in range(3):
print(i)  # IndentationError
```

**✅ To'g'ri:**
```python
for i in range(3):
    print(i)  # 4 bo'sh joy yoki 1 Tab
```

---
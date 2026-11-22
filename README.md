# Farm Valley v0.2

O‘zbek tilidagi izometrik ferma o‘yini. Bu yangilanish v0.1 manba kodiga qurilgan. Ekinlar, hosil, hayvonlar, ishlab chiqarish, savdo, darajalar, ombor, buyurtmalar, qurilish va ochiladigan hududlar davom etadi. O‘yin HTML, CSS va JavaScript bilan ishlaydi. Build bosqichi, npm yoki pullik xizmat kerak emas.

## O‘ynash

- Vertikal yoki gorizontal ekranda o‘ynang. Bir barmoq bilan xaritani suring, ikki barmoq bilan kattalashtiring. O‘ng tomondagi tugmalar ham kamerani boshqaradi.
- Dalaga bosib bug‘doy eking. 12 soniyadan keyin shu daladan hosil yig‘ing. **Buyurtmalar** menyusida choyxonaga uch dona bug‘doy topshiring.
- Nonvoyxonaga masalliq olib boring, tovuqlarga yem bering yoki yem tegirmonida yangi yem tayyorlang. Tayyor mahsulotni yig‘ish uchun tegishli binoga bosing.
- **Do‘kon → Tanlash** orqali bino yoki bezakni sotib oling va belgilangan bo‘sh yerga qo‘ying. Obyektni ochib **Ko‘chirish** bilan joyini almashtiring.
- Animatsiyalarni kamaytirish va render o‘lchamini kichraytirish uchun **Sozlamalar → Grafika → Tejamkor**ni tanlang.

## Telefonda xarita yasash

1. **Sozlamalar → Admin → Xarita muharriri**ni oching. O‘yin xaritasi ustida tahrirlash kataklari chiqadi.
2. **Yo‘l** yoki **Suv**ni tanlang. Katakka bir marta bosing yoki barmog‘ingizni tortib ketma-ket kataklar chizing. Qo‘shni kataklar tutashadi. **O‘t** eski yo‘lni yoki daryo ustidagi katakni quruqlikka aylantiradi va shu katakdagi avtomatik bezakni yashiradi.
3. **Daraxt**, **Tosh**, **Bino** yoki **Bezak**ni tanlang va ochiq, bo‘sh o‘tli katakka qo‘ying. **Hudud** vositasi orqali qo‘shimcha katak ochishingiz mumkin.
4. Joylashtirilgan obyektni tahrirlash uchun **Tanlash**ni bosib, obyektni tanlang. **Ko‘chirish**dan keyin yangi bo‘sh katakka bosing. **O‘chirish** yoki **O‘chirgich** obyektni olib tashlaydi. Muhim obyektlar, oxirgi dala, ekinli dala va faol ishlab chiqarish joylari himoyalangan.
5. Xarita markazini o‘zgartirish uchun **Surish**ni tanlang. Ikki barmoqli zoom chizish vositasi tanlangan paytda ham ishlaydi. **Qaytarish** va **Tiklash** bir bosishda yoki barmoqni tortib qo‘yilgan o‘zgarishni butunlay qaytaradi yoki tiklaydi.
6. **Ko‘rib chiqish** orqali xaritani katak chiziqlari va muharrir tugmalarisiz ko‘ring. **Muharrirga qaytish** orqali tahrirni davom ettiring.
7. Har bir tugallangan tahrir avtomatik qoralamaga yoziladi. **Qoralamalar** bo‘limida nom bering va **Saqlash**ni bosing. Shu bo‘limdan avvalgi nusxani ochish yoki xaritani JSON formatida eksport va import qilish mumkin.
8. **Fermaga qo‘llash**ni bosib tasdiqlang. Xarita shu brauzerdagi fermaga o‘tadi. Tahrir va joriy ferma bir katakda to‘qnashsa, o‘yin o‘zgarishni rad etadi. Saqlangan obyektlar, ekinlar va ishlab chiqarish taymerlari ko‘chirilganda saqlanadi.

**Admin** bu versiyada mahalliy muharrirga kirish joyi. Hozirgi loyiha statik. **Nashr qilish** tugmasi faol bo‘lishi uchun server, admin autentifikatsiyasi va umumiy xarita saqlovi kerak. JSON xaritasi qoralama sifatida ishlaydi. **Fermaga qo‘llash** shu brauzerdagi fermani yangilaydi.

## Progress va zaxira

O‘yinni bir xil Chrome profili va bir xil sayt manzilidan ochsangiz, progress avtomatik yuklanadi. v0.1 saqlovi v0.2 ga avtomatik o‘qiladi va keyingi saqlashda yangi formatga o‘tadi. Ekin va ishlab chiqarish taymerlari o‘yin yopiq bo‘lgan vaqtni ham hisoblaydi. Kamera o‘yin ichida va ekran aylantirilganda saqlanadi.

- **Sozlamalar → Progress zaxirasi → Eksport** fermani, kamerani va qo‘llangan xaritani JSON faylga saqlaydi.
- **Sozlamalar → Progress zaxirasi → Import** shu fayldan progressni tiklaydi. Joriy progress almashtirilishidan oldin o‘yin tasdiq so‘raydi.
- Nomlangan qoralamalar va amaldagi tahrir alohida saqlanadi. Ularni zaxiralash uchun **Qoralamalar → JSON eksport**dan foydalaning.
- Brauzer ma’lumotlarini tozalash, inkognito rejimi, boshqa domen yoki boshqa brauzer progressga ta’sir qiladi. Telefon almashtirishdan oldin JSON zaxiralarni yuklab oling.

## Samsung telefonidan mavjud GitHub va Vercel loyihasini yangilash

1. ZIPni yuklab oling. Samsung **Mening fayllarim → Yuklamalar** bo‘limida ZIP ustiga bosing va **Ajratib olish / Extract**ni tanlang.
2. Chrome’da Farm Valley’ning **mavjud** GitHub reposini oching. **Add file** ko‘rinmasa, Chrome menyusida **Kompyuter uchun sayt / Desktop site**ni yoqing.
3. Eski `index.html` qaysi papkada turgan bo‘lsa, shu papkada **Add file → Upload files → choose your files** tugmalarini bosing. Ajratilgan papkadan quyidagi 10 o‘yin faylini birga tanlang: `index.html`, `style.css`, `data.js`, `world.js`, `save.js`, `model.js`, `editor.js`, `art.js`, `game.js`, `icon.svg`. ZIP va README o‘yinni ishga tushirish uchun kerak emas.
4. **Commit changes**ni bosing. Ulangan Vercel loyihasi saytni yangilashi uchun commit ishlab turgan sayt shoxiga (odatda `main`) tushishi kerak. Agar GitHub pull request ochsa, fayllarni tekshirib, uni shu shoxga birlashtiring. [GitHub fayl yuklash](https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository)
5. Vercel’da mavjud Farm Valley loyihasining **Deployments** oynasida yangi commit uchun **Ready** holatini tekshiring. Chrome’da oldingi odatiy o‘yin manzilini oching va sahifani yangilang. Shu manzildagi v0.1 progress avtomatik yuklanadi. [Vercel Git orqali joylashtirish](https://vercel.com/docs/git)
6. **Sozlamalar → Admin** menyusi chiqqanini tekshiring. Joriy progressni **Sozlamalar → Progress zaxirasi → Eksport** orqali yuklab oling.

## Sinovlar va cheklovlar

- Asosiy o‘yin mexanikasi bo‘yicha 60 dan ortiq regressiya tekshiruvi o‘tdi. Hosil, mahsulot ishlab chiqarish, sotuv, buyurtma, daraja, sig‘im, qurilish, ko‘chirish va hudud kengayishi sinovdan o‘tdi.
- v0.1 saqlovini yuklash, v2 zaxiraga o‘tish, buzilgan saqlovdan avvalgi nusxani tiklash, noto‘g‘ri JSONni rad etish va o‘yin yopiq paytdagi taymerlar sinovdan o‘tdi.
- O‘yin JS fayllari Canvas bilan 360 × 640 va 640 × 360 o‘lchamlarda ishlatildi. Sensor hodisalari simulyatsiyasida chizish, pan, pinch, qaytarish va tiklash, qoralama, preview, obyekt ko‘chirish, mahalliy qo‘llash va ikki turdagi JSON almashinuvi tekshirildi.
- Chrome’dagi yakuniy CSS joylashuvi, brauzerning mahalliy fayl tanlash oynasi va Samsung Galaxy A03 Core’dagi FPS haqiqiy qurilmada tekshiruvga qolgan. Admin autentifikatsiyasi va umumiy nashr server ulangach sinovdan o‘tkaziladi.

## Manba tuzilmasi

| Fayl | Vazifa |
| --- | --- |
| `index.html`, `style.css`, `icon.svg` | O‘yin ekrani, moslashuvchan menyular va belgi |
| `data.js` | Ekinlar, retseptlar, buyurtmalar va boshlang‘ich ferma |
| `model.js` | Inventar, qurilish, iqtisodiyot, ekin va ishlab chiqarish |
| `save.js` | Saqlovni tekshirish, v1 formatidan o‘tish, oldingi saqlovni tiklash |
| `world.js` | Yer kataklari, xarita JSON formati, moslik va to‘qnashuv tekshiruvi |
| `editor.js` | Muharrir vositalari, qoralamalar, qaytarish va tiklash |
| `art.js` | Izometrik grafikalar, keshdagi landshaft va o‘yin obyektlari |
| `game.js` | Boshqaruv, animatsiya va menyularni o‘yin tizimlariga ulash |

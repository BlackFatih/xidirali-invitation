# Xidirali & Zamira — to'y taklifnomasi

## 1. Musiqa qo'shish
Istagan qo'shiqni **`music.mp3`** nomi bilan shu papkaga tashlang.
(Fayl 2–4 MB dan oshmasin — Telegramda tez ochilishi uchun.)

Mehmon "ochish" tugmasini bosganda musiqa avtomatik, ovozi asta ko'tarilib boshlanadi.
O'ng yuqoridagi tugma orqali o'chirib-yoqish mumkin.

> Telegram va iPhone brauzerlari musiqani o'z-o'zidan ishga tushirishga ruxsat bermaydi —
> shuning uchun "ochish" pardasi qo'yilgan. Bu yagona ishlaydigan usul.

## 2. Ma'lumotlarni to'ldirish
`index.html` faylini oching va quyidagilarni almashtiring:

**`<script>` ichidagi CONFIG (fayl oxirida):**
```js
toy: new Date(2026, 8, 12, 17, 0),  // yil, oy(0=yanvar!), kun, soat, daqiqa
xarita: "https://yandex.uz/maps/..." // to'yxona joylashuvi havolasi
```
⚠️ Oy **0 dan** boshlanadi: 0=yanvar, 8=sentabr, 11=dekabr.

**HTML ichidagi `[...]` qavslar:**
- `[00:00] dan` — marosim vaqti
- `[To'yxona nomi]`
- `[Viloyat, tuman, ko'cha, uy]`

Sana va hafta kuni CONFIG'dan avtomatik yoziladi — qo'lda tegmang.

## 3. Internetga joylash (bepul)
**Eng oson — Netlify Drop:**
1. https://app.netlify.com/drop ga kiring
2. `toy-taklifnoma` papkasini brauzerga sudrab tashlang
3. Tayyor havolani Telegramga yuboring

**Yoki GitHub Pages:** repo yarating → fayllarni yuklang → Settings → Pages → main branch.

## 4. Telegramga yuborish
Havolani kanalga/guruhga tashlaganda taklifnoma nomi va tavsifi ko'rinadi.
Chiroyliroq ko'rinishi uchun rasm qo'shmoqchi bo'lsangiz — `cover.jpg` (1200×630)
tayyorlab, `<head>` ichiga qo'shing:
```html
<meta property="og:image" content="https://sizning-saytingiz.netlify.app/cover.jpg">
```

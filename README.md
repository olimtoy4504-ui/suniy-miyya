# Sun'iy miya — Android ilova

## APK olish (kompyutersiz ham bo'ladi, faqat GitHub kerak)

1. github.com saytida ro'yxatdan o'ting va **New repository** tugmasini bosing. Nom bering, masalan `suniy-miya`, keyin **Create repository**ni bosing.
2. **uploading an existing file** havolasini bosing. Zip ichidagi hamma fayl va papkalarni sudrab tashlang, so'ng **Commit changes**ni bosing.
   - `.github` papkasi yuklanmay qolsa: **Add file → Create new file** ni bosing, nomiga `.github/workflows/build.yml` deb yozing va shu fayl ichidagi matnni joylang.
3. **Actions** bo'limiga o'ting. «APK yig'ish» ishi o'zi boshlanadi va 3–5 daqiqada tugaydi (yashil ✓ chiqadi).
4. Tugagan ishni oching. Pastdagi **Artifacts** qismida `suniy-miya-apk` bor — uni yuklab oling. Zip ichida `app-debug.apk` turadi.
5. APK'ni telefonga o'tkazib o'rnating. Telefon «noma'lum manbalar»dan o'rnatishga ruxsat so'rasa, ruxsat bering.

## Android Studio bilan

Papkani **File → Open** orqali oching, keyin **Build → Build APK(s)** ni bosing.

## Gaplashish

Ilova ichida yuqoridagi 🔑 tugmasini bosing va Anthropic API kalitini kiriting. Kalitni console.anthropic.com saytidan olasiz; bu xizmat alohida pullik. Kalit faqat telefoningizda saqlanadi.
Kalitsiz ham 3D miya, chizib o'rgatish va rasm tanish ishlaydi. 3D shar uchun internet kerak.

## 🎬 Montaj Studiya

Bosh sahifada yuqoridagi 🎥 tugmasini bosing. Ichida 5 bo'lim bor:

- **📊 Hisob** — montajlaringiz soni, sarflangan soat, o'rtacha ko'rishlar, haftalik grafik, qaysi stil ko'proq ko'rilgani. «Tahlil qilish» tugmasi AI'dan hisobot va keyingi haftaga vazifalar oladi. Zaxira (JSON) bilan ma'lumotni saqlab qo'yish mumkin.
- **➕ Qo'shish** — har bir montajni yozib boring: stil, shrift, effektlar, musiqa, dastur, vaqt, narx, ko'rish/layk/saqlash.
- **🎬 Tahlil** — videoni tanlang: dastur kesimlar sonini, tempni, o'lchamni o'zi hisoblaydi, keyin AI 8 ta kadrni ko'rib hook, shrift, rang, temp bo'yicha baho va shu videoga qo'shsa bo'ladigan yangiliklarni aytadi.
- **🔥 Trendlar** — AI internetdan eng so'nggi reels stillari, shriftlar (namunasi bilan), o'tishlar va audio trendlarni qidirib beradi. Yo'nalishni tanlash mumkin (to'y, avto, sport…).
- **🤖 Hamkor** — montajlaringiz va trendlarni biladigan AI bilan suhbat; kerak bo'lsa internetdan qidiradi.

AI qismlari uchun 🔑 API kalit kerak (bosh sahifadagi kalit bilan bir xil). Video kadrlari va trend qidiruvi ko'proq token ishlatadi.

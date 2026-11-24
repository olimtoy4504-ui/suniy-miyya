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

Reels montajchi uchun studiya: `app/src/main/assets/montaj.html` (bitta fayl). Bosh sahifadagi 🎥 tugmasi orqali ochiladi.

- **📊 Hisob** — montajlar soni, soatlar, ko'rishlar grafigi, haftalik maqsad, ketma-ket kunlar, «Davom ettirish» va AI hisobot.
- **🎞 Timeline** — professional NLE uslubida: ko'p trekli (V1–V3, A1–A2, +V/+A), bog'langan video+audio, kadrlar lentasi va to'lqin shakli, Tanlash (V) va Ustara (C) asboblari, yopishish (S), overwrite, ripple o'chirish, markerlar (M), timecode, keyframe'lar (masshtab, joy, burilish, shaffoflik), fade in/out, ovoz indikatori, Ctrl+K / Q / W / J-K-L klavishlari, o'ng tugma menyusi. Hammasi avtomatik saqlanadi.
- **🤖 AI montaj** — AI kadrlaringizni ko'rib, musiqa beatlariga mos montaj qiladi va timelinega joylaydi. «✨ AI'ga buyruq» bilan tayyor montajni o'zgartirtirasiz. API'siz «⚡ Tezkor avto» ham bor.
- **⬇ MP4** — kadrma-kadr H.264 + ovoz, 720p yoki 1080p. **AE .jsx** — timeline'ni After Effects'ga ko'chiruvchi skript.
- **🎬 Tahlil** — kesimlar, harakat grafigi, BPM, beatga moslik %, hook bahosi, rang palitrasi; «Kesimlar bo'yicha timelinega» va «Shu uslubda AI montaj».
- **🔤 Shriftlar** — 130+ Google shrift, kategoriyalar, sevimlilar, trend shriftlar, tayyor juftliklar.
- **🔥 Trendlar** — avtomatik yangilanadi, yangilari «YANGI» belgisi bilan.

### AI qanday ishlaydi

- **Claude.ai ichida** (tavsiya etiladi): sahifa claude.ai'da ochilsa, AI sizning Claude obunangiz orqali ishlaydi — kalit va qo'shimcha to'lov kerak emas.
- **Fayl yoki Android ilova sifatida**: 🔑 orqali Anthropic API kaliti kiritiladi (alohida pullik). Kalitsiz ham timeline, eksport, tahlil va shriftlar ishlaydi.

### 💻 Kompyuterda

`montaj.html` faylini Chrome yoki Edge'da oching (o'ng tugma → «Open with»). MP4 eksport uchun Chrome/Edge'ning yangi versiyasi kerak.

# Android TG Manager (APK Loyihasi)

Ushbu loyiha Telegram akkauntlaringizni (1-chi, 2-chi, 3-chi va h.k.) fonda doimiy "Online" ushlab turish va xabarlarni avtomatik o'qish uchun yaratilgan to'liq Android ilovasi.

---

## Ilovaning Ichki Arxitekturasi:
1. **Foreground Service (`TelegramForegroundService.kt`):** Android tizimi batareyani tejash bahonasida ilovani fondan o'chirib yubormasligi uchun 24/7 uzluksiz ishlaydigan doimiy xizmat.
2. **Ko'p Akkauntli Interfeys (`MainActivity.kt`):** Har bir ulangan Telegram akkauntini (telefon, ism, @username, status) to'liq ekranda qulay boshqarish.
3. **Avto-O'qish & Online:** Fonda xabarlar kelishi bilan o'qiladi va Telegram serveriga status yuboriladi.

---

## APK Faylini Qanday Olish Mumkin?

### 1-Yo'l: GitHub Actions orqali (Kompyuteringizga hech narsa o'rnatmasdan avtomatik):
1. Ushbu `android_telegram_manager` papkasini GitHub'dagi repozitoriyingizga yuklang (push qiling).
2. GitHub'dagi `.github/workflows/build-apk.yml` fayli avtomatik ishga tushadi va bir necha daqiqada tayyor **`app-debug.apk`** faylini tayyorlab beradi.
3. Uni to'g'ridan-to'g'ri telefoningizga yuklab olib o'rnatishingiz mumkin.

### 2-Yo'l: Android Studio orqali:
1. Kompyuteringizda **Android Studio** dasturini oching.
2. **Open Project** tugmasini bosib `d:\birinchi mijon\android_telegram_manager` papkasini tanlang.
3. Yuqori menyudan **Build -> Build Bundle(s) / APK(s) -> Build APK(s)** ni bosing.
4. Tayyor bo'lgan `app-debug.apk` faylini telefoningizga o'tkazing.

---

## Zudlik bilan Ishlatish (PWA / Installable App):
Agar APK kutib o'tirmasdan, hoziroq telefoningizda ilova sifatida ishlatmoqchi bo'lsangiz:
1. `telegram_assistant` ichidagi `run.bat` orqali ishga tushiring.
2. Telefoningizda ochib, **"Ilovani Telefonga O'rnatish"** tugmasini bosing.
3. Ilova xuddi APK kabi telefoningiz ekraniga o'rnatiladi!

# AXIOUX — الموقع (نسخة مفصولة)

هذه النسخة هي نفس موقع `axioux.github.io` بعد:

- فصل CSS إلى `assets/css/styles.css`.
- فصل JavaScript إلى `assets/js/app.js`.
- تحديث فريق العمل إلى **8 أعضاء** (حُذف بشار، وحُذفت بطاقات قسّام ونورهان المكررة من الشبكة لأنهم في صف القيادة).
- تحديث التخصصات: Qassam/Nourhan = AI Agents & Automation، Abdulaziz = Backend & AI Agents، Batool = UI/UX & AI Agents، Lama = AI Solutions Architect، Jenan = Data Analysis & Backend، Saleh = Cybersecurity & Backend، Abdelrahman = Frontend & Data.
- تحديث البريد إلى `axioux3@gmail.com`.
- إضافة شريط **AT-Mind Early Access** أسفل الهيرو + خيار «أريد تجربة AT-Mind» في نموذج التواصل.
- إزالة Font Awesome (كل الأيقونات صارت SVG داخلي) لتقليل الطلبات.
- تقصير مدة شاشة البداية من 3.4 ثانية إلى حوالي 2.1 ثانية.
- إصلاح `robots.txt` و`sitemap.xml` (كانا يشيران إلى `axioux.com` غير العامل).
- إضافة صفحة `404.html`.

## بنية المجلد

```
axioux-site/
  index.html
  robots.txt
  sitemap.xml
  404.html
  assets/
    css/styles.css
    js/app.js
```

> **مهم:** ملف `assets/og.png` موجود أصلاً في الريبو ولا تلمسه. الدليل أعلاه يوضح الملفات التي نعدّلها فقط.

## طريقة النشر

1. خذ نسخة احتياطية من الريبو الحالي.
2. استبدل `index.html` بالنسخة الجديدة.
3. أضف `assets/css/styles.css` و`assets/js/app.js`.
4. استبدل `robots.txt` و`sitemap.xml`.
5. أضف `404.html`.
6. ارفع إلى GitHub Pages.

## إعدادات ما زالت مطلوبة منك

داخل `assets/js/app.js` → `SITE_CONFIG`:

```js
INSTAGRAM_URL: "",
TELEGRAM_URL: "",
LINKEDIN_URL: "",
CLOUDFLARE_ANALYTICS_TOKEN: "",
```

- عبّئ روابط إنستغرام/تلغرام/لينكدإن الشركة (أو اتركها فارغة مؤقتاً، الأيقونات ما تظهر).
- أضف توكن Cloudflare Web Analytics لقياس الزيارات وتسجيلات الـWaitlist.
- راجع رابط لينكدإن صالح: الرابط الحالي `linkedin.com/in/sameh-fer-...` يبدو أنه لحساب آخر — تأكد منه أو احذفه.

## اختبار محلي

شغّل سيرفر بسيط من داخل المجلد:

```powershell
powershell -NoProfile -ExecutionPolicy Bypass -File serve.ps1
```

ثم افتح `http://127.0.0.1:8766/`.

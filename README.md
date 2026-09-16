# MGE Scanner

تطبيق ويب خفيف لمسح باركود المنتجات، مع حفظ آخر 50 رمزًا محليًا، وقابل للتحويل إلى تطبيق Android عبر Capacitor.

## التشغيل المحلي

```bash
npm install
npx serve www
```

افتح العنوان الذي يعرضه الخادم، ثم اسمح للمتصفح باستخدام الكاميرا. يمكن استخدام الإدخال اليدوي إذا لم يدعم المتصفح `BarcodeDetector`.

## بناء تطبيق Android

يتطلب Android Studio وAndroid SDK مثبتين محليًا:

```bash
npx cap add android
npm run cap:sync
npx cap open android
```

يُبنى ملف APK تلقائيًا عند الدفع إلى فرع `main` أو عبر التشغيل اليدوي لسير العمل الموجود في `.github/workflows/build-apk.yml`.
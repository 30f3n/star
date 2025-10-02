STAR - LORD Image Host (Starter)
=================================

ملف تجريبي لتشغيل نسخة محلية بسيطة تحتوي على:
- backend: Express.js (index.js) يقوم باستقبال الصور، يضيف watermark من logo.png، يحفظ كـ webp ويعطي رابط قصير.
- frontend: صفحة ثابتة (frontend/index.html) للرفع والمعاينة.
- docker-compose لتشغيل الخادم بسهولة.

تشغيل محلي (بدون Docker):
1. انتقل إلى backend، ثبت الاعتماديات: `npm install`
2. ضع شعارك باسم `logo.png` داخل مجلد backend (تم تضمين لوجو تجريبي).
3. شغّل: `node index.js`
4. افتح http://localhost:4000

تشغيل باستخدام Docker:
1. تأكد أن Docker مثبت.
2. نفّذ: `docker compose up --build`
3. افتح http://localhost:4000

ملاحظات أمنية ومراجعات لاحقة:
- هذه نسخة مختصرة للبدء. في بيئة الإنتاج استخدم Postgres/S3/CDN، تحقق من الحماية، أضف auth، وقم بعمل اختبار تحميل كبير.

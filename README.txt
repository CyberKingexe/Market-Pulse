پروژه قیمت لحظه‌ای — PWA آماده GitHub Pages

ساختار:
index.html
manifest.json
sw.js
icons/
  icon-32.png
  icon-180.png
  icon-192.png
  icon-512.png
  icon-1040.png

نکته:
همه مسیرها نسبی هستند (./) تا روی GitHub Pages داخل Repository هم درست کار کنند.

آپلود:
1) محتوای این پوشه را داخل Repository سایت قرار بده.
2) مطمئن شو index.html در ریشه Repository سایت است.
3) پوشه icons و فایل‌های manifest.json و sw.js هم در همان ریشه باشند.
4) بعد از Deploy، اگر PWA قبلی نصب است، آن را حذف و دوباره نصب کن تا آیکون جدید از Manifest خوانده شود.

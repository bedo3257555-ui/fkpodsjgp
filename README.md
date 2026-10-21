# شرقاوي — المتابعة الغذائية والعلاجية والرياضية

تطبيق ويب (React + TanStack Start + Tailwind v4) لمتابعة النظام الغذائي والأدوية والتمارين والنوم والقياسات (InBody) والصور. الواجهة عربية RTL بوضع داكن.

## المتطلبات
- Node.js 20 أو أحدث

## التشغيل
```bash
npm install
npm run dev        # http://localhost:8080
```

## أوامر أخرى
```bash
npm run build      # بناء نسخة الإنتاج
npm run preview    # معاينة النسخة المبنية
npm run lint
npm test
```

## هيكل المشروع
```
src/
  routes/       الصفحات (index, nutrition, meds, training, sleep, measures, photos, insights, dossier)
  components/   مكونات الواجهة (shell, ui, charts)
  lib/          المنطق: analytics, clinical, store, format, auth, db
  styles.css    ستايل Tailwind
data/dossier.json   بيانات الملف الغذائي والعلاجي
styles.compiled.css نسخة الستايل المبنية
.grok/app-env.json  متغيرات البيئة (VITE_AUTH_ENABLED=false)
```

## ملاحظة خصوصية
`data/dossier.json` فيه بيانات صحية شخصية. لو الـ repo عام (Public) احذفه أو غيّر البيانات قبل الرفع.

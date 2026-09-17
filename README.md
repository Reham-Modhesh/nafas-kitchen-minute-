# Nafas — 60 Second Kitchen Manager

نسخة Render من ملف HTML المعدّل.

## Shared Leaderboard
النتائج تُحفظ في PostgreSQL بدل تخزين المتصفح، لذلك الجوالات المختلفة ترى نفس الأسماء والنتائج.

## Render
`render.yaml` ينشئ Web Service + PostgreSQL ويربط `DATABASE_URL` تلقائيًا.

Build Command:
`pip install -r requirements.txt`

Start Command:
`uvicorn main:app --host 0.0.0.0 --port $PORT`

ملاحظة: Render يذكر حاليًا أن Free Postgres بسعة 1GB وينتهي بعد 30 يومًا من إنشائه. مناسب للبوث القريب، أما التخزين طويل المدى فيحتاج قاعدة بيانات غير منتهية أو خطة مدفوعة.

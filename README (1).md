# لهجتي | Lahjti

مشروع «لهجتي» بالتعاون مع @SDAIA في برنامج معالجة اللغات التطبيقية

**لهجتي** مساعد ذكي في البنوك يستقبل طلب العميل نصًا أو صوتًا بلهجته المحلية (النجدية، الحجازية، القصيمية، إضافة إلى الفصحى)، فيفهم نيّته أولًا، ثم ينفّذ الخدمة المطلوبة، كالاستعلام عن الرصيد أو التحويل، بعد تأكيد صريح منه. (يغطي النموذج الأولي الإدخال النصي؛ انظر «حدود المشروع».)

يوضح المشروع كيف يمكن دمج نموذج لغوي مضبوط (Fine-tuned) مع قواعد استخراج المعلومات وخطوة تأكيد بشرية، لبناء مساعد يخدم من يصعب عليهم استخدام التطبيقات البنكية التقليدية.

> **تنبيه:** الحساب والأرصدة والمستفيدون **بيانات وهمية** لأغراض تعليمية، ولا يوجد أي ربط ببنك حقيقي.

---

## جرّب المساعد مباشرة

**الرابط:** [almudayani-kadi.github.io/lahjti-Banking-assistant](https://almudayani-kadi.github.io/lahjti-Banking-assistant/)

- يعمل مباشرة داخل المتصفح دون تسجيل أو تثبيت.
- أول تحميل للنموذج قد يستغرق نحو دقيقة، ثم يعمل بسرعة.
- أمثلة للتجربة: «وش رصيدي الحين»، «ابي احول لأبوي خمسمية»، «أبغى أحول لأخوي تلتمية».

يمكن أيضًا تشغيل النسخة الكاملة (واجهة Gradio) من الدفتر `lahjti.ipynb` في Google Colab.

---

## آلية العمل

1. **الاستماع والفهم:** تحديد اللهجة ونية العميل، واستخراج المعلومات مثل المبلغ واسم المستفيد.
2. **التنفيذ:** تنفيذ الخدمة المطلوبة بعد تأكيد العميل.

## التقنيات

- CAMeLBERT لتصنيف النية واستخراج الكيانات (NER)
- Sentence Transformers + FAISS + Cross-Encoder للبحث الدلالي
- Gradio لواجهة النسخة الكاملة

## حدود المشروع

- النموذج الأولي يدعم الإدخال النصي فقط، والإدخال الصوتي ضمن التطوير المستقبلي.
- جميع البيانات وهمية، ولا يوجد ربط بأي نظام بنكي حقيقي.

---

## English

**Lahjti** is a smart banking assistant that understands customer requests in Saudi dialects (Najdi, Hijazi, Qassimi) as well as Modern Standard Arabic. It identifies the customer's intent, extracts key details such as the amount and recipient, and executes services like balance inquiries and transfers after explicit confirmation. It is designed for people who find traditional banking apps hard to use, such as the elderly.

**Live demo:** [almudayani-kadi.github.io/lahjti-Banking-assistant](https://almudayani-kadi.github.io/lahjti-Banking-assistant/)

> All accounts, balances and beneficiaries are fictional, for educational purposes only.

---

إعداد: كادي المضياني
مشروع نهائي لمقرر معالجة اللغات التطبيقية — @SDAIA

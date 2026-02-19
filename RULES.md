# دليل قواعد استخدام المشروع - TailAdmin Laravel

## 🔹 المقدمة
هذا الدليل يوضح القواعد والإرشادات المتبعة في مشروع TailAdmin Laravel لضمان تناسق الكود وسهولة الصيانة.

## 📁 هيكل المجلدات
```
app/
├── Console/          # أوامر الأرتيزان المخصصة
├── Exceptions/       # معالجة الاستثناءات
├── Http/
│   ├── Controllers/ # المتحكمات
│   ├── Middleware/  # الوسائط
│   └── Requests/    # طلبات التحقق
├── Models/          # النماذج
└── Providers/       

resources/
├── css/             # ملفات CSS المخصصة
├── js/              # ملفات JavaScript
├── lang/            # ملفات الترجمة
└── views/           # قوالب Blade
    ├── components/  # المكونات القابلة لإعادة الاستخدام
    ├── layouts/     # الهياكل الأساسية
    └── pages/       # صفحات التطبيق
```

## 📝 قواعد الترميز

### 1. تسمية الملفات
- استخدم `PascalCase` للأصناف (Classes)
- استخدم `kebab-case` لملفات القوالب (Blade)
- استخدم `camelCase` للدوال والمتغيرات

### 2. قاعدة البيانات
- استخدم الهجرات (Migrations) لتعديل هيكل قاعدة البيانات
- استخدم المصانع (Factories) لإنشاء بيانات تجريبية
- استخدم البذور (Seeders) لملء البيانات الأولية

### 3. المتحكمات (Controllers)
- التزم بمبدأ التحكم الواحد (Single Responsibility)
- استخدم طلبات النماذج (Form Requests) للتحقق من صحة المدخلات
- استخدم الخدمات (Services) للتعامل مع المنطق المعقد

### 4. النماذج (Models)
- استخدم `PascalCase` لأسماء النماذج
- حدد الحقول القابلة للتعبئة في `$fillable`
- استخدم العلاقات (Relationships) عند الحاجة

### 5. القوالب (Views)
- استخدم مكونات Blade القابلة لإعادة الاستخدام
- تجنب كتابة JavaScript مضمن في القوالب
- استخدم ملفات الترجمة للنصوص

## 🛠️ الأدوات الموصى بها
- PHP 8.2+
- Composer
- Node.js 18+
- محرر أكواد يدعم Laravel (مثل: PHPStorm, VS Code)

## 🔄 سير العمل
1. إنشاء فرع (branch) جديد لكل ميزة
2. كتابة اختبارات الوحدة عند الإمكان
3. إجراء مراجعة الكود (Code Review)
4. دمج التغييرات مع الفرع الرئيسي

## 🚀 النشر
1. قم بتشغيل `composer install --optimize-autoloader --no-dev`
2. قم بتشغيل `npm run build`
3. اضبط `APP_ENV=production`
4. اضبط `APP_DEBUG=false`

## 📚 المصادر
- [توثيق Laravel](https://laravel.com/docs)
- [توثيق Tailwind CSS](https://tailwindcss.com/docs)
- [Alpine.js](https://alpinejs.dev/)

## 🔗 روابط مفيدة
- [إصدارات TailAdmin](https://tailadmin.com)
- [مستودع GitHub](https://github.com/TailAdmin/tailadmin-laravel)
- [الدليل الكامل](https://tailadmin.com/docs)

---
آخر تحديث: يناير 2025

# Store Ideal - نموذج متجر إلكتروني متكامل

🛒 **متجر إلكتروني احترافي على GitHub Pages** - قالب جاهز للاستخدام والتخصيص

## ✨ المميزات

### التصميم والأداء
- ✅ **تصميم عصري متجاوب** - يعمل على جميع الأجهزة
- ✅ **Dark Mode** - دعم الوضع الليلي تلقائياً
- ✅ **سريع جداً** - ملفات HTML ستاتيك بدون dependencies
- ✅ **Design System** - ألوان ومتغيرات CSS منظمة

### الوظائف
- ✅ **عرض منتجات احترافي** - بطاقات منتجات جذابة
- ✅ **بحث فوري** - بحث سريع في المنتجات
- ✅ **فلترة بالفئات** - 6 فئات رئيسية
- ✅ **ترتيب ذكي** - بالسعر، التقييم، الجديد
- ✅ **سلة تسوق تفاعلية** - إضافة وعرض المنتجات
- ✅ **إتمام عبر WhatsApp** - إرسال الطلب مباشرة
- ✅ **نظام تقييمات** - نجوم ومراجعات

### SEO والتحسين
- ✅ **Schema Markup** - بيانات منظمة للمنتجات
- ✅ **Meta Tags** - Open Graph للسوشيال ميديا
- ✅ **Sitemap.xml** - خريطة موقع جاهزة
- ✅ **Robots.txt** - توجيه محركات البحث
- ✅ **Semantic HTML** - عناصر HTML5 سيمانتيك

### PWA
- ✅ **Manifest.json** - تطبيق ويب تقدمي
- ✅ **أيقونات متعددة** - للأجهزة المختلفة
- ✅ **قابل للتثبيت** - يعمل كتطبيق عادي

## 🔗 الموقع المباشر

https://sherow1982.github.io/store-ideal/

## 📁 هيكل الملفات

```
store-ideal/
├── index.html              # الصفحة الرئيسية
├── product.html            # صفحة تفاصيل المنتج
├── about.html              # عن المتجر
├── contact.html            # اتصل بنا
├── privacy.html            # سياسة الخصوصية
├── terms.html              # شروط الخدمة
├── returns.html            # سياسة الإرجاع
├── 404.html                # صفحة الخطأ
├── products.json           # بيانات المنتجات
├── manifest.json           # PWA Manifest
├── sitemap.xml             # خريطة الموقع
├── robots.txt              # تعليمات محركات البحث
└── README.md               # دليل الاستخدام
```

## 🚀 كيفية الاستخدام

### 1. استنساخ المشروع (Fork)

1. اضغط على زر **Fork** في أعلى الصفحة
2. سيتم نسخ المشروع لحسابك

### 2. تفعيل GitHub Pages

1. اذهب إلى **Settings** → **Pages**
2. في **Source** اختر `main` branch
3. احفظ الإعدادات
4. انتظر دقيقة وافتح: `https://yourusername.github.io/store-ideal/`

### 3. تخصيص المتجر

#### تغيير رقم WhatsApp
في `index.html` ابحث عن:
```javascript
const whatsappNumber = '966501234567'; // غيّر لرقمك
```

#### إضافة منتجات جديدة
عدّل `products.json`:
```json
{
  "id": 13,
  "name": "اسم المنتج",
  "category": "electronics",
  "price": 299,
  "oldPrice": 399,
  "image": "https://your-image-url.jpg",
  "description": "وصف المنتج",
  "rating": 4.5,
  "reviews": 100,
  "badge": "جديد"
}
```

#### تغيير الألوان
في CSS غيّر المتغيرات:
```css
:root {
    --color-primary: rgba(33, 128, 141, 1);  /* لونك الرئيسي */
}
```

### 4. ربط دومين مخصص

1. أضف ملف `CNAME` في الجذر
2. ضع دومينك: `store.yourdomain.com`
3. في مزود الدومين أضف CNAME record:
```
store.yourdomain.com  →  yourusername.github.io
```

## 🛠️ التخصيص المتقدم

### إضافة Google Analytics

أضف قبل `</head>`:
```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_MEASUREMENT_ID');
</script>
```

### إضافة Facebook Pixel

أضف قبل `</head>`:
```html
<!-- Facebook Pixel -->
<script>
  !function(f,b,e,v,n,t,s)
  {if(f.fbq)return;n=f.fbq=function(){n.callMethod?
  n.callMethod.apply(n,arguments):n.queue.push(arguments)};
  if(!f._fbq)f._fbq=n;n.push=n;n.loaded=!0;n.version='2.0';
  n.queue=[];t=b.createElement(e);t.async=!0;
  t.src=v;s=b.getElementsByTagName(e)[0];
  s.parentNode.insertBefore(t,s)}(window, document,'script',
  'https://connect.facebook.net/en_US/fbevents.js');
  fbq('init', 'YOUR_PIXEL_ID');
  fbq('track', 'PageView');
</script>
```

## 🎯 أفضل الممارسات

### SEO
- ✅ غيّر `title` و `description` لكل صفحة
- ✅ استخدم صور محسّنة (WebP)
- ✅ أضف alt text لجميع الصور
- ✅ استخدم Schema markup للمنتجات

### الأداء
- ✅ ضغّط الصور (TinyPNG)
- ✅ استخدم CDN للصور
- ✅ Lazy loading للصور
- ✅ Minify CSS/JS للإنتاج

### الأمان
- ✅ استخدم HTTPS دائماً
- ✅ لا تخزّن بيانات حساسة
- ✅ Sanitize مدخلات المستخدم

## 📚 المصادر

- [GitHub Pages Docs](https://docs.github.com/en/pages)
- [Schema.org Products](https://schema.org/Product)
- [Open Graph Protocol](https://ogp.me/)
- [PWA Documentation](https://web.dev/progressive-web-apps/)

## 👥 الدعم

للمساعدة أو الاقتراحات:
- افتح Issue في GitHub
- راسلنا على [WhatsApp](https://wa.me/966501234567)

## 🛡️ الترخيص

MIT License - مجاني للاستخدام التجاري

## 🌟 تحديثات مستقبلية

- [ ] Service Worker للعمل Offline
- [ ] Multi-language Support
- [ ] ربط Shopify/WooCommerce API
- [ ] نظام مراجعات تفاعلي
- [ ] Wishlist و Compare
- [ ] فلترة بالسعر والتقييم

---

❤️ **مبني بحب للمجتمع العربي** | 🚀 **GitHub Pages Ready**
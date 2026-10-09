# نوین‌دارو — بازطراحی Frontend

این نسخه یک بازطراحی کامل و مستقل از فرانت‌اند قدیمی است و با HTML5 + CSS3 + Vanilla JavaScript ساخته شده؛ بدون npm و بدون نیاز به build.

## امکانات اصلی
- طراحی RTL و کاملاً واکنش‌گرا، موبایل‌محور
- هویت بصری جدید با سبز سلامت، فضای سفید و رنگ‌های تاکیدی کنترل‌شده
- صفحه خانه مدرن با Hero، دسته‌بندی، اعتماد، محصولات، خدمات و خبرنامه
- فروشگاه با جستجو، فیلتر دسته‌بندی و مرتب‌سازی
- صفحه جزئیات محصول با URL پارامتری
- سبد خرید واقعی سمت مرورگر با localStorage
- تغییر تعداد و حذف محصول
- checkout و صفحه تایید سفارش نمایشی
- ارسال نسخه با آپلود فایل و پیش‌نمایش نام فایل
- خدمات سلامت، درباره ما، تماس، سوالات متداول، مجله و مقاله
- دستیار هوشمند Frontend با پاسخ‌های مبتنی بر intent؛ آماده اتصال به API/LLM
- تم روشن/تیره
- Toast notification
- Wishlist نمایشی
- SEO پایه: title/description/canonical/OG/JSON-LD، sitemap و robots
- accessibility: skip link، label، focus، semantic HTML، alt و tap target مناسب
- فونت فارسی محلی و assetهای پروژه؛ بدون وابستگی به Google Fonts

## نکته مهم
این پروژه Frontend است. برای فروش واقعی دارو، احراز هویت، نسخه الکترونیک، پرداخت، موجودی، ارسال، CRM و چت‌بات واقعی باید Backend و API امن اضافه شود. همچنین داروهای نسخه‌ای نباید صرفاً بر اساس اطلاعات Frontend فروخته شوند.

## اجرا
فایل `index.html` را در مرورگر باز کنید یا پوشه را روی یک static server ساده اجرا کنید.


## Stage 1 bilingual upgrade
- English is the default language on first visit; Persian is available from the header. Preference is stored in localStorage.
- Document direction switches between LTR and RTL. Core navigation and common storefront labels have English equivalents. Longer editorial text remains Persian until fully localized; this is a partial translation release.
- Currency remains the original IRR/Toman catalogue values; English display uses IRR, **not** an invented USD exchange rate.
- Chat is a rule-based demo, not a live AI model. User chat text is inserted safely as text, not HTML. Do not enter sensitive health data.
- Cart, checkout, prescription upload, contact and newsletter are frontend demonstrations. No payment, order or prescription is sent to a server.
- Run using `python -m http.server 8000` and visit http://localhost:8000.
- Production TODO: full English content localization, secure backend, licensed pharmacy verification, secure prescription processing, real AI endpoint with privacy safeguards, and test suite.


## Stage 3: 3D-inspired page backgrounds
See `STAGE3_NOTES.md`. All pages use a locally bundled SVG medical background.


See STAGE4_NOTES.md for the latest visual improvements and remaining limitations.


See `STAGE5_NOTES.md` for the Stage 5 improvements and limitations.


## Stage 6
See [STAGE6_NOTES.md](STAGE6_NOTES.md) for wishlist functionality and limitations.


## Stage 7
See `STAGE7_NOTES.md` for page-specific backgrounds, privacy disclosure, and demo-service safeguards.

<!DOCTYPE html>
<style>
  /* زر الهامبرغر الاحترافي */
  .hamburger-menu {
    display: flex;
    flex-direction: column;
    gap: 5px;
    padding: 6px;
    cursor: pointer;
  }
  /* خلفية الـ Bottom Sheet */
#shareSheet {
  backdrop-filter: blur(4px);
  animation: fadeIn 0.3s ease;
}

/* محتوى المشاركة */
#shareContent {
  font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
  box-shadow: 0 -10px 30px rgba(0, 0, 0, 0.15);
  animation: slideUp 0.35s ease forwards;
}

/* شريط السحب */
#shareContent > div:first-child {
  background: linear-gradient(90deg, #e5e7eb, #9ca3af, #e5e7eb);
}

/* العنوان */
#shareContent h3 {
  font-size: 1.1rem;
  font-weight: 700;
  color: #111827;
}

/* أزرار الشبكات */
#shareContent a {
  text-decoration: none;
  font-size: 0.9rem;
  font-weight: 600;
  padding: 12px 14px;
  border-radius: 12px;
  background: #f3f4f6;
  color: #111827;
  min-width: 64px;
  text-align: center;
  transition: all 0.25s ease;
}

/* Hover */
#shareContent a:hover {
  transform: translateY(-3px);
  box-shadow: 0 6px 14px rgba(0, 0, 0, 0.15);
}

/* ألوان مخصصة */
#wa { background: #dcfce7; color: #166534; }
#fb { background: #dbeafe; color: #1e40af; }
#tg { background: #e0f2fe; color: #075985; }
#tw { background: #f1f5f9; color: #0f172a; }

/* زر الإغلاق */
#shareContent button {
  border: none;
  background: #111827;
  color: #fff;
  padding: 14px;
  border-radius: 14px;
  font-size: 0.95rem;
  font-weight: 600;
  cursor: pointer;
  transition: background 0.25s ease, transform 0.15s ease;
}

#shareContent button:hover {
  background: #000;
  transform: scale(0.98);
}

/* Animations */
@keyframes slideUp {
  from {
    transform: translateY(100%);
  }
  to {
    transform: translateY(0);
  }
}

@keyframes fadeIn {
  from {
    background: rgba(0, 0, 0, 0);
  }
  to {
    background: rgba(0, 0, 0, 0.5);
  }
}

/* تحسين للموبايل */
@media (max-width: 480px) {
  #shareContent a {
    font-size: 0.85rem;
    padding: 10px;
  }
}
  /* Active category button */
  .category-btn.active {
    --active-text-color: #ffffff;
    --active-icon-bg: rgba(255, 255, 255, 0.15);
    --active-icon-brightness: 1.1;
  }

  /* النص */
  .category-btn.active .btn-text {
    color: var(--active-text-color);
  }

  /* حاوية الأيقونة */
  .category-btn.active .icon-wrapper {
    background-color: var(--active-icon-bg);
  }

  /* الأيقونة نفسها */
  .category-btn.active svg {
    opacity: 1;
    filter: brightness(var(--active-icon-brightness));
  }

  /* إزالة أي تداخل من الـ CSS السابق */
  .category-btn.active div,
  .category-btn.active svg {
    color: initial !important;
    background-color: initial !important;
  }
  .category-btn.active .btn-text {
    color: white !important;
  }

  /* إلغاء أي تأثير على الأيقونات - تبقى بألوانها الأصلية */
  .category-btn.active div,
  .category-btn.active svg {
    color: inherit !important;
    background-color: inherit !important;
  }
  /* إصلاح التباعد في الإعدادات حسب اللغة */
  .settings-item .flex {
    gap: 1rem; /* مسافة ثابتة بين الأيقونة والنص */
  }

  /* للغة العربية - الاتجاه الافتراضي */
  .settings-item .flex.items-center.space-x-4.space-x-reverse {
    gap: 1rem;
    margin-left: 0;
    margin-right: 0;
  }

  /* للغات LTR (الإنجليزية والفرنسية) */
  .lang-english .settings-item .flex,
  .lang-french .settings-item .flex {
    gap: 1rem;
    flex-direction: row;
  }

  /* إزالة المسافات الافتراضية وتطبيق gap */
  .settings-item .space-x-4 > * + * {
    margin-left: 0 !important;  /*  توقف*/
    margin-right: 0 !important;
  }

  .lang-english .settings-item .space-x-reverse > * + *,
  .lang-french .settings-item .space-x-reverse > * + * {
    margin-left: 0 !important;
    margin-right: 0 !important;
  }

  /* ضمان توحيد المسافات في جميع اللغات */
  .settings-item .w-10 {
    margin-left: 0;
    margin-right: 0;
    flex-shrink: 0;
  }
  /* النص فقط أبيض */
  .category-btn.active .btn-text {
    color: white !important;
  }

  /* إلغاء أي تأثير على الأيقونات - تبقى بألوانها الأصلية */
  .category-btn.active div,
  .category-btn.active svg {
    color: inherit !important;
    background-color: inherit !important;
  }

  /* إعادة تطبيق الألوان الأصلية للأيقونات */
  .category-btn.active svg[class*="text-"] {
    color: var(--tw-text-opacity, 1) !important;
  }

  #favoriteBtn.active {
    background-color: #ff4d4d; /* لون أحمر كمثال */
    color: white;
    /* بدون pointer-events:none */
    cursor: pointer;
  }
  .favorites-empty-container {
    position: relative;
    z-index: 10;
    pointer-events: auto; /* باش يكون قابل للتفاعل فقط داخل div */
  }

  .bottom-nav {
    position: fixed;
    bottom: 0;
    left: 0;
    right: 0;
    z-index: 50; /* فوق كل شيء */
  }

  .bottom-nav .nav-item:active,
  .bottom-nav .nav-item:focus {
    color: #28c7ed; /* لون FLUXY */
  }

  .bottom-nav .nav-item:active svg,
  .bottom-nav .nav-item:focus svg {
    stroke: #28c7ed;
  }
  /* الشريط السفلي */
  .bottom-nav {
    background-color: #ffffff; /* خلفية عادية */
    border-top: 1px solid #e5e7eb;
    box-shadow: 0 -2px 8px rgba(0, 0, 0, 0.05);
    padding: 8px 0;
    z-index: 50;
  }

  .dark .bottom-nav {
    background-color: #1f2937;
    border-color: #374151;
  }

  /* كل زر */
  .bottom-nav .nav-item {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    padding: 6px 8px;
    color: #6b7280; /* رمادي فاتح */
    transition: all 0.25s ease;
    border-radius: 12px;
  }

  /* أيقونات */
  .bottom-nav .nav-item svg {
    width: 24px;
    height: 24px;
    margin-bottom: 2px;
    transition: all 0.25s ease;
  }

  /* النص */
  .bottom-nav .nav-item span {
    font-size: 10px;
  }

  /* عند الضغط أو اختيار الزر */
  .bottom-nav .nav-item.active {
    color: #28c7ed; /* لون FLUXY */
  }

  .bottom-nav .nav-item.active svg {
    stroke: #28c7ed;
  }

  /* تأثير hover خفيف */
  .bottom-nav .nav-item:hover {
    background-color: rgba(40, 199, 237, 0.1);
  }
  /* شكل أنيق لمربع البحث */
  #homeSearchInput {
    height: 55px; /* كبر الحجم */
    border-radius: 16px; /* زوايا كبيرة */
    font-size: 17px; /* خط أوضح */
    padding-left: 50px; /* مساحة قبل النص */
    background: #fff;
    border: 1px solid #dcdcdc; /* برواز خفيف */
    box-shadow: 0 3px 12px rgba(0, 0, 0, 0.08); /* ظل احترافي */
    transition: 0.25s ease;
  }
  #homeSearchInput {
    caret-color: #28c7ed; /* لون المؤشر */
  }
  #homeSearchInput {
    color: #000000 !important; /* نص أبيض */
  }

  .dark #homeSearchInput {
    color: #000000 !important; /* نص واضح أكثر في الوضع المظلم */
  }

  /* عند الضغط */
  #homeSearchInput:focus {
    border-color: #4e5bff; /* لون يشبه الأزرق الفاتح */
    box-shadow: 0 4px 14px rgba(78, 91, 255, 0.25);
  }
  /* الحقل كامل */
  #searchInput {
    background: #ffffff; /* خلفية نظيفة */
    border: 2px solid #e5e7eb; /* إطار خفيف */
    border-radius: 14px; /* زوايا ناعمة */
    padding: 12px 45px 12px 16px; /* مساحة داخلية */
    font-size: 16px;
    transition: all 0.25s ease;
    caret-color: #28c7ed; /* لون خط الكتابة */
  }

  /* أيقونة البحث */
  #searchInput + div svg {
    width: 20px;
    height: 20px;
    opacity: 0.6;
  }

  /* الـ Placeholder */
  #searchInput::placeholder {
    color: #9ca3af;
    opacity: 1;
  }

  /* عند التركيز */
  #searchInput:focus {
    border-color: #28c7ed;
    box-shadow: 0 0 0 3px rgba(40, 199, 237, 0.25);
    outline: none;
  }

  /* الوضع المظلم */
  .dark #searchInput {
    background: #111827; /* نفس ستايل الآخر */
    border-color: #374151;
    color: #e5f8ff; /* نص واضح */
  }

  /* Placeholder في المظلم */
  .dark #searchInput::placeholder {
    color: #7abdd4;
  }

  /* إزالة المربع الأسود الداخلي */
  .dark #searchInput:focus {
    background: #111827;
  }

  #homeSearchInput:focus {
    outline: none !important;
    box-shadow: 0 0 0 3px rgba(0, 152, 218, 0.3); /* تأثير لطيف */
    border-color: #0098da;
  }

  /* تعديل أيقونة البحث */
  #homeSearchInput + div svg {
    width: 22px;
    height: 22px;
    color: #9aa0a6; /* لون أنيق مثل Google */
  }

  .hamburger-line {
    width: 26px;
    height: 3px;
    background: linear-gradient(to right, #0098da, #28c7ed);
    border-radius: 4px;
    transition: 0.3s ease;
  }
  /* تحديث سمك خطوط الهامبرغر */
  .hamburger-line {
    height: 4px !important;
    border-radius: 2px !important;
  }
  #hamburgerBtn {
    padding: 4px; /* أو أي حجم تريده */
    width: 30px; /* عرض ثابت */
    height: 26px; /* ارتفاع ثابت */
  }

  /* Switches الحديثة */
  .toggle-switch-modern {
    background-color: #e5e7eb;
    position: relative;
    transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
    box-shadow: inset 0 1px 3px rgba(0, 0, 0, 0.1);
  }

  .toggle-switch-modern:hover {
    transform: scale(1.05);
  }

  .toggle-switch-modern.active {
    background: linear-gradient(135deg, #0098da, #28c7ed);
    box-shadow: 0 4px 15px rgba(0, 152, 218, 0.4);
  }

  .dark .toggle-switch-modern.inactive {
    background-color: #4b5563;
  }

  .toggle-circle-modern {
    position: absolute;
    top: 2px;
    width: 24px;
    height: 24px;
    background: white;
    border-radius: 50%;
    transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
    box-shadow: 0 2px 8px rgba(0, 0, 0, 0.15), 0 1px 2px rgba(0, 0, 0, 0.1);
    display: flex;
    align-items: center;
    justify-content: center;
  }

  .toggle-circle-modern.left {
    left: 2px;
  }

  .toggle-circle-modern.right {
    right: 2px;
  }

  .toggle-circle-modern::after {
    content: "";
    width: 12px;
    height: 12px;
    border-radius: 50%;
    background: rgba(0, 152, 218, 0.2);
    transition: all 0.2s ease;
    opacity: 0;
  }

  .toggle-switch-modern.active .toggle-circle-modern::after {
    opacity: 1;
    background: rgba(255, 255, 255, 0.3);
  }

  /* تحسينات إضافية للإعدادات */
  .settings-item {
    transition: all 0.2s ease;
  }

  .settings-item:hover {
    transform: translateX(-2px);
  }

  .lang-english .settings-item:hover,
  .lang-french .settings-item:hover {
    transform: translateX(2px);
  }

  /* تحسين قسم المفضلة الفارغة */
  .favorites-empty-container {
    text-align: center;
    padding: 3rem 1.5rem;
    max-width: 400px;
    margin: 0 auto;
  }

  .favorites-empty-heart {
    width: 120px;
    height: 120px;
    background: linear-gradient(135deg, #ff6b6b, #ee5a52);
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    margin: 0 auto 2rem;
    box-shadow: 0 8px 30px rgba(255, 107, 107, 0.3);
    animation: heartbeat 2s ease-in-out infinite;
  }

  .favorites-empty-heart svg {
    width: 60px;
    height: 60px;
    color: white;
    filter: drop-shadow(0 2px 4px rgba(0, 0, 0, 0.1));
  }

  @keyframes heartbeat {
    0%,
    100% {
      transform: scale(1);
    }
    50% {
      transform: scale(1.05);
    }
  }

  .dark .favorites-empty-heart {
    background: linear-gradient(135deg, #dc2626, #b91c1c);
    box-shadow: 0 8px 30px rgba(220, 38, 38, 0.4);
  }

  .favorites-empty-title {
    font-size: 1.5rem;
    font-weight: 700;
    color: #1f2937;
    margin-bottom: 0.75rem;
    line-height: 1.3;
  }

  .dark .favorites-empty-title {
    color: #f9fafb;
  }

  .favorites-empty-desc {
    font-size: 1rem;
    color: #6b7280;
    margin-bottom: 2rem;
    line-height: 1.6;
  }

  .dark .favorites-empty-desc {
    color: #9ca3af;
  }

  .favorites-add-btn {
    background: linear-gradient(135deg, #0098da, #28c7ed);
    color: white;
    padding: 1rem 2rem;
    border-radius: 1rem;
    font-weight: 600;
    font-size: 1.1rem;
    border: none;
    cursor: pointer;
    box-shadow: 0 4px 20px rgba(0, 152, 218, 0.3);
    transition: all 0.3s ease;
    display: inline-flex;
    align-items: center;
    gap: 0.75rem;
    margin-bottom: 1rem;
  }

  .favorites-add-btn:hover {
    transform: translateY(-2px);
    box-shadow: 0 6px 25px rgba(0, 152, 218, 0.4);
    background: linear-gradient(135deg, #0086c3, #25b5d9);
  }

  .favorites-add-btn:active {
    transform: translateY(0);
  }

  .favorites-add-btn svg {
    width: 20px;
    height: 20px;
  }

  .favorites-add-desc {
    font-size: 0.9rem;
    color: #6b7280;
    line-height: 1.5;
    max-width: 300px;
    margin: 0 auto;
  }

  .dark .favorites-add-desc {
    color: #9ca3af;
  }
</style>

<html lang="ar" dir="rtl">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>مكتبة التطبيقات</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
      tailwind.config = {
        darkMode: "class",
        theme: {
          extend: {
            colors: {
              primary: "#0098DA",
              secondary: "#28C7ED",
              dark: {
                bg: "#0f0f0f",
                surface: "#1a1a1a",
                card: "#262626",
              },
            },
          },
        },
      };
    </script>
    <style>
      body {
        font-family: "Tahoma", "Arian", sans-serif;
        transition: background-color 0.3s ease, color 0.3s ease;
      }

      /* English font override */
      .lang-english body {
        font-family: "Inter", "Arial", sans-serif;
      }

      /* French font override */
      .lang-french body {
        font-family: "Inter", "Arial", sans-serif;
      }

      /* إخفاء شريط التمرير */
      .scrollbar-hide {
        -ms-overflow-style: none;
        scrollbar-width: none;
      }
      .scrollbar-hide::-webkit-scrollbar {
        display: none;
      }

      /* شريط التنقل السفلي */
      .bottom-nav {
        backdrop-filter: blur(10px);
        -webkit-backdrop-filter: blur(10px);
        border-top: 1px solid rgba(255, 255, 255, 0.1);
        transition: all 0.3s ease;
      }

      .nav-item {
        transition: all 0.3s ease;
        position: relative;
      }

      .nav-item.active {
        color: #0098da;
      }

      .nav-item.active::before {
        content: "";
        position: absolute;
        top: -2px;
        left: 50%;
        transform: translateX(-50%);
        width: 4px;
        height: 4px;
        background: #0098da;
        border-radius: 50%;
      }

      .nav-item:hover {
        transform: translateY(-2px);
      }

      /* تحديد مساحة للشريط السفلي */
      .main-content {
        padding-bottom: 100px;
        padding-top: 20px; /* مساحة مقللة لشريط التنقل العلوي */
      }

      /* إخفاء المحتوى غير النشط */
      .content-section {
        display: none;
      }

      .content-section.active {
        display: block;
      }

      /* تأثيرات التطبيقات مع الوضع المظلم */
      .app-card {
        transition: transform 0.2s ease, box-shadow 0.2s ease,
          background-color 0.3s ease, border-color 0.3s ease;
      }
      .app-card:hover {
        transform: translateY(-5px);
        box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
      }
      .dark .app-card:hover {
        box-shadow: 0 10px 25px rgba(0, 0, 0, 0.3);
      }

      /* تصميم أزرار التصنيفات مع الوضع المظلم */
      .category-btn {
        background: linear-gradient(135deg, #f8fafc, #e2e8f0);
        color: #0098da;
        border: 1px solid #e2e8f0;
        position: relative;
        overflow: hidden;
        transition: all 0.3s ease;
      }

      .category-btn::before {
        content: "";
        position: absolute;
        top: 0;
        left: 0;
        right: 0;
        bottom: 0;
        background: linear-gradient(135deg, #0098da, #28c7ed);
        opacity: 0;
        transition: opacity 0.3s ease;
        z-index: 0;
      }

      .category-btn span,
      .category-btn .btn-text {
        position: relative;
        z-index: 1;
      }

      .category-btn:hover {
        transform: translateY(-2px);
        box-shadow: 0 8px 20px rgba(0, 152, 218, 0.3);
      }

      .category-btn:hover::before {
        opacity: 0.1;
      }

      .category-btn.active {
        background: linear-gradient(135deg, #0098da, #28c7ed);
        color: white;
        border-color: #0098da;
        box-shadow: 0 6px 20px rgba(0, 152, 218, 0.4);
      }

      .category-btn.active::before {
        opacity: 1;
      }

      /* الوضع المظلم المحسن */
      .dark {
        background-color: #0f0f0f;
      }

      .dark .category-btn {
        background: linear-gradient(135deg, #1f2937, #374151);
        color: #9ca3af;
        border-color: #374151;
      }

      .dark .category-btn:hover {
        background: linear-gradient(135deg, #374151, #4b5563);
        box-shadow: 0 8px 20px rgba(0, 152, 218, 0.4);
      }

      .dark .category-btn.active {
        background: linear-gradient(135deg, #0098da, #28c7ed);
        color: white;
        border-color: #0098da;
      }

      /* تحسينات إضافية للوضع المظلم */
      .dark .main-content {
        background-color: #0f0f0f;
      }

      .dark .bottom-nav {
        background-color: rgba(15, 15, 15, 0.9);
        border-top-color: rgba(55, 65, 81, 0.3);
      }

      /* تأثير التمرير الناعم */
      .category-carousel-container {
        position: relative;
      }

      .scroll-btn {
        transition: all 0.3s ease;
        backdrop-filter: blur(10px);
      }

      .scroll-btn:hover {
        transform: scale(1.1);
        box-shadow: 0 8px 25px rgba(0, 0, 0, 0.15);
      }

      /* تأثيرات النافذة المنبثقة مع الوضع المظلم */
      .modal-backdrop {
        backdrop-filter: blur(5px);
        animation: fadeIn 0.3s ease;
      }
      .modal-content {
        animation: slideUp 0.3s ease;
        position: relative;
      }
      @keyframes fadeIn {
        from {
          opacity: 0;
        }
        to {
          opacity: 1;
        }
      }
      @keyframes slideUp {
        from {
          opacity: 0;
          transform: translateY(30px) scale(0.95);
        }
        to {
          opacity: 1;
          transform: translateY(0) scale(1);
        }
      }

      /* تصميم بطاقات الملف الشخصي */
      .profile-card {
        background: linear-gradient(135deg, #0098da, #28c7ed);
      }

      .settings-item {
        transition: all 0.2s ease;
      }

      .settings-item:hover {
        background-color: rgba(0, 152, 218, 0.05);
      }

      .dark .settings-item:hover {
        background-color: rgba(0, 152, 218, 0.1);
      }

      /* تأثيرات مفتاح التبديل مع الوضع المظلم */
      .toggle-switch {
        position: relative;
        transition: all 0.3s ease;
      }

      .toggle-switch.active {
        background-color: #0098da;
      }

      .toggle-switch.inactive {
        background-color: #d1d5db;
      }

      .dark .toggle-switch.inactive {
        background-color: #4b5563;
      }

      .toggle-circle {
        position: absolute;
        top: 0.125rem;
        width: 1.25rem;
        height: 1.25rem;
        background: white;
        border-radius: 50%;
        transition: all 0.3s ease;
        box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
      }

      .toggle-circle.right {
        right: 0.125rem;
      }

      .toggle-circle.left {
        left: 0.125rem;
      }

      /* زر الوضع المظلم السريع */
      .dark-mode-toggle {
        transition: all 0.3s ease;
      }

      .dark-mode-toggle:hover {
        transform: scale(1.1);
      }

      /* تحسينات الألوان للوضع المظلم */
      .dark input {
        background-color: #1f2937;
        border-color: #374151;
        color: #f3f4f6;
      }

      .dark input:focus {
        border-color: #0098da;
        background-color: #1f2937;
      }

      .dark input::placeholder {
        color: #6b7280;
      }

      /* إشعارات محسنة للوضع المظلم */
      .notification {
        transition: all 0.3s ease;
      }

      .dark .notification {
        background-color: #1f2937;
        border: 1px solid #374151;
        color: #f3f4f6;
      }

      /* تحسينات النوافذ المنبثقة */
      .dark .modal-content {
        background-color: #1a1a1a;
        border: 1px solid #374151;
      }

      /* شريط التنقل العلوي المحسن */
      .top-navbar {
        background: rgba(255, 255, 255, 0.95);
        backdrop-filter: blur(10px);
        -webkit-backdrop-filter: blur(10px);
        border-bottom: 1px solid rgba(0, 0, 0, 0.1);
        transition: all 0.3s ease;
        position: sticky;
        top: 0;
        z-index: 40;
      }

      .dark .top-navbar {
        background: rgba(15, 15, 15, 0.95);
        border-bottom: 1px solid rgba(255, 255, 255, 0.1);
      }

      /* تحسين عرض الشعار والنص */
      .app-logo-section {
        min-width: 0; /* للسماح بانكماش النص عند الحاجة */
      }

      .app-logo-section h1 {
        font-size: 1rem;
        line-height: 1.2;
      }

      .app-logo-section p {
        font-size: 0.75rem;
        line-height: 1.1;
        margin-top: 1px;
      }

      @media (min-width: 640px) {
        .app-logo-section h1 {
          font-size: 1.125rem;
        }
        .app-logo-section p {
          font-size: 0.8rem;
        }
      }

      @media (min-width: 768px) {
        .app-logo-section h1 {
          font-size: 1.25rem;
        }
        .app-logo-section p {
          font-size: 0.85rem;
        }
      }

      .hamburger-menu {
        width: 24px;
        height: 18px;
        position: relative;
        cursor: pointer;
        transition: all 0.3s ease;
        margin-right: 0px; /* ملتصق بالزاوية */
        margin-left: 0px; /* بدون هامش إضافي */
      }

      .hamburger-line {
        position: absolute;
        width: 100%;
        height: 2px;
        background-color: #374151;
        transition: all 0.3s ease;
        border-radius: 1px;
      }

      .dark .hamburger-line {
        background-color: #d1d5db;
      }

      .hamburger-line:nth-child(1) {
        top: 0;
      }
      .hamburger-line:nth-child(2) {
        top: 50%;
        transform: translateY(-50%);
      }
      .hamburger-line:nth-child(3) {
        bottom: 0;
      }

      .hamburger-menu.active .hamburger-line:nth-child(1) {
        top: 50%;
        transform: translateY(-50%) rotate(45deg);
      }

      .hamburger-menu.active .hamburger-line:nth-child(2) {
        opacity: 0;
      }

      .hamburger-menu.active .hamburger-line:nth-child(3) {
        bottom: 50%;
        transform: translateY(50%) rotate(-45deg);
      }

      /* قائمة التنقل الجانبية */
      .side-menu {
        position: fixed;
        top: 0;
        right: -300px;
        width: 300px;
        height: 100vh;
        background: rgba(255, 255, 255, 0.98);
        backdrop-filter: blur(15px);
        -webkit-backdrop-filter: blur(15px);
        border-left: 1px solid rgba(0, 0, 0, 0.1);
        transition: right 0.3s ease;
        z-index: 50;
        padding: 20px;
        overflow-y: auto;
      }

      .dark .side-menu {
        background: rgba(15, 15, 15, 0.98);
        border-left: 1px solid rgba(255, 255, 255, 0.1);
      }

      .side-menu.active {
        right: 0;
      }

      .menu-overlay {
        position: fixed;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background: rgba(0, 0, 0, 0.5);
        z-index: 45;
        opacity: 0;
        visibility: hidden;
        transition: all 0.3s ease;
      }

      .menu-overlay.active {
        opacity: 1;
        visibility: visible;
      }

      .menu-item {
        display: flex;
        align-items: center;
        padding: 12px 16px;
        margin: 8px 0;
        border-radius: 12px;
        transition: all 0.2s ease;
        cursor: pointer;
        color: #374151;
      }

      .dark .menu-item {
        color: #d1d5db;
      }

      .menu-item:hover {
        background: rgba(0, 152, 218, 0.1);
        transform: translateX(-4px);
      }

      .menu-item.active {
        background: linear-gradient(135deg, #0098da, #28c7ed);
        color: white;
        box-shadow: 0 4px 15px rgba(0, 152, 218, 0.3);
      }

      .menu-item-icon {
        width: 20px;
        height: 20px;
        margin-left: 12px;
      }

      .top-search {
        background: rgba(248, 250, 252, 0.9);
        border: 1px solid rgba(226, 232, 240, 0.8);
      }

      .dark .top-search {
        background: rgba(31, 41, 55, 0.9);
        border: 1px solid rgba(55, 65, 81, 0.8);
      }

      .top-search:focus {
        background: rgba(255, 255, 255, 1);
        box-shadow: 0 0 0 3px rgba(0, 152, 218, 0.1);
      }

      .dark .top-search:focus {
        background: rgba(31, 41, 55, 1);
      }

      /* تصميم carousel الأقسام */
      .section-carousel {
        position: relative;
      }

      .carousel-btn {
        opacity: 0;
        transition: all 0.3s ease;
        border: 1px solid rgba(0, 0, 0, 0.1);
      }

      .dark .carousel-btn {
        border: 1px solid rgba(255, 255, 255, 0.1);
      }

      .section-carousel:hover .carousel-btn {
        opacity: 1;
      }

      .carousel-btn:hover {
        transform: translateY(-50%) scale(1.1);
        box-shadow: 0 8px 25px rgba(0, 0, 0, 0.15);
      }

      .dark .carousel-btn:hover {
        box-shadow: 0 8px 25px rgba(0, 0, 0, 0.3);
      }

      /* بطاقات التطبيقات في carousel */
      .carousel-app-card {
        width: 140px;
        flex-shrink: 0;
        transition: transform 0.2s ease, box-shadow 0.2s ease;
      }

      .carousel-app-card:hover {
        transform: translateY(-5px);
        box-shadow: 0 8px 20px rgba(0, 0, 0, 0.1);
      }

      .dark .carousel-app-card:hover {
        box-shadow: 0 8px 20px rgba(0, 0, 0, 0.3);
      }

      .carousel-app-image {
        width: 100%;
        height: 100px;
        object-fit: cover;
        border-radius: 12px;
      }

      .carousel-app-badge {
        position: absolute;
        top: 8px;
        right: 8px;
        background: linear-gradient(135deg, #0098da, #28c7ed);
        color: white;
        font-size: 10px;
        padding: 2px 6px;
        border-radius: 6px;
        font-weight: 500;
      }

      /* RTL direction for English and French */
      .lang-english,
      .lang-french {
        direction: ltr;
      }

      .lang-english .side-menu,
      .lang-french .side-menu {
        right: auto;
        left: -300px;
        border-left: none;
        border-right: 1px solid rgba(0, 0, 0, 0.1);
      }

      .dark .lang-english .side-menu,
      .dark .lang-french .side-menu {
        border-right: 1px solid rgba(255, 255, 255, 0.1);
      }

      .lang-english .side-menu.active,
      .lang-french .side-menu.active {
        left: 0;
      }

      .lang-english .menu-item:hover,
      .lang-french .menu-item:hover {
        transform: translateX(4px);
      }

      .lang-english .settings-item:hover,
      .lang-french .settings-item:hover {
        transform: translateX(5px);
      }

      .lang-english .menu-item-icon,
      .lang-french .menu-item-icon {
        margin-left: 0;
        margin-right: 12px;
      }

      .lang-english .carousel-app-badge,
      .lang-french .carousel-app-badge {
        right: auto;
        left: 8px;
      }

      /* تحسينات للصفحات المتعددة */
      .pagination-enhanced {
        background: rgba(255, 255, 255, 0.9);
        backdrop-filter: blur(10px);
        border-radius: 16px;
        padding: 16px;
        border: 1px solid rgba(0, 0, 0, 0.1);
      }

      .dark .pagination-enhanced {
        background: rgba(26, 26, 26, 0.9);
        border: 1px solid rgba(255, 255, 255, 0.1);
      }

      .page-btn {
        transition: all 0.2s ease;
        min-width: 40px;
        height: 40px;
        display: flex;
        align-items: center;
        justify-content: center;
      }

      .page-btn:hover:not(:disabled) {
        transform: translateY(-2px);
        box-shadow: 0 4px 12px rgba(0, 152, 218, 0.3);
      }

      .page-btn.active {
        background: linear-gradient(135deg, #0098da, #28c7ed);
        color: white;
        box-shadow: 0 4px 15px rgba(0, 152, 218, 0.4);
      }

      .apps-grid-enhanced {
        display: grid;
        grid-template-columns: repeat(auto-fill, minmax(160px, 1fr));
        gap: 20px;
      }

      @media (max-width: 640px) {
        .apps-grid-enhanced {
          grid-template-columns: repeat(auto-fill, minmax(140px, 1fr));
          gap: 16px;
        }
      }

      /* مؤشر التحميل */
      .loading-indicator {
        animation: pulse 2s cubic-bezier(0.4, 0, 0.6, 1) infinite;
      }

      @keyframes pulse {
        0%,
        100% {
          opacity: 1;
        }
        50% {
          opacity: 0.5;
        }
      }

      /* زر الرجوع المخصص */
      .back-btn {
        transition: all 0.2s ease;
      }

      .back-btn:hover {
        transform: translateX(-2px);
      }

      .lang-english .back-btn:hover,
      .lang-french .back-btn:hover {
        transform: translateX(2px);
      }
    </style>
    <style>
  /* نحيد أي glow أو shadow */
  .category-btn,
  .category-btn:hover,
  .category-btn:focus,
  .category-btn:active {
    box-shadow: none !important;
    outline: none !important;
    filter: none !important;
  }

  /* نحيد أي تأثير على الدوائر */
  .category-btn > div {
    box-shadow: none !important;
    filter: none !important;
  }

  /* نحيد أي transition ضوئي */
  .category-btn,
  .category-btn * {
    transition: none !important;
  }
</style>
  </head>
  <body
    class="bg-gray-50 dark:bg-dark-bg min-h-screen transition-colors duration-300"
  >
    <!-- شريط التنقل العلوي المحسن -->
    <nav class="top-navbar">
      <div class="max-w-6xl mx-auto px-3 py-3">
        <div class="flex items-center justify-between">
          <!-- قائمة الهامبرغر والشعار -->
          <div class="flex items-center gap-4">
            <button
              id="hamburgerBtn"
              class="hamburger-menu p-2"
              onclick="toggleSideMenu()"
            >
              <div class="hamburger-line"></div>
              <div class="hamburger-line"></div>
              <div class="hamburger-line"></div>
            </button>

            <!-- شعار التطبيق مع الاسم المحسن -->
            <div class="flex items-center gap-2">
              <img
                src="https://pfst.cf2.poecdn.net/base/image/2941d35e0a5c2d3f37779cecb6ac36cc243699a07e24afc34a576cc83cb72544?w=500&h=500"
                alt="شعار FLUXY"
                class="w-9 h-9 rounded-lg flex-shrink-0"
              />
              <div class="flex flex-col">
                <h1
                  id="appTitle"
                  class="font-extrabold !text-3xl tracking-wider bg-gradient-to-r from-[#0098DA] to-[#28C7ED] text-transparent bg-clip-text leading-tight uppercase drop-shadow-sm select-none"
                >
                  FLUXY
                </h1>
                <p
                  id="appTagline"
                  class="text-gray-500 dark:text-gray-400 leading-tight hidden sm:block truncate"
                >
                  اكتشف تطبيقاتك المفضلة
                </p>
              </div>
            </div>
          </div>

          <!-- مساحة فارغة للتوسيط -->
          <div class="flex-1"></div>

          <!-- أزرار الإجراءات -->
          <div class="flex items-center gap-2">
            <!-- زر البحث -->
            <button
              id="searchToggleBtn"
              class="p-2 transition-all duration-200 hover:scale-110"
              style="color: #0098da"
              onclick="toggleSearch()"
            >
              <svg
                class="w-7 h-7 stroke-[2.5]"
                fill="none"
                stroke="currentColor"
                viewBox="0 0 24 24"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z"
                ></path>
              </svg>
            </button>

            <!-- زر الوضع المظلم -->
            <button
              id="quickDarkModeToggle"
              class="dark-mode-toggle p-2 transition-all duration-200 hover:scale-110"
              style="color: #0098da"
              onclick="toggleNotifications()"
            >
              <svg
                id="darkModeIcon"
                class="w-7 h-7 stroke-[2.5]"
                fill="none"
                stroke="#0098da"
                viewBox="0 0 24 24"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M15 17h5l-1.405-1.405
                  A2.032 2.032 0 0118 14.158V11
                  a6 6 0 00-4-5.659V5
                  a2 2 0 10-4 0v.341
                  C7.67 6.165 6 8.388 6 11v3.159
                  c0 .538-.214 1.055-.595 1.436L4 17h5
                  m6 0a3 3 0 11-6 0"
                ></path>
              </svg>
            </svg>

            <svg id="lightModeIcon" class="w-7 h-7 stroke-[2.5] hidden" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                      d="M15 17h5l-1.405-1.405
                          A2.032 2.032 0 0118 14.158V11
                          a6 6 0 00-4-5.659V5
                          a2 2 0 10-4 0v.341
                          C7.67 6.165 6 8.388 6 11v3.159
                          c0 .538-.214 1.055-.595 1.436L4 17h5
                          m6 0a3 3 0 11-6 0">
                </path>
            </svg>
        </button>
              <svg id="lightModeIcon" class="w-7 h-7 stroke-[2.5] hidden"></svg>
            </button>
          </div>
        </div>
      </div>
    </nav>
    <div
      id="notificationsPanel"
      class="fixed top-20 right-4 w-80 bg-white dark:bg-gray-800 shadow-xl rounded-xl hidden z-50"
    >
      <div
        class="flex items-center justify-between px-4 py-3 border-b border-gray-200 dark:border-gray-700"
      >
        <span class="font-semibold text-gray-800 dark:text-white">
          الإشعارات
        </span>

        <button
          onclick="closeNotifications()"
          class="text-gray-500 hover:text-red-500 text-xl font-bold"
        >
          ×
        </button>
      </div>

      <div class="p-4 text-sm text-gray-600 dark:text-gray-300">
        🔔 لا توجد إشعارات جديدة
      </div>
    </div>

    <!-- القائمة الجانبية -->
    <div id="menuOverlay" class="menu-overlay" onclick="closeSideMenu()"></div>
    <div id="sideMenu" class="side-menu">
      <div class="flex items-center justify-between mb-6">
        <h2
          id="menuTitle"
          class="text-xl font-bold text-gray-900 dark:text-white"
        >
          القائمة
        </h2>
        <button
          onclick="closeSideMenu()"
          class="p-2 rounded-lg hover:bg-gray-100 dark:hover:bg-gray-700 transition-colors"
        >
          <svg
            class="w-5 h-5 text-gray-600 dark:text-gray-300"
            fill="none"
            stroke="currentColor"
            viewBox="0 0 24 24"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M6 18L18 6M6 6l12 12"
            ></path>
          </svg>
        </button>
      </div>

      <!-- عناصر القائمة -->
      <div class="space-y-2">
        <div
          class="menu-item active"
          data-section="homeSection"
          onclick="navigateToSection('homeSection')"
        >
          <svg
            class="menu-item-icon"
            fill="none"
            stroke="currentColor"
            viewBox="0 0 24 24"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M3 12l2-2m0 0l7-7 7 7M5 10v10a1 1 0 001 1h3m10-11l2 2m-2-2v10a1 1 0 01-1 1h-3m-6 0a1 1 0 001-1v-4a1 1 0 011-1h2a1 1 0 011 1v4a1 1 0 001 1m-6 0h6"
            ></path>
          </svg>
          <span id="menuHome">الرئيسية</span>
        </div>

        <div
          class="menu-item"
          data-section="favoritesSection"
          onclick="navigateToSection('favoritesSection')"
        >
          <svg
            class="menu-item-icon"
            fill="none"
            stroke="currentColor"
            viewBox="0 0 24 24"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M4.318 6.318a4.5 4.5 0 000 6.364L12 20.364l7.682-7.682a4.5 4.5 0 00-6.364-6.364L12 7.636l-1.318-1.318a4.5 4.5 0 00-6.364 0z"
            ></path>
          </svg>
          <span id="menuFavorites">المفضلة</span>
        </div>

        <div
          class="menu-item"
          data-section="profileSection"
          onclick="navigateToSection('profileSection')"
        >
          <svg
            class="menu-item-icon"
            fill="none"
            stroke="currentColor"
            viewBox="0 0 24 24"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M19 11H5m14 0a2 2 0 012 2v6a2 2 0 01-2 2H5a2 2 0 01-2-2v-6a2 2 0 012-2m14 0V9a2 2 0 00-2-2M5 11V9a2 2 0 012-2m0 0V5a2 2 0 012-2h6a2 2 0 012 2v2M7 7h10"
            ></path>
          </svg>
          <span id="menuApps">التطبيقات</span>
        </div>

        <div
          class="menu-item"
          data-section="settingsSection"
          onclick="navigateToSection('settingsSection')"
        >
          <svg
            class="menu-item-icon"
            fill="none"
            stroke="currentColor"
            viewBox="0 0 24 24"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M10.325 4.317c.426-1.756 2.924-1.756 3.35 0a1.724 1.724 0 002.573 1.066c1.543-.94 3.31.826 2.37 2.37a1.724 1.724 0 001.065 2.572c1.756.426 1.756 2.924 0 3.35a1.724 1.724 0 00-1.066 2.573c.94 1.543-.826 3.31-2.37 2.37a1.724 1.724 0 00-2.572 1.065c-.426 1.756-2.924 1.756-3.35 0a1.724 1.724 0 00-2.573-1.066c-1.543.94-3.31-.826-2.37-2.37a1.724 1.724 0 00-1.065-2.572c-1.756-.426-1.756-2.924 0-3.35a1.724 1.724 0 001.066-2.573c-.94-1.543.826-3.31 2.37-2.37.996.608 2.296.07 2.572-1.065z"
            ></path>
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M15 12a3 3 0 11-6 0 3 3 0 016 0z"
            ></path>
          </svg>
          <span id="menuSettings">الإعدادات</span>
        </div>
      </div>

      <!-- تصنيفات سريعة -->
      <div class="mt-8">
        <h3
          id="quickCategoriesTitle"
          class="text-sm font-semibold text-gray-600 dark:text-gray-400 mb-4 uppercase tracking-wider"
        >
          تصنيفات سريعة
        </h3>
        <div class="space-y-2">
          <div class="menu-item" onclick="quickFilterCategory('productivity')">
            <span class="menu-item-icon text-lg">🏢</span>
            <span id="categoryProductivity">إنتاجية</span>
          </div>
          <div class="menu-item" onclick="quickFilterCategory('entertainment')">
            <span class="menu-item-icon text-lg">🎮</span>
            <span id="categoryEntertainment">ترفيه</span>
          </div>
          <div class="menu-item" onclick="quickFilterCategory('tools')">
            <span class="menu-item-icon text-lg">🔧</span>
            <span id="categoryTools">أدوات</span>
          </div>
          <div class="menu-item" onclick="quickFilterCategory('communication')">
            <span class="menu-item-icon text-lg">💬</span>
            <span id="categoryCommunication">تواصل</span>
          </div>
          <div class="menu-item" onclick="quickFilterCategory('media')">
            <span class="menu-item-icon text-lg">📱</span>
            <span id="categoryMedia">وسائط</span>
          </div>
        </div>
      </div>
    </div>

    <div class="main-content">
      <!-- صفحة الرئيسية -->
      <div id="homeSection" class="content-section active p-6">
        <div class="max-w-6xl mx-auto">
          <!-- العنوان الرئيسي -->
          <div class="text-center mb-3">
            <div class="flex flex-col items-center">
              <h1
                id="homeTitle"
                class="text-3xl font-bold mb-1 bg-gradient-to-r from-[#0098DA] to-[#28C7ED] text-transparent bg-clip-text"
              >
                مرحباً بك في FLUXY
              </h1>

              <p id="homeSubtitle" class="text-gray-600 dark:text-gray-400">
                اكتشف واستمتع بتطبيقاتك المفضلة
              </p>
            </div>
          </div>

          <!-- شريط البحث -->
          <div class="max-w-md mx-auto mb-4">
            <div class="relative">
              <input
                type="text"
                id="homeSearchInput"
                placeholder="ابحث عن تطبيق..."
                class="w-full px-4 py-3 pr-12 text-base rounded-xl border border-gray-300 dark:border-gray-600 bg-white dark:bg-gray-800 text-gray-900 dark:text-white placeholder-gray-500 dark:placeholder-gray-400 focus:ring-2 focus:ring-primary focus:border-transparent transition-all"
              />
              <div class="absolute inset-y-0 right-0 pr-3 flex items-center">
                <svg
                  class="h-5 w-5 text-gray-400"
                  fill="none"
                  stroke="currentColor"
                  viewBox="0 0 24 24"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z"
                  ></path>
                </svg>
              </div>
            </div>
          </div>

          <!-- أقسام التطبيقات المميزة (Carousel Sections) -->
          <div id="featuredSections" class="space-y-8 mb-8">
            <!-- قسم الأكثر استعمالاً -->
            <div class="section-carousel">
              <div class="flex items-center justify-between mb-4">
                <h2
                  id="mostUsedTitle"
                  class="text-xl font-bold text-gray-900 dark:text-white"
                >
                  الأكثر استعمالاً
                </h2>
                <button
                  id="mostUsedViewAll"
                  class="text-primary hover:text-blue-600 text-sm font-medium transition-colors"
                  onclick="showAllInCategory('most-used')"
                >
                  عرض الكل →
                </button>
              </div>
              <div class="relative">
                <div
                  id="mostUsedCarousel"
                  class="overflow-x-auto scrollbar-hide scroll-smooth"
                >
                  <div class="flex gap-4 pb-2" style="width: max-content">
                    <!-- سيتم ملء التطبيقات هنا -->
                  </div>
                </div>
                <!-- أزرار التنقل -->
                <button
                  class="carousel-btn carousel-btn-left absolute left-0 top-1/2 transform -translate-y-1/2 -translate-x-2 bg-white dark:bg-gray-800 shadow-lg rounded-full p-2 hover:shadow-xl transition-all z-10"
                  onclick="scrollCarousel('mostUsedCarousel', -200)"
                >
                  <svg
                    class="w-5 h-5 text-gray-600 dark:text-gray-300"
                    fill="none"
                    stroke="currentColor"
                    viewBox="0 0 24 24"
                  >
                    <path
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      stroke-width="2"
                      d="M15 19l-7-7 7-7"
                    ></path>
                  </svg>
                </button>
                <button
                  class="carousel-btn carousel-btn-right absolute right-0 top-1/2 transform -translate-y-1/2 translate-x-2 bg-white dark:bg-gray-800 shadow-lg rounded-full p-2 hover:shadow-xl transition-all z-10"
                  onclick="scrollCarousel('mostUsedCarousel', 200)"
                >
                  <svg
                    class="w-5 h-5 text-gray-600 dark:text-gray-300"
                    fill="none"
                    stroke="currentColor"
                    viewBox="0 0 24 24"
                  >
                    <path
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      stroke-width="2"
                      d="M9 5l7 7-7 7"
                    ></path>
                  </svg>
                </button>
              </div>
            </div>

            <!-- قسم الأعلى تقييماً -->
            <div class="section-carousel">
              <div class="flex items-center justify-between mb-4">
                <h2
                  id="topRatedTitle"
                  class="text-xl font-bold text-gray-900 dark:text-white"
                >
                  الأعلى تقييماً
                </h2>
                <button
                  id="topRatedViewAll"
                  class="text-primary hover:text-blue-600 text-sm font-medium transition-colors"
                  onclick="showAllInCategory('top-rated')"
                >
                  عرض الكل →
                </button>
              </div>
              <div class="relative">
                <div
                  id="topRatedCarousel"
                  class="overflow-x-auto scrollbar-hide scroll-smooth"
                >
                  <div class="flex gap-4 pb-2" style="width: max-content">
                    <!-- سيتم ملء التطبيقات هنا -->
                  </div>
                </div>
                <!-- أزرار التنقل -->
                <button
                  class="carousel-btn carousel-btn-left absolute left-0 top-1/2 transform -translate-y-1/2 -translate-x-2 bg-white dark:bg-gray-800 shadow-lg rounded-full p-2 hover:shadow-xl transition-all z-10"
                  onclick="scrollCarousel('topRatedCarousel', -200)"
                >
                  <svg
                    class="w-5 h-5 text-gray-600 dark:text-gray-300"
                    fill="none"
                    stroke="currentColor"
                    viewBox="0 0 24 24"
                  >
                    <path
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      stroke-width="2"
                      d="M15 19l-7-7 7-7"
                    ></path>
                  </svg>
                </button>
                <button
                  class="carousel-btn carousel-btn-right absolute right-0 top-1/2 transform -translate-y-1/2 translate-x-2 bg-white dark:bg-gray-800 shadow-lg rounded-full p-2 hover:shadow-xl transition-all z-10"
                  onclick="scrollCarousel('topRatedCarousel', 200)"
                >
                  <svg
                    class="w-5 h-5 text-gray-600 dark:text-gray-300"
                    fill="none"
                    stroke="currentColor"
                    viewBox="0 0 24 24"
                  >
                    <path
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      stroke-width="2"
                      d="M9 5l7 7-7 7"
                    ></path>
                  </svg>
                </button>
              </div>
            </div>

            <!-- قسم الأحدث -->
            <div class="section-carousel">
              <div class="flex items-center justify-between mb-4">
                <h2
                  id="newestTitle"
                  class="text-xl font-bold text-gray-900 dark:text-white"
                >
                  الأحدث
                </h2>
                <button
                  id="newestViewAll"
                  class="text-primary hover:text-blue-600 text-sm font-medium transition-colors"
                  onclick="showAllInCategory('newest')"
                >
                  عرض الكل →
                </button>
              </div>
              <div class="relative">
                <div
                  id="newestCarousel"
                  class="overflow-x-auto scrollbar-hide scroll-smooth"
                >
                  <div class="flex gap-4 pb-2" style="width: max-content">
                    <!-- سيتم ملء التطبيقات هنا -->
                  </div>
                </div>
                <!-- أزرار التنقل -->
                <button
                  class="carousel-btn carousel-btn-left absolute left-0 top-1/2 transform -translate-y-1/2 -translate-x-2 bg-white dark:bg-gray-800 shadow-lg rounded-full p-2 hover:shadow-xl transition-all z-10"
                  onclick="scrollCarousel('newestCarousel', -200)"
                >
                  <svg
                    class="w-5 h-5 text-gray-600 dark:text-gray-300"
                    fill="none"
                    stroke="currentColor"
                    viewBox="0 0 24 24"
                  >
                    <path
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      stroke-width="2"
                      d="M15 19l-7-7 7-7"
                    ></path>
                  </svg>
                </button>
                <button
                  class="carousel-btn carousel-btn-right absolute right-0 top-1/2 transform -translate-y-1/2 translate-x-2 bg-white dark:bg-gray-800 shadow-lg rounded-full p-2 hover:shadow-xl transition-all z-10"
                  onclick="scrollCarousel('newestCarousel', 200)"
                >
                  <svg
                    class="w-5 h-5 text-gray-600 dark:text-gray-300"
                    fill="none"
                    stroke="currentColor"
                    viewBox="0 0 24 24"
                  >
                    <path
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      stroke-width="2"
                      d="M9 5l7 7-7 7"
                    ></path>
                  </svg>
                </button>
              </div>
            </div>

            <!-- قسم الألعاب المميزة -->
            <div class="section-carousel">
              <div class="flex items-center justify-between mb-4">
                <h2
                  id="featuredGamesTitle"
                  class="text-xl font-bold text-gray-900 dark:text-white"
                >
                  الألعاب المميزة
                </h2>
                <button
                  id="featuredGamesViewAll"
                  class="text-primary hover:text-blue-600 text-sm font-medium transition-colors"
                  onclick="showAllInCategory('featured-games')"
                >
                  عرض الكل →
                </button>
              </div>
              <div class="relative">
                <div
                  id="featuredGamesCarousel"
                  class="overflow-x-auto scrollbar-hide scroll-smooth"
                >
                  <div class="flex gap-4 pb-2" style="width: max-content">
                    <!-- سيتم ملء التطبيقات هنا -->
                  </div>
                </div>
                <!-- أزرار التنقل -->
                <button
                  class="carousel-btn carousel-btn-left absolute left-0 top-1/2 transform -translate-y-1/2 -translate-x-2 bg-white dark:bg-gray-800 shadow-lg rounded-full p-2 hover:shadow-xl transition-all z-10"
                  onclick="scrollCarousel('featuredGamesCarousel', -200)"
                >
                  <svg
                    class="w-5 h-5 text-gray-600 dark:text-gray-300"
                    fill="none"
                    stroke="currentColor"
                    viewBox="0 0 24 24"
                  >
                    <path
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      stroke-width="2"
                      d="M15 19l-7-7 7-7"
                    ></path>
                  </svg>
                </button>
                <button
                  class="carousel-btn carousel-btn-right absolute right-0 top-1/2 transform -translate-y-1/2 translate-x-2 bg-white dark:bg-gray-800 shadow-lg rounded-full p-2 hover:shadow-xl transition-all z-10"
                  onclick="scrollCarousel('featuredGamesCarousel', 200)"
                >
                  <svg
                    class="w-5 h-5 text-gray-600 dark:text-gray-300"
                    fill="none"
                    stroke="currentColor"
                    viewBox="0 0 24 24"
                  >
                    <path
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      stroke-width="2"
                      d="M9 5l7 7-7 7"
                    ></path>
                  </svg>
                </button>
              </div>
            </div>
          </div>

          <!-- زر عرض جميع التطبيقات -->
          <div class="text-center mt-8">
            <button
              onclick="navigateToSection('profileSection')"
              class="bg-primary hover:bg-blue-600 text-white px-8 py-3 rounded-xl font-medium transition-colors flex items-center justify-center mx-auto space-x-2 space-x-reverse"
            >
              <svg
                class="w-5 h-5"
                fill="none"
                stroke="currentColor"
                viewBox="0 0 24 24"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M19 11H5m14 0a2 2 0 012 2v6a2 2 0 01-2 2H5a2 2 0 01-2-2v-6a2 2 0 012-2m14 0V9a2 2 0 00-2-2M5 11V9a2 2 0 012-2m0 0V5a2 2 0 012-2h6a2 2 0 012 2v2M7 7h10"
                ></path>
              </svg>
              <span id="browseAllAppsBtn">تصفح جميع التطبيقات</span>
            </button>
            <p
              id="discoverMoreText"
              class="text-gray-500 dark:text-gray-400 text-sm mt-2"
            >
              اكتشف أكثر من 1000+ تطبيق مختلف
            </p>
          </div>
        </div>
      </div>

      <!-- صفحة المفضلة المحسنة -->
      <div id="favoritesSection" class="content-section p-6">
        <div class="max-w-4xl mx-auto">
          <h1
            id="favoritesTitle"
            class="text-3xl font-bold text-center mb-8 bg-gradient-to-r from-[#0098DA] to-[#28C7ED] text-transparent bg-clip-text"
          >
            التطبيقات المفضلة
          </h1>

          <div id="favoritesGrid" class="grid grid-cols-2 md:grid-cols-3 gap-6">
            <!-- سيتم إضافة التطبيقات المفضلة هنا -->
          </div>

          <div id="emptyFavorites" class="favorites-empty-container">
            <div class="favorites-empty-heart">
              <svg viewBox="0 0 24 24" fill="currentColor">
                <path
                  d="M12 21.35l-1.45-1.32C5.4 15.36 2 12.28 2 8.5 
                                       2 5.42 4.42 3 7.5 3c1.74 0 3.41.81 
                                       4.5 2.09C13.09 3.81 14.76 3 16.5 3 
                                       19.58 3 22 5.42 22 8.5c0 3.78-3.4 
                                       6.86-8.55 11.54L12 21.35z"
                ></path>
              </svg>
            </div>

            <h3 id="emptyFavoritesTitle" class="favorites-empty-title">
              لا توجد تطبيقات مفضلة
            </h3>
            <p id="emptyFavoritesDesc" class="favorites-empty-desc">
              قم بإضافة تطبيقاتك المفضلة لتظهر هنا
            </p>

            <button
              id="addAppsBtn"
              onclick="navigateToAppsFromFavorites()"
              class="favorites-add-btn"
            >
              <svg fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M12 6v6m0 0v6m0-6h6m-6 0H6"
                ></path>
              </svg>
              <span>أضف التطبيقات</span>
            </button>

            <p id="addAppsDesc" class="favorites-add-desc">
              استكشف مجموعة التطبيقات المتنوعة وأضف المفضل منها
            </p>
          </div>
        </div>
      </div>

      <!-- صفحة الأقسام المميزة الجديدة -->
      <div id="categorySection" class="content-section p-6">
        <div class="max-w-6xl mx-auto">
          <!-- زر الرجوع -->
          <div class="mb-6">
            <button
              onclick="navigateToSection('homeSection')"
              class="back-btn flex items-center space-x-2 space-x-reverse text-primary hover:text-blue-600 font-medium transition-colors"
            >
              <svg
                class="w-5 h-5"
                fill="none"
                stroke="currentColor"
                viewBox="0 0 24 24"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M15 19l-7-7 7-7"
                ></path>
              </svg>
              <span id="backToHomeBtn">العودة للرئيسية</span>
            </button>
          </div>

          <!-- العنوان الرئيسي -->
          <div class="text-center mb-6">
            <h1
              id="categoryTitle"
              class="text-3xl font-bold text-gray-900 dark:text-white mb-2"
            >
              الأكثر استعمالاً
            </h1>
            <p id="categorySubtitle" class="text-gray-600 dark:text-gray-400">
              اكتشف التطبيقات الأكثر استعمالاً
            </p>
          </div>

          <!-- شريط البحث المخصص للقسم -->
          <div class="max-w-lg mx-auto mb-6">
            <div class="relative">
              <input
                type="text"
                id="categorySearchInput"
                placeholder="ابحث في هذا القسم..."
                class="w-full px-4 py-3 pr-12 text-base rounded-xl border border-gray-300 dark:border-gray-600 bg-white dark:bg-gray-800 text-gray-900 dark:text-white placeholder-gray-500 dark:placeholder-gray-400 focus:ring-2 focus:ring-primary focus:border-transparent transition-all"
              />
              <div class="absolute inset-y-0 right-0 pr-3 flex items-center">
                <svg
                  class="h-5 w-5 text-gray-400"
                  fill="none"
                  stroke="currentColor"
                  viewBox="0 0 24 24"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z"
                  ></path>
                </svg>
              </div>
              <!-- مؤشر البحث -->
              <div
                id="categorySearchIndicator"
                class="absolute left-3 top-1/2 transform -translate-y-1/2 hidden"
              >
                <div
                  class="loading-indicator w-5 h-5 border-2 border-primary border-t-transparent rounded-full animate-spin"
                ></div>
              </div>
            </div>
          </div>

          <!-- مؤشر التحميل -->
          <div id="categoryLoadingIndicator" class="hidden text-center py-8">
            <div
              class="loading-indicator inline-block w-8 h-8 border-4 border-primary border-t-transparent rounded-full animate-spin mb-4"
            ></div>
            <p
              id="categoryLoadingText"
              class="text-gray-600 dark:text-gray-400"
            >
              جاري تحميل التطبيقات...
            </p>
          </div>

          <!-- رسالة عدم وجود نتائج -->
          <div id="categoryNoResultsMessage" class="hidden text-center py-12">
            <svg
              class="mx-auto h-12 w-12 text-gray-400 mb-4"
              fill="none"
              stroke="currentColor"
              viewBox="0 0 24 24"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z"
              ></path>
            </svg>
            <h3
              id="categoryNoResultsTitle"
              class="text-lg font-medium text-gray-900 dark:text-white mb-2"
            >
              لا توجد نتائج
            </h3>
            <p
              id="categoryNoResultsDesc"
              class="text-gray-500 dark:text-gray-400"
            >
              لم نجد أي تطبيق يطابق بحثك في هذا القسم
            </p>
          </div>

          <!-- شبكة التطبيقات المحسنة -->
          <div class="apps-grid-enhanced mb-8" id="categoryAppsGrid">
            <!-- سيتم إضافة التطبيقات هنا بواسطة JavaScript -->
          </div>

          <!-- نظام الصفحات المخصص للقسم -->
          <div id="categoryPaginationContainer" class="pagination-enhanced">
            <!-- معلومات الصفحة -->
            <div class="text-center mb-4">
              <div
                class="flex items-center justify-center space-x-4 space-x-reverse text-sm text-gray-600 dark:text-gray-400"
              >
                <span id="categoryPageInfo">صفحة 1 من 1</span>
                <span class="text-gray-400">•</span>
                <span id="categoryTotalAppsInfo">0 تطبيق</span>
              </div>
            </div>

            <!-- أزرار التنقل الرئيسية -->
            <div
              class="flex items-center justify-center space-x-2 space-x-reverse mb-4"
            >
              <!-- الانتقال للصفحة الأولى -->
              <button
                id="categoryFirstPageBtn"
                class="page-btn px-3 py-2 text-gray-500 dark:text-gray-400 hover:text-primary disabled:opacity-50 disabled:cursor-not-allowed rounded-lg border border-gray-300 dark:border-gray-600 hover:border-primary transition-all"
              >
                <svg
                  class="w-4 h-4"
                  fill="none"
                  stroke="currentColor"
                  viewBox="0 0 24 24"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M11 19l-7-7 7-7m8 14l-7-7 7-7"
                  ></path>
                </svg>
              </button>

              <!-- الصفحة السابقة -->
              <button
                id="categoryPrevBtn"
                class="page-btn px-4 py-2 text-gray-500 dark:text-gray-400 hover:text-primary disabled:opacity-50 disabled:cursor-not-allowed rounded-lg border border-gray-300 dark:border-gray-600 hover:border-primary transition-all"
              >
                <svg
                  class="w-4 h-4"
                  fill="none"
                  stroke="currentColor"
                  viewBox="0 0 24 24"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M15 19l-7-7 7-7"
                  ></path>
                </svg>
              </button>

              <!-- أرقام الصفحات -->
              <div
                id="categoryPageNumbers"
                class="flex space-x-1 space-x-reverse"
              >
                <!-- سيتم إضافة أرقام الصفحات هنا -->
              </div>

              <!-- الصفحة التالية -->
              <button
                id="categoryNextBtn"
                class="page-btn px-4 py-2 text-gray-500 dark:text-gray-400 hover:text-primary disabled:opacity-50 disabled:cursor-not-allowed rounded-lg border border-gray-300 dark:border-gray-600 hover:border-primary transition-all"
              >
                <svg
                  class="w-4 h-4"
                  fill="none"
                  stroke="currentColor"
                  viewBox="0 0 24 24"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M9 5l7 7-7 7"
                  ></path>
                </svg>
              </button>

              <!-- الانتقال للصفحة الأخيرة -->
              <button
                id="categoryLastPageBtn"
                class="page-btn px-3 py-2 text-gray-500 dark:text-gray-400 hover:text-primary disabled:opacity-50 disabled:cursor-not-allowed rounded-lg border border-gray-300 dark:border-gray-600 hover:border-primary transition-all"
              >
                <svg
                  class="w-4 h-4"
                  fill="none"
                  stroke="currentColor"
                  viewBox="0 0 24 24"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M13 5l7 7-7 7M5 5l7 7-7 7"
                  ></path>
                </svg>
              </button>
            </div>

            <!-- الانتقال السريع لصفحة معينة -->
            <div
              class="flex items-center justify-center space-x-3 space-x-reverse"
            >
              <span
                id="categoryGoToPageLabel"
                class="text-sm text-gray-600 dark:text-gray-400"
                >الانتقال للصفحة:</span
              >
              <input
                type="number"
                id="categoryPageJumpInput"
                min="1"
                max="1"
                class="w-20 px-3 py-2 text-sm border border-gray-300 dark:border-gray-600 rounded-lg bg-white dark:bg-gray-800 text-gray-900 dark:text-white text-center focus:ring-2 focus:ring-primary focus:border-transparent transition-all"
                placeholder="1"
              />
              <button
                id="categoryGoToPageBtn"
                class="px-4 py-2 text-sm bg-primary text-white rounded-lg hover:bg-blue-600 transition-colors font-medium"
              >
                انتقال
              </button>
            </div>
          </div>
        </div>
      </div>

      <!-- صفحة التطبيقات المحدثة -->
      <div id="profileSection" class="content-section p-6">
        <div class="max-w-6xl mx-auto">
          <!-- العنوان الرئيسي -->
          <div class="text-center mb-6">
            <h1
              id="profileTitle"
              class="text-3xl font-bold mb-2 bg-gradient-to-r from-[#0098DA] to-[#28C7ED] text-transparent bg-clip-text"
            >
              مكتبة التطبيقات
            </h1>

            <p id="profileSubtitle" class="text-gray-600 dark:text-gray-400">
              تصفح واكتشف جميع التطبيقات المتاحة
            </p>
          </div>

          <!-- شريط البحث المحسن -->
          <div class="max-w-lg mx-auto mb-6">
            <div class="relative">
              <input
                type="text"
                id="searchInput"
                placeholder="ابحث عن تطبيق..."
                class="w-full px-4 py-3 pr-12 text-base rounded-xl border border-gray-300 dark:border-gray-600 bg-white dark:bg-gray-800 text-gray-900 dark:text-white placeholder-gray-500 dark:placeholder-gray-400 focus:ring-2 focus:ring-primary focus:border-transparent transition-all"
              />
              <div class="absolute inset-y-0 right-0 pr-3 flex items-center">
                <svg
                  class="h-5 w-5 text-gray-400"
                  fill="none"
                  stroke="currentColor"
                  viewBox="0 0 24 24"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z"
                  ></path>
                </svg>
              </div>
              <!-- مؤشر البحث -->
              <div
                id="searchIndicator"
                class="absolute left-3 top-1/2 transform -translate-y-1/2 hidden"
              >
                <div
                  class="loading-indicator w-5 h-5 border-2 border-primary border-t-transparent rounded-full animate-spin"
                ></div>
              </div>
            </div>
          </div>

          <!-- شريط التصنيفات -->
<div class="-mx-6 -my-2 mb-6">
  <div
    id="categoryCarousel"
    class="overflow-x-auto scrollbar-hide scroll-smooth py-4"
  >
    <div
      class="flex gap-3 px-6"
      id="categoryFilter"
      style="width: max-content"
    >

      <!-- جميع التطبيقات -->
      <button
        class="category-btn active px-4 py-1.5 rounded-full text-xs font-medium whitespace-nowrap flex-shrink-0 flex items-center"
        data-category="all"
      >
        <div class="w-7 h-7 rounded-full flex items-center justify-center ml-1.5">
          <svg
            class="w-3.5 h-3.5 text-blue-600 dark:text-blue-400"
            fill="none"
            stroke="currentColor"
            viewBox="0 0 24 24"
          >
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
              d="M19 11H5m14 0a2 2 0 012 2v6a2 2 0 01-2 2H5a2 2 0 01-2-2v-6a2 2 0 012-2m14 0V9a2 2 0 00-2-2M5 11V9a2 2 0 012-2m0 0V5a2 2 0 012-2h6a2 2 0 012 2v2M7 7h10" />
          </svg>
        </div>
        <span id="allAppsBtn" class="btn-text">جميع التطبيقات</span>
      </button>

      <!-- إنتاجية -->
      <button
        class="category-btn px-4 py-1.5 rounded-full text-xs font-medium whitespace-nowrap flex-shrink-0 flex items-center"
        data-category="productivity"
      >
        <div class="w-7 h-7 rounded-full bg-green-50 dark:bg-green-900/20 flex items-center justify-center ml-1.5">
          <svg
            class="w-3.5 h-3.5 text-green-600 dark:text-green-400"
            fill="none"
            stroke="currentColor"
            viewBox="0 0 24 24"
          >
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
              d="M9 12h6m-6 4h6m2 5H7a2 2 0 01-2-2V5a2 2 0 012-2h5.586a1 1 0 01.707.293l5.414 5.414a1 1 0 01.293.707V19a2 2 0 01-2 2z" />
          </svg>
        </div>
        <span id="productivityBtn" class="btn-text">إنتاجية</span>
      </button>

      <!-- ترفيه -->
      <button
        class="category-btn px-4 py-1.5 rounded-full text-xs font-medium whitespace-nowrap flex-shrink-0 flex items-center"
        data-category="entertainment"
      >
        <div class="w-7 h-7 rounded-full bg-purple-50 dark:bg-purple-900/20 flex items-center justify-center ml-1.5">
          <svg
            class="w-3.5 h-3.5 text-purple-600 dark:text-purple-400"
            fill="none"
            stroke="currentColor"
            viewBox="0 0 24 24"
          >
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
              d="M11 4a2 2 0 114 0v1a1 1 0 001 1h3a1 1 0 011 1v3a1 1 0 01-1 1h-1a2 2 0 100 4h1a1 1 0 011 1v3a1 1 0 01-1 1h-3a1 1 0 01-1-1v-1a2 2 0 10-4 0v1a1 1 0 01-1 1H7a1 1 0 01-1-1v-3a1 1 0 011-1h1a2 2 0 100-4H7a1 1 0 01-1-1V7a1 1 0 011-1h3a1 1 0 001-1V4z" />
          </svg>
        </div>
        <span id="entertainmentBtn" class="btn-text">ترفيه</span>
      </button>

      <!-- أدوات -->
      <button
        class="category-btn px-4 py-1.5 rounded-full text-xs font-medium whitespace-nowrap flex-shrink-0 flex items-center"
        data-category="tools"
      >
        <div class="w-7 h-7 rounded-full bg-orange-50 dark:bg-orange-900/20 flex items-center justify-center ml-1.5">
          <svg
            class="w-3.5 h-3.5 text-orange-600 dark:text-orange-400"
            fill="none"
            stroke="currentColor"
            viewBox="0 0 24 24"
          >
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
              d="M10.325 4.317c.426-1.756 2.924-1.756 3.35 0a1.724 1.724 0 002.573 1.066c1.543-.94 3.31.826 2.37 2.37a1.724 1.724 0 001.065 2.572c1.756.426 1.756 2.924 0 3.35a1.724 1.724 0 00-1.066 2.573c.94 1.543-.826 3.31-2.37 2.37a1.724 1.724 0 00-2.572 1.065c-.426 1.756-2.924 1.756-3.35 0a1.724 1.724 0 00-2.573-1.066c-1.543.94-3.31-.826-2.37-2.37a1.724 1.724 0 00-1.065-2.572c-1.756-.426-1.756-2.924 0-3.35a1.724 1.724 0 001.066-2.573c-.94-1.543.826-3.31 2.37-2.37.996.608 2.296.07 2.572-1.065z" />
          </svg>
        </div>
        <span id="toolsBtn" class="btn-text">أدوات</span>
      </button>

      <!-- تواصل -->
      <button
        class="category-btn px-4 py-1.5 rounded-full text-xs font-medium whitespace-nowrap flex-shrink-0 flex items-center"
        data-category="communication"
      >
        <div class="w-7 h-7 rounded-full bg-indigo-50 dark:bg-indigo-900/20 flex items-center justify-center ml-1.5">
          <svg
            class="w-3.5 h-3.5 text-indigo-600 dark:text-indigo-400"
            fill="none"
            stroke="currentColor"
            viewBox="0 0 24 24"
          >
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
              d="M8 12h.01M12 12h.01M16 12h.01M21 12c0 4.418-4.03 8-9 8a9.863 9.863 0 01-4.255-.949L3 20l1.395-3.72C3.512 15.042 3 13.574 3 12c0-4.418 4.03-8 9-8s9 3.582 9 8z" />
          </svg>
        </div>
        <span id="communicationBtn" class="btn-text">تواصل</span>
      </button>

      <!-- وسائط -->
      <button
        class="category-btn px-4 py-1.5 rounded-full text-xs font-medium whitespace-nowrap flex-shrink-0 flex items-center"
        data-category="media"
      >
        <div class="w-7 h-7 rounded-full bg-pink-50 dark:bg-pink-900/20 flex items-center justify-center ml-1.5">
          <svg
            class="w-3.5 h-3.5 text-pink-600 dark:text-pink-400"
            fill="none"
            stroke="currentColor"
            viewBox="0 0 24 24"
          >
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
              d="M15 10l4.553-2.276A1 1 0 0121 8.618v6.764a1 1 0 01-1.447.894L15 14M5 18h8a2 2 0 002-2V8a2 2 0 00-2-2H5a2 2 0 00-2 2v8a2 2 0 002 2z" />
          </svg>
        </div>
        <span id="mediaBtn" class="btn-text">وسائط</span>
      </button>

    </div>
  </div>
</div>

          <!-- مؤشر التحميل -->
          <div id="loadingIndicator" class="hidden text-center py-8">
            <div
              class="loading-indicator inline-block w-8 h-8 border-4 border-primary border-t-transparent rounded-full animate-spin mb-4"
            ></div>
            <p id="loadingText" class="text-gray-600 dark:text-gray-400">
              جاري تحميل التطبيقات...
            </p>
          </div>

          <!-- رسالة عدم وجود نتائج -->
          <div id="noResultsMessage" class="hidden text-center py-12">
            <svg
              class="mx-auto h-12 w-12 text-gray-400 mb-4"
              fill="none"
              stroke="currentColor"
              viewBox="0 0 24 24"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z"
              ></path>
            </svg>
            <h3
              id="noResultsTitle"
              class="text-lg font-medium text-gray-900 dark:text-white mb-2"
            >
              لا توجد نتائج
            </h3>
            <p id="noResultsDesc" class="text-gray-500 dark:text-gray-400">
              لم نجد أي تطبيق يطابق بحثك
            </p>
          </div>

          <!-- شبكة التطبيقات المحسنة -->
          <div class="apps-grid-enhanced mb-8" id="appsGrid">
            <!-- سيتم إضافة التطبيقات هنا بواسطة JavaScript -->
          </div>

          <!-- نظام الصفحات المحسن -->
          <div id="paginationContainer" class="pagination-enhanced">
            <!-- معلومات الصفحة -->
            <div class="text-center mb-4">
              <div
                class="flex items-center justify-center space-x-4 space-x-reverse text-sm text-gray-600 dark:text-gray-400"
              >
                <span id="pageInfo">صفحة 1 من 1</span>
                <span class="text-gray-400">•</span>
                <span id="totalAppsInfo">0 تطبيق</span>
              </div>
            </div>

            <!-- أزرار التنقل الرئيسية -->
            <div
              class="flex items-center justify-center space-x-2 space-x-reverse mb-4"
            >
              <!-- الانتقال للصفحة الأولى -->
              <button
                id="firstPageBtn"
                class="page-btn px-3 py-2 text-gray-500 dark:text-gray-400 hover:text-primary disabled:opacity-50 disabled:cursor-not-allowed rounded-lg border border-gray-300 dark:border-gray-600 hover:border-primary transition-all"
              >
                <svg
                  class="w-4 h-4"
                  fill="none"
                  stroke="currentColor"
                  viewBox="0 0 24 24"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M11 19l-7-7 7-7m8 14l-7-7 7-7"
                  ></path>
                </svg>
              </button>

              <!-- الصفحة السابقة -->
              <button
                id="prevBtn"
                class="page-btn px-4 py-2 text-gray-500 dark:text-gray-400 hover:text-primary disabled:opacity-50 disabled:cursor-not-allowed rounded-lg border border-gray-300 dark:border-gray-600 hover:border-primary transition-all"
              >
                <svg
                  class="w-4 h-4"
                  fill="none"
                  stroke="currentColor"
                  viewBox="0 0 24 24"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M15 19l-7-7 7-7"
                  ></path>
                </svg>
              </button>

              <!-- أرقام الصفحات -->
              <div id="pageNumbers" class="flex space-x-1 space-x-reverse">
                <!-- سيتم إضافة أرقام الصفحات هنا -->
              </div>

              <!-- الصفحة التالية -->
              <button
                id="nextBtn"
                class="page-btn px-4 py-2 text-gray-500 dark:text-gray-400 hover:text-primary disabled:opacity-50 disabled:cursor-not-allowed rounded-lg border border-gray-300 dark:border-gray-600 hover:border-primary transition-all"
              >
                <svg
                  class="w-4 h-4"
                  fill="none"
                  stroke="currentColor"
                  viewBox="0 0 24 24"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M9 5l7 7-7 7"
                  ></path>
                </svg>
              </button>

              <!-- الانتقال للصفحة الأخيرة -->
              <button
                id="lastPageBtn"
                class="page-btn px-3 py-2 text-gray-500 dark:text-gray-400 hover:text-primary disabled:opacity-50 disabled:cursor-not-allowed rounded-lg border border-gray-300 dark:border-gray-600 hover:border-primary transition-all"
              >
                <svg
                  class="w-4 h-4"
                  fill="none"
                  stroke="currentColor"
                  viewBox="0 0 24 24"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M13 5l7 7-7 7M5 5l7 7-7 7"
                  ></path>
                </svg>
              </button>
            </div>

            <!-- الانتقال السريع لصفحة معينة -->
            <div
              class="flex items-center justify-center space-x-3 space-x-reverse"
            >
              <span
                id="goToPageLabel"
                class="text-sm text-gray-600 dark:text-gray-400"
                >الانتقال للصفحة:</span
              >
              <input
                type="number"
                id="pageJumpInput"
                min="1"
                max="1"
                class="w-20 px-3 py-2 text-sm border border-gray-300 dark:border-gray-600 rounded-lg bg-white dark:bg-gray-800 text-gray-900 dark:text-white text-center focus:ring-2 focus:ring-primary focus:border-transparent transition-all"
                placeholder="1"
              />
              <button
                id="goToPageBtn"
                class="px-4 py-2 text-sm bg-primary text-white rounded-lg hover:bg-blue-600 transition-colors font-medium"
              >
                انتقال
              </button>
            </div>
          </div>
        </div>
      </div>

      <!-- صفحة الإعدادات المحدثة -->
      <div id="settingsSection" class="content-section p-6">
        <div class="max-w-2xl mx-auto">
          <h1
            id="settingsTitle"
            class="text-3xl font-bold text-center mb-10 bg-gradient-to-r from-[#0098DA] to-[#28C7ED] text-transparent bg-clip-text"
          >
            الإعدادات
          </h1>

          <!-- إعدادات التطبيق السريعة -->
          <div class="mb-8">
            <h3
              id="quickSettingsTitle"
              class="text-lg font-semibold text-gray-900 dark:text-white mb-6 px-4"
            >
              الإعدادات السريعة
            </h3>

            <div
              class="bg-white dark:bg-dark-card rounded-2xl border border-gray-200 dark:border-gray-700 overflow-hidden"
            >
              <div
                class="settings-item px-6 py-4 flex items-center justify-between border-b border-gray-100 dark:border-gray-600 last:border-b-0"
              >
                <div class="flex items-center space-x-4 space-x-reverse">
                  <div
                    class="w-10 h-10 rounded-full bg-blue-50 dark:bg-blue-900/20 flex items-center justify-center"
                  >
                    <svg
                      class="w-5 h-5 text-blue-600 dark:text-blue-400"
                      fill="none"
                      stroke="currentColor"
                      viewBox="0 0 24 24"
                    >
                      <path
                        stroke-linecap="round"
                        stroke-linejoin="round"
                        stroke-width="2"
                        d="M20.354 15.354A9 9 0 018.646 3.646 9.003 9.003 0 0012 21a9.003 9.003 0 008.354-5.646z"
                      ></path>
                    </svg>
                  </div>
                  <span
                    id="darkModeLabel"
                    class="text-gray-900 dark:text-white font-medium"
                    >الوضع المظلم</span
                  >
                </div>
                <div
                  id="darkModeToggle"
                  class="w-14 h-7 toggle-switch-modern active rounded-full relative cursor-pointer transition-all duration-300"
                  onclick="toggleDarkMode(event)"
                >
                  <div class="toggle-circle-modern left"></div>
                </div>
              </div>

              <div
                class="settings-item px-6 py-4 flex items-center justify-between border-b border-gray-100 dark:border-gray-600 last:border-b-0"
              >
                <div class="flex items-center space-x-4 space-x-reverse">
                  <div
                    class="w-10 h-10 rounded-full bg-purple-50 dark:bg-purple-900/20 flex items-center justify-center"
                  >
                    <svg
                      class="w-5 h-5 text-purple-600 dark:text-purple-400"
                      fill="none"
                      stroke="currentColor"
                      viewBox="0 0 24 24"
                    >
                      <path
                        stroke-linecap="round"
                        stroke-linejoin="round"
                        stroke-width="2"
                        d="M13 10V3L4 14h7v7l9-11h-7z"
                      ></path>
                    </svg>
                  </div>
                  <span
                    id="animationsLabel"
                    class="text-gray-900 dark:text-white font-medium"
                    >التأثيرات المتحركة</span
                  >
                </div>
                <div
                  id="animationsToggle"
                  class="w-14 h-7 toggle-switch-modern active rounded-full relative cursor-pointer transition-all duration-300"
                  onclick="toggleAnimations(event)"
                >
                  <div class="toggle-circle-modern left"></div>
                </div>
              </div>

              <div
                class="settings-item px-6 py-4 flex items-center justify-between border-b border-gray-100 dark:border-gray-600 last:border-b-0"
              >
                <div class="flex items-center space-x-4 space-x-reverse">
                  <div
                    class="w-10 h-10 rounded-full bg-green-50 dark:bg-green-900/20 flex items-center justify-center"
                  >
                    <svg
                      class="w-5 h-5 text-green-600 dark:text-green-400"
                      fill="none"
                      stroke="currentColor"
                      viewBox="0 0 24 24"
                    >
                      <path
                        stroke-linecap="round"
                        stroke-linejoin="round"
                        stroke-width="2"
                        d="M12 18h.01M8 21h8a2 2 0 002-2V5a2 2 0 00-2-2H8a2 2 0 00-2 2v14a2 2 0 002 2z"
                      ></path>
                    </svg>
                  </div>
                  <span
                    id="compactViewLabel"
                    class="text-gray-900 dark:text-white font-medium"
                    >العرض المضغوط</span
                  >
                </div>
                <div
                  id="compactViewToggle"
                  class="w-14 h-7 toggle-switch-modern inactive rounded-full relative cursor-pointer transition-all duration-300"
                  onclick="toggleCompactView(event)"
                >
                  <div class="toggle-circle-modern right"></div>
                </div>
              </div>
            </div>
          </div>

          <!-- إعدادات العامة -->
          <div class="mb-8">
            <h3
              id="generalSettingsTitle"
              class="text-lg font-semibold text-gray-900 dark:text-white mb-6 px-4"
            >
              الإعدادات العامة
            </h3>

            <div
              class="bg-white dark:bg-dark-card rounded-2xl border border-gray-200 dark:border-gray-700 overflow-hidden"
            >
              <div
                class="settings-item px-6 py-4 flex items-center justify-between cursor-pointer border-b border-gray-100 dark:border-gray-600 last:border-b-0 hover:bg-gray-50 dark:hover:bg-gray-700/30 transition-colors"
                onclick="openLanguageSettings()"
              >
                <div class="flex items-center space-x-4 space-x-reverse">
                  <div
                    class="w-10 h-10 rounded-full bg-orange-50 dark:bg-orange-900/20 flex items-center justify-center"
                  >
                    <svg
                      class="w-5 h-5 text-orange-600 dark:text-orange-400"
                      fill="none"
                      stroke="currentColor"
                      viewBox="0 0 24 24"
                    >
                      <path
                        stroke-linecap="round"
                        stroke-linejoin="round"
                        stroke-width="2"
                        d="M3 5h12M9 3v2m1.048 9.5A18.022 18.022 0 016.412 9m6.088 9h7M11 21l5-10 5 10M12.751 5C11.783 10.77 8.07 15.61 3 18.129"
                      ></path>
                    </svg>
                  </div>
                  <div>
                    <div
                      id="languageLabel"
                      class="text-gray-900 dark:text-white font-medium"
                    >
                      اللغة
                    </div>
                    <div
                      class="text-sm text-gray-500 dark:text-gray-400"
                      id="currentLanguage"
                    >
                      العربية
                    </div>
                  </div>
                </div>
                <svg
                  class="w-5 h-5 text-gray-400"
                  fill="none"
                  stroke="currentColor"
                  viewBox="0 0 24 24"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M9 5l7 7-7 7"
                  ></path>
                </svg>
              </div>

              <div
                class="settings-item px-6 py-4 flex items-center justify-between cursor-pointer border-b border-gray-100 dark:border-gray-600 last:border-b-0 hover:bg-gray-50 dark:hover:bg-gray-700/30 transition-colors"
                onclick="openThemeSettings()"
              >
                <div class="flex items-center space-x-4 space-x-reverse">
                  <div
                    class="w-10 h-10 rounded-full bg-pink-50 dark:bg-pink-900/20 flex items-center justify-center"
                  >
                    <svg
                      class="w-5 h-5 text-pink-600 dark:text-pink-400"
                      fill="none"
                      stroke="currentColor"
                      viewBox="0 0 24 24"
                    >
                      <path
                        stroke-linecap="round"
                        stroke-linejoin="round"
                        stroke-width="2"
                        d="M7 21a4 4 0 01-4-4V5a2 2 0 012-2h4a2 2 0 012 2v12a4 4 0 01-4 4zM21 5a2 2 0 00-2-2h-4a2 2 0 00-2 2v12a4 4 0 004 4 4 4 0 004-4V5z"
                      ></path>
                    </svg>
                  </div>
                  <div>
                    <div
                      id="themeLabel"
                      class="text-gray-900 dark:text-white font-medium"
                    >
                      المظهر
                    </div>
                    <div
                      class="text-sm text-gray-500 dark:text-gray-400"
                      id="currentTheme"
                    >
                      تلقائي
                    </div>
                  </div>
                </div>
                <svg
                  class="w-5 h-5 text-gray-400"
                  fill="none"
                  stroke="currentColor"
                  viewBox="0 0 24 24"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M9 5l7 7-7 7"
                  ></path>
                </svg>
              </div>

              <div
                class="settings-item px-6 py-4 flex items-center justify-between cursor-pointer border-b border-gray-100 dark:border-gray-600 last:border-b-0 hover:bg-gray-50 dark:hover:bg-gray-700/30 transition-colors"
                onclick="openDisplaySettings()"
              >
                <div class="flex items-center space-x-4 space-x-reverse">
                  <div
                    class="w-10 h-10 rounded-full bg-indigo-50 dark:bg-indigo-900/20 flex items-center justify-center"
                  >
                    <svg
                      class="w-5 h-5 text-indigo-600 dark:text-indigo-400"
                      fill="none"
                      stroke="currentColor"
                      viewBox="0 0 24 24"
                    >
                      <path
                        stroke-linecap="round"
                        stroke-linejoin="round"
                        stroke-width="2"
                        d="M9 17V7m0 10a2 2 0 01-2 2H5a2 2 0 01-2-2V7a2 2 0 012-2h2a2 2 0 012 2m0 10a2 2 0 002 2h2a2 2 0 002-2M9 7a2 2 0 012-2h2a2 2 0 012 2m0 0a2 2 0 012 2v6a2 2 0 01-2 2m-6 0a2 2 0 002 2 2 2 0 002-2m0 0V9a2 2 0 012-2 2 2 0 012 2v8a2 2 0 01-2 2 2 2 0 01-2-2z"
                      ></path>
                    </svg>
                  </div>
                  <div>
                    <div
                      id="displayLabel"
                      class="text-gray-900 dark:text-white font-medium"
                    >
                      عرض التطبيقات
                    </div>
                    <div
                      class="text-sm text-gray-500 dark:text-gray-400"
                      id="currentDisplay"
                    >
                      شبكة
                    </div>
                  </div>
                </div>
                <svg
                  class="w-5 h-5 text-gray-400"
                  fill="none"
                  stroke="currentColor"
                  viewBox="0 0 24 24"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M9 5l7 7-7 7"
                  ></path>
                </svg>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- شريط التنقل السفلي -->
    <div
      class="fixed bottom-0 left-0 right-0 bottom-nav bg-white dark:bg-dark-surface border-t border-gray-200 dark:border-gray-700 px-6 py-3"
    >
      <div class="flex justify-around items-center max-w-md mx-auto">
        <button
          class="nav-item active flex flex-col items-center space-y-1 px-3 py-2 text-gray-600 dark:text-gray-400"
          data-section="homeSection"
        >
          <svg
            class="w-6 h-6"
            fill="none"
            stroke="currentColor"
            viewBox="0 0 24 24"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M3 12l2-2m0 0l7-7 7 7M5 10v10a1 1 0 001 1h3m10-11l2 2m-2-2v10a1 1 0 01-1 1h-3m-6 0a1 1 0 001-1v-4a1 1 0 011-1h2a1 1 0 011 1v4a1 1 0 001 1m-6 0h6"
            ></path>
          </svg>
          <span id="navHome" class="text-xs">الرئيسية</span>
        </button>

        <button
          class="nav-item flex flex-col items-center space-y-1 px-3 py-2 text-gray-600 dark:text-gray-400"
          data-section="favoritesSection"
        >
          <svg
            class="w-6 h-6"
            fill="none"
            stroke="currentColor"
            viewBox="0 0 24 24"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M4.318 6.318a4.5 4.5 0 000 6.364L12 20.364l7.682-7.682a4.5 4.5 0 00-6.364-6.364L12 7.636l-1.318-1.318a4.5 4.5 0 00-6.364 0z"
            ></path>
          </svg>
          <span id="navFavorites" class="text-xs">المفضلة</span>
        </button>

        <button
          class="nav-item flex flex-col items-center space-y-1 px-3 py-2 text-gray-600 dark:text-gray-400"
          data-section="profileSection"
        >
          <svg
            class="w-6 h-6"
            fill="none"
            stroke="currentColor"
            viewBox="0 0 24 24"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M19 11H5m14 0a2 2 0 012 2v6a2 2 0 01-2 2H5a2 2 0 01-2-2v-6a2 2 0 012-2m14 0V9a2 2 0 00-2-2M5 11V9a2 2 0 012-2m0 0V5a2 2 0 012-2h6a2 2 0 012 2v2M7 7h10"
            ></path>
          </svg>
          <span id="navApps" class="text-xs">التطبيقات</span>
        </button>

        <button
          class="nav-item flex flex-col items-center space-y-1 px-3 py-2 text-gray-600 dark:text-gray-400"
          data-section="settingsSection"
        >
          <svg
            class="w-6 h-6"
            fill="none"
            stroke="currentColor"
            viewBox="0 0 24 24"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M10.325 4.317c.426-1.756 2.924-1.756 3.35 0a1.724 1.724 0 002.573 1.066c1.543-.94 3.31.826 2.37 2.37a1.724 1.724 0 001.065 2.572c1.756.426 1.756 2.924 0 3.35a1.724 1.724 0 00-1.066 2.573c.94 1.543-.826 3.31-2.37 2.37a1.724 1.724 0 00-2.572 1.065c-.426 1.756-2.924 1.756-3.35 0a1.724 1.724 0 00-2.573-1.066c-1.543.94-3.31-.826-2.37-2.37a1.724 1.724 0 00-1.065-2.572c-1.756-.426-1.756-2.924 0-3.35a1.724 1.724 0 001.066-2.573c-.94-1.543.826-3.31 2.37-2.37.996.608 2.296.07 2.572-1.065z"
            ></path>
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M15 12a3 3 0 11-6 0 3 3 0 016 0z"
            ></path>
          </svg>
          <span id="navSettings" class="text-xs">الإعدادات</span>
        </button>
      </div>
    </div>

    <!-- النافذة المنبثقة -->
    <div
      id="appModal"
      class="hidden fixed inset-0 z-50 modal-backdrop bg-black bg-opacity-50 flex items-center justify-center p-4"
    >
      <div
        class="modal-content bg-white dark:bg-dark-card rounded-2xl shadow-2xl max-w-md w-full mx-4 overflow-hidden"
      >
        <!-- رأس النافذة -->
        <div
          class="flex items-center justify-between p-6 border-b border-gray-200 dark:border-gray-700"
        >
          <h2
            id="modalTitle"
            class="text-xl font-bold text-gray-900 dark:text-white"
          >
            تفاصيل التطبيق
          </h2>
          <button
            id="closeModal"
            class="p-1 rounded-lg hover:bg-gray-100 dark:hover:bg-gray-700 transition-colors"
          >
            <svg
              class="h-6 w-6 text-gray-600 dark:text-gray-400"
              fill="none"
              stroke="currentColor"
              viewBox="0 0 24 24"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M6 18L18 6M6 6l12 12"
              ></path>
            </svg>
          </button>
        </div>

        <!-- محتوى النافذة -->
        <div class="p-6 max-h-96 overflow-y-auto pb-24">
          <div class="flex items-start space-x-4 space-x-reverse mb-4">
            <img
              id="modalImage"
              src=""
              alt=""
              class="w-16 h-16 rounded-xl object-cover"
            />
            <div class="flex-1">
              <h3
                id="modalAppName"
                class="text-lg font-semibold text-gray-900 dark:text-white mb-1"
              ></h3>
              <p id="modalCategory" class="text-sm text-primary mb-2"></p>
              <!-- تقييم بالنجوم -->
              <div class="flex items-center space-x-1 space-x-reverse">
                <div
                  id="modalRating"
                  class="flex items-center space-x-1 space-x-reverse"
                >
                  <!-- سيتم إضافة النجوم هنا -->
                </div>
                <span
                  id="modalRatingText"
                  class="text-xs text-gray-500 dark:text-gray-400 mr-2"
                ></span>
              </div>
            </div>
          </div>

          <p
            id="modalDescription"
            class="text-gray-600 dark:text-gray-300 text-sm leading-relaxed mb-6"
          ></p>

          <!-- إحصائيات سريعة -->
          <div class="grid grid-cols-2 gap-3 mb-6">
            <div class="bg-gray-50 dark:bg-gray-700 rounded-lg p-3 text-center">
              <div
                id="modalDownloads"
                class="text-lg font-semibold text-gray-900 dark:text-white"
              ></div>
              <div
                id="downloadsLabel"
                class="text-xs text-gray-500 dark:text-gray-400"
              >
                مستخدم
              </div>
            </div>
            <div class="bg-gray-50 dark:bg-gray-700 rounded-lg p-3 text-center">
              <div
                id="modalRatingDisplay"
                class="text-lg font-semibold text-gray-900 dark:text-white"
              ></div>
              <div
                id="ratingLabel"
                class="text-xs text-gray-500 dark:text-gray-400"
              >
                تقييم
              </div>
            </div>
          </div>

          <!-- معلومات التطبيق التفصيلية -->
          <div class="space-y-3">
            <div
              class="flex items-center justify-between py-2 border-b border-gray-100 dark:border-gray-700"
            >
              <span
                id="developerLabel"
                class="text-sm font-medium text-gray-700 dark:text-gray-300"
                >المطور</span
              >
              <span
                id="modalDeveloper"
                class="text-sm text-gray-600 dark:text-gray-400"
              ></span>
            </div>
            <div
              class="flex items-center justify-between py-2 border-b border-gray-100 dark:border-gray-700"
            >
              <span
                id="versionLabel"
                class="text-sm font-medium text-gray-700 dark:text-gray-300"
                >الإصدار</span
              >
              <span
                id="modalVersion"
                class="text-sm text-gray-600 dark:text-gray-400"
              ></span>
            </div>
            <div
              class="flex items-center justify-between py-2 border-b border-gray-100 dark:border-gray-700"
            >
              <span
                id="sizeLabel"
                class="text-sm font-medium text-gray-700 dark:text-gray-300"
                >الحجم</span
              >
              <span
                id="modalSize"
                class="text-sm text-gray-600 dark:text-gray-400"
              ></span>
            </div>
            <div
              class="flex items-center justify-between py-2 border-b border-gray-100 dark:border-gray-700"
            >
              <span
                id="lastUpdateLabel"
                class="text-sm font-medium text-gray-700 dark:text-gray-300"
                >آخر تحديث</span
              >
              <span
                id="modalLastUpdate"
                class="text-sm text-gray-600 dark:text-gray-400"
              ></span>
            </div>
            <div
              class="flex items-center justify-between py-2 border-b border-gray-100 dark:border-gray-700"
            >
              <span
                id="languageDetailLabel"
                class="text-sm font-medium text-gray-700 dark:text-gray-300"
                >اللغة</span
              >
              <span
                id="modalLanguage"
                class="text-sm text-gray-600 dark:text-gray-400"
              ></span>
            </div>
            <div
              class="flex items-center justify-between py-2 border-b border-gray-100 dark:border-gray-700"
            >
              <span
                id="requirementsLabel"
                class="text-sm font-medium text-gray-700 dark:text-gray-300"
                >متطلبات النظام</span
              >
              <span
                id="modalRequirements"
                class="text-sm text-gray-600 dark:text-gray-400"
              ></span>
            </div>
          </div>

          <!-- لقطات الشاشة -->
          <div class="mt-6">
            <h4
              id="screenshotsLabel"
              class="text-sm font-medium text-gray-700 dark:text-gray-300 mb-3"
            >
              لقطات الشاشة
            </h4>
            <div
              id="modalScreenshots"
              class="flex gap-2 overflow-x-auto scrollbar-hide"
            >
              <!-- سيتم إضافة لقطات الشاشة هنا -->
            </div>
          </div>
        </div>

        <!-- أزرار العمل الثابتة -->
        <div
          class="absolute bottom-0 left-0 right-0 p-6 pt-4 bg-white dark:bg-dark-card border-t border-gray-200 dark:border-gray-700 rounded-b-2xl"
        >
          <div class="flex space-x-3 space-x-reverse">
            <button
              id="openAppBtn"
              class="flex-1 bg-[#0098DA] text-white py-3 px-6 rounded-xl font-medium hover:bg-[#0284C7] transition-colors"
            >
              فتح التطبيق
            </button>
            <div class="flex space-x-2 space-x-reverse">
              <!-- زر المفضلة -->
              <button
                id="favoriteBtn"
                class="px-4 py-3 border border-gray-300 dark:border-gray-600 text-gray-700 dark:text-gray-300 rounded-xl hover:bg-gray-50 dark:hover:bg-gray-700 transition-colors flex items-center justify-center"
                title="إضافة إلى المفضلة"
              >
                <svg
                  class="w-5 h-5"
                  fill="none"
                  stroke="currentColor"
                  viewBox="0 0 24 24"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M4.318 6.318a4.5 4.5 0 000 6.364L12 20.364l7.682-7.682a4.5 4.5 0 00-6.364-6.364L12 7.636l-1.318-1.318a4.5 4.5 0 00-6.364 0z"
                  ></path>
                </svg>
              </button>
            
              <!-- زر المشاركة -->
              <button
                id="shareBtn"
                class="px-4 py-3 border border-gray-300 dark:border-gray-600 text-gray-700 dark:text-gray-300 rounded-xl hover:bg-gray-50 dark:hover:bg-gray-700 transition-colors flex items-center justify-center"
                title="مشاركة التطبيق"
              >
                <svg
                  class="w-5 h-5"
                  fill="none"
                  stroke="currentColor"
                  viewBox="0 0 24 24"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M18 2a3 3 0 100 6 3 3 0 000-6zM6 9a3 3 0 100 6 3 3 0 000-6zM18 16a3 3 0 100 6 3 3 0 000-6zM8.59 11.51L15.4 7.3M8.59 12.49L15.4 16.7"
                  ></path>
                </svg>
              </button>
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- نوافذ منبثقة للإعدادات -->
    <div
      id="settingsModal"
      class="hidden fixed inset-0 z-50 modal-backdrop bg-black bg-opacity-50 flex items-center justify-center p-4"
    >
      <div
        class="modal-content bg-white dark:bg-dark-card rounded-2xl shadow-2xl max-w-md w-full mx-4"
      >
        <div
          class="flex items-center justify-between p-6 border-b border-gray-200 dark:border-gray-700"
        >
          <h2
            id="settingsModalTitle"
            class="text-xl font-bold text-gray-900 dark:text-white"
          ></h2>
          <button
            onclick="closeSettingsModal()"
            class="p-1 rounded-lg hover:bg-gray-100 dark:hover:bg-gray-700 transition-colors"
          >
            <svg
              class="h-6 w-6 text-gray-600 dark:text-gray-400"
              fill="none"
              stroke="currentColor"
              viewBox="0 0 24 24"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M6 18L18 6M6 6l12 12"
              ></path>
            </svg>
          </button>
        </div>
        <div id="settingsModalContent" class="p-6">
          <!-- المحتوى يتم إدراجه ديناميكيًا -->
        </div>
      </div>
    </div>
<!-- Share Bottom Sheet -->
<div id="shareSheet" style="
  position: fixed;
  inset: 0;
  background: rgba(0,0,0,.5);
  display: none;
  z-index: 9999;
">

  <div id="shareContent" style="
    position: absolute;
    bottom: 0;
    left: 0;
    right: 0;
    background: #fff;
    border-radius: 16px 16px 0 0;
    padding: 20px;
    transform: translateY(100%);
    transition: transform .3s ease;
  ">

    <div style="
      width: 40px;
      height: 4px;
      background: #ccc;
      border-radius: 2px;
      margin: 0 auto 15px;
    "></div>

    <h3 style="text-align:center;margin-bottom:20px">
      مشاركة التطبيق
    </h3>

    <div style="display:flex;justify-content:space-around">
      <a id="wa" target="_blank">واتساب</a>
      <a id="fb" target="_blank">فيسبوك</a>
      <a id="tg" target="_blank">تيليجرام</a>
      <a id="tw" target="_blank">تويتر</a>
    </div>

    <button
      onclick="closeShare()"
      style="width:100%;margin-top:20px"
    >
      إغلاق
    </button>

  </div>
</div>
    <script>
      // إعداد الوضع المظلم المحسن
      let isDarkMode =
        window.matchMedia &&
        window.matchMedia("(prefers-color-scheme: dark)").matches;
      // دالة حفظ حالة الوضع المظلم
      function saveDarkMode() {
        localStorage.setItem("darkMode", isDarkMode);
      }

      // دالة تحميل حالة الوضع المظلم
      function loadDarkMode() {
        const saved = localStorage.getItem("darkMode");
        if (saved !== null) {
          isDarkMode = saved === "true";
        }
      }

      // تطبيق الوضع المظلم عند التحميل
      function initializeDarkMode() {
        if (isDarkMode) {
          document.documentElement.classList.add("dark");
          updateDarkModeIcons();
        } else {
          document.documentElement.classList.remove("dark");
          updateDarkModeIcons();
        }
      }

      // تحديث أيقونات الوضع المظلم
      function updateDarkModeIcons() {
        const darkIcon = document.getElementById("darkModeIcon");
        const lightIcon = document.getElementById("lightModeIcon");

        if (isDarkMode) {
          darkIcon.classList.add("hidden");
          lightIcon.classList.remove("hidden");
        } else {
          darkIcon.classList.remove("hidden");
          lightIcon.classList.add("hidden");
        }
      }

      // دالة التبديل السريع للوضع المظلم
      function toggleQuickDarkMode() {
        isDarkMode = !isDarkMode;
        saveDarkMode(); // ← أضف هذا السطر فقط
        if (isDarkMode) {
          document.documentElement.classList.add("dark");
        } else {
          document.documentElement.classList.remove("dark");
        }

        updateDarkModeIcons();
        updateDarkModeToggle();
        updateCurrentThemeDisplay();

        // إظهار إشعار
        const t = translations[appSettings.language];
        showNotification(
          (isDarkMode ? "تم تفعيل" : "تم إيقاف") + " " + t.darkMode
        );
      }

      // مراقب تغيير الوضع المظلم من النظام
      window
        .matchMedia("(prefers-color-scheme: dark)")
        .addEventListener("change", (event) => {
          isDarkMode = event.matches;
          if (event.matches) {
            document.documentElement.classList.add("dark");
          } else {
            document.documentElement.classList.remove("dark");
          }
          updateDarkModeIcons();
          updateDarkModeToggle();
          updateCurrentThemeDisplay();
        });

      // تحديث عرض المظهر الحالي مع دعم الترجمة
      function updateCurrentThemeDisplay() {
        const currentThemeElement = document.getElementById("currentTheme");
        const t = translations[appSettings.language];
        if (isDarkMode) {
          appSettings.theme = t.dark;
        } else {
          appSettings.theme = t.light;
        }
        if (currentThemeElement) {
          currentThemeElement.textContent = appSettings.theme;
        }
      }

      // تحديث عناوين التطبيق حسب اللغة المحددة
      function updateAppTitleAndTagline() {
        const appTitleElement = document.getElementById("appTitle");
        const appTaglineElement = document.getElementById("appTagline");

        // اسم التطبيق يبقى ثابت دائماً "FLUXY"
        if (appTitleElement) {
          appTitleElement.textContent = "FLUXY";
        }

        // فقط العبارة التوضيحية تتغير حسب اللغة
        if (appTaglineElement) {
          const t = translations[appSettings.language];
          appTaglineElement.textContent = t.appSubtitle;
        }
      }

      // إعدادات التطبيق مع دعم اللغات المتعددة
      let appSettings = {
        darkMode: isDarkMode,
        animations: true,
        compactView: false,
        language: "العربية",
        theme: isDarkMode ? "مظلم" : "فاتح",
        display: "شبكة",
      };

      // ترجمات التطبيق مع دعم اللغات الثلاث - محدثة مع فصل العناوين
      const translations = {
        العربية: {
          appTitle: "FLUXY",
          appSubtitle: "اكتشف واستمتع بتطبيقاتك المفضلة",
          homePageTitle: "مرحباً بك في FLUXY",
          profilePageTitle: "مكتبة التطبيقات",
          exploreDesc: "تصفح واكتشف جميع التطبيقات المتاحة",
          searchPlaceholder: "ابحث عن تطبيق...",
          categorySearchPlaceholder: "ابحث في هذا القسم...",
          allApps: "جميع التطبيقات",
          productivity: "إنتاجية",
          entertainment: "ترفيه",
          tools: "أدوات",
          communication: "تواصل",
          media: "وسائط",
          noResults: "لا توجد نتائج",
          noResultsDesc: "لم نجد أي تطبيق يطابق بحثك",
          favorites: "التطبيقات المفضلة",
          emptyFavoritesTitle: "لا توجد تطبيقات مفضلة",
          emptyFavoritesDesc: "قم بإضافة تطبيقاتك المفضلة لتظهر هنا",
          addAppsBtn: "أضف التطبيقات",
          addAppsDesc: "استكشف مجموعة التطبيقات المتنوعة وأضف المفضل منها",
          profile: "التطبيقات",
          user: "المستخدم",
          userDesc: "مستخدم تطبيق مكتبة التطبيقات",
          appCount: "تطبيق",
          favoriteCount: "مفضل",
          rating: "تقييم",
          appSettings: "الإعدادات",
          darkMode: "الوضع المظلم",
          animations: "التأثيرات المتحركة",
          compactView: "العرض المضغوط",
          settings: "الإعدادات",
          generalSettings: "الإعدادات العامة",
          language: "اللغة",
          theme: "المظهر",
          display: "عرض التطبيقات",
          privacy: "الخصوصية والأمان",
          privacySettings: "إعدادات الخصوصية",
          security: "الأمان",
          other: "أخرى",
          helpSupport: "المساعدة والدعم",
          aboutApp: "حول التطبيق",
          logout: "تسجيل الخروج",
          home: "الرئيسية",
          favorite: "المفضلة",
          openApp: "فتح التطبيق",
          addFavorite: "مفضلة",
          removeFavorite: "إزالة من المفضلة",
          appDetails: "تفاصيل التطبيق",
          downloads: "مستخدم",
          developer: "المطور",
          version: "الإصدار",
          size: "الحجم",
          lastUpdate: "آخر تحديث",
          requirements: "متطلبات النظام",
          screenshots: "لقطات الشاشة",
          languageChanged: "تم تغيير اللغة إلى",
          auto: "تلقائي",
          light: "فاتح",
          dark: "مظلم",
          grid: "شبكة",
          list: "قائمة",
          menu: "القائمة",
          mostUsed: "الأكثر استعمالاً",
          topRated: "الأعلى تقييماً",
          newest: "الأحدث",
          featuredGames: "الألعاب المميزة",
          viewAll: "عرض الكل",
          browseAllApps: "تصفح جميع التطبيقات",
          discoverMore: "اكتشف أكثر من 1000+ تطبيق مختلف",
          quickSettings: "الإعدادات السريعة",
          quickCategories: "تصنيفات سريعة",
          loading: "جاري التحميل...",
          loadingApps: "جاري تحميل التطبيقات...",
          pageOf: "صفحة {page} من {total}",
          totalApps: "{total} تطبيق",
          goToPage: "الانتقال للصفحة:",
          jumpToPage: "انتقال",
          backToHome: "العودة للرئيسية",
          categoryMostUsedDesc: "اكتشف التطبيقات الأكثر استعمالاً",
          categoryTopRatedDesc: "اكتشف التطبيقات الأعلى تقييماً",
          categoryNewestDesc: "اكتشف أحدث التطبيقات",
          categoryFeaturedGamesDesc: "اكتشف أفضل الألعاب المميزة",
        },
        English: {
          appTitle: "FLUXY",
          appSubtitle: "Discover and enjoy your favorite apps",
          homePageTitle: "Welcome to FLUXY",
          profilePageTitle: "Apps Library",
          exploreDesc: "Browse and discover all available apps",
          searchPlaceholder: "Search for an app...",
          categorySearchPlaceholder: "Search in this category...",
          allApps: "All Apps",
          productivity: "Productivity",
          entertainment: "Entertainment",
          tools: "Tools",
          communication: "Communication",
          media: "Media",
          noResults: "No Results",
          noResultsDesc: "No app matches your search",
          favorites: "Favorite Apps",
          emptyFavoritesTitle: "No Favorite Apps",
          emptyFavoritesDesc: "Add your favorite apps to appear here",
          addAppsBtn: "Add Apps",
          addAppsDesc: "Explore the diverse collection and add your favorites",
          profile: "Apps",
          user: "User",
          userDesc: "App Library User",
          appCount: "App",
          favoriteCount: "Favorite",
          rating: "Rating",
          appSettings: "Settings",
          darkMode: "Dark Mode",
          animations: "Animations",
          compactView: "Compact View",
          settings: "Settings",
          generalSettings: "General Settings",
          language: "Language",
          theme: "Theme",
          display: "App Display",
          privacy: "Privacy & Security",
          privacySettings: "Privacy Settings",
          security: "Security",
          other: "Other",
          helpSupport: "Help & Support",
          aboutApp: "About App",
          logout: "Logout",
          home: "Home",
          favorite: "Favorites",
          openApp: "Open App",
          addFavorite: "Favorite",
          removeFavorite: "Remove from Favorites",
          appDetails: "App Details",
          downloads: "Users",
          developer: "Developer",
          version: "Version",
          size: "Size",
          lastUpdate: "Last Update",
          requirements: "System Requirements",
          screenshots: "Screenshots",
          languageChanged: "Language changed to",
          auto: "Auto",
          light: "Light",
          dark: "Dark",
          grid: "Grid",
          list: "List",
          menu: "Menu",
          mostUsed: "Most Used",
          topRated: "Top Rated",
          newest: "Newest",
          featuredGames: "Featured Games",
          viewAll: "View All",
          browseAllApps: "Browse All Apps",
          discoverMore: "Discover more than 1000+ different apps",
          quickSettings: "Quick Settings",
          quickCategories: "Quick Categories",
          loading: "Loading...",
          loadingApps: "Loading apps...",
          pageOf: "Page {page} of {total}",
          totalApps: "{total} apps",
          goToPage: "Go to page:",
          jumpToPage: "Go",
          backToHome: "Back to Home",
          categoryMostUsedDesc: "Discover the most used apps",
          categoryTopRatedDesc: "Discover the top rated apps",
          categoryNewestDesc: "Discover the newest apps",
          categoryFeaturedGamesDesc: "Discover the best featured games",
        },
        Français: {
          appTitle: "FLUXY",
          appSubtitle: "Découvrez et profitez de vos applications favorites",
          homePageTitle: "Bienvenue à FLUXY",
          profilePageTitle: "Bibliothèque d'Applications",
          exploreDesc:
            "Parcourez et découvrez toutes les applications disponibles",
          searchPlaceholder: "Rechercher une application...",
          categorySearchPlaceholder: "Rechercher dans cette catégorie...",
          allApps: "Toutes les Applications",
          productivity: "Productivité",
          entertainment: "Divertissement",
          tools: "Outils",
          communication: "Communication",
          media: "Médias",
          noResults: "Aucun Résultat",
          noResultsDesc: "Aucune application ne correspond à votre recherche",
          favorites: "Applications Favorites",
          emptyFavoritesTitle: "Aucune Application Favorite",
          emptyFavoritesDesc:
            "Ajoutez vos applications favorites pour qu'elles apparaissent ici",
          addAppsBtn: "Ajouter des Applications",
          addAppsDesc:
            "Explorez la collection diversifiée et ajoutez vos favoris",
          profile: "Applications",
          user: "Utilisateur",
          userDesc: "Utilisateur de Bibliothèque d'Applications",
          appCount: "Application",
          favoriteCount: "Favori",
          rating: "Évaluation",
          appSettings: "Paramètres",
          darkMode: "Mode Sombre",
          animations: "Animations",
          compactView: "Vue Compacte",
          settings: "Paramètres",
          generalSettings: "Paramètres Généraux",
          language: "Langue",
          theme: "Thème",
          display: "Affichage des Applications",
          privacy: "Confidentialité et Sécurité",
          privacySettings: "Paramètres de Confidentialité",
          security: "Sécurité",
          other: "Autres",
          helpSupport: "Aide et Support",
          aboutApp: "À Propos de l'Application",
          logout: "Déconnexion",
          home: "Accueil",
          favorite: "Favoris",
          openApp: "Ouvrir l'Application",
          addFavorite: "Favori",
          removeFavorite: "Retirer des Favoris",
          appDetails: "Détails de l'Application",
          downloads: "Utilisateurs",
          developer: "Développeur",
          version: "Version",
          size: "Taille",
          lastUpdate: "Dernière Mise à Jour",
          requirements: "Exigences Système",
          screenshots: "Captures d'Écran",
          languageChanged: "Langue changée en",
          auto: "Automatique",
          light: "Clair",
          dark: "Sombre",
          grid: "Grille",
          list: "Liste",
          menu: "Menu",
          mostUsed: "Les Plus Utilisées",
          topRated: "Les Mieux Notées",
          newest: "Les Plus Récentes",
          featuredGames: "Jeux en Vedette",
          viewAll: "Voir Tout",
          browseAllApps: "Parcourir Toutes les Applications",
          discoverMore: "Découvrez plus de 1000+ applications différentes",
          quickSettings: "Paramètres Rapides",
          quickCategories: "Catégories Rapides",
          loading: "Chargement...",
          loadingApps: "Chargement des applications...",
          pageOf: "Page {page} de {total}",
          totalApps: "{total} applications",
          goToPage: "Aller à la page:",
          jumpToPage: "Aller",
          backToHome: "Retour à l'accueil",
          categoryMostUsedDesc: "Découvrez les applications les plus utilisées",
          categoryTopRatedDesc: "Découvrez les applications les mieux notées",
          categoryNewestDesc: "Découvrez les applications les plus récentes",
          categoryFeaturedGamesDesc: "Découvrez les meilleurs jeux en vedette",
        },
      };

      // دالة تطبيق الترجمة على واجهة المستخدم (محدثة مع العناوين المنفصلة)
      function applyLanguage(language) {
        const t = translations[language];
        if (!t) return;

        // تحديث اتجاه الصفحة وفئة اللغة
        const body = document.body;
        const html = document.documentElement;

        // إزالة فئات اللغة السابقة
        body.classList.remove("lang-english", "lang-french");

        if (language === "English" || language === "Français") {
          html.setAttribute("dir", "ltr");
          if (language === "English") {
            body.classList.add("lang-english");
          } else {
            body.classList.add("lang-french");
          }
        } else {
          html.setAttribute("dir", "rtl");
        }

        // تحديث عناوين التطبيق في الشريط العلوي (يبقى ثابت)
        updateAppTitleAndTagline();

        // تحديث النصوص في واجهة المستخدم
        const elements = {
          // العناوين الرئيسية - محدثة باستخدام المتغيرات المنفصلة
          homeTitle: t.homePageTitle,
          homeSubtitle: t.appSubtitle,
          profileTitle: t.profilePageTitle,
          profileSubtitle: t.exploreDesc,
          favoritesTitle: t.favorites,
          settingsTitle: t.settings,

          // القائمة الجانبية
          menuTitle: t.menu,
          menuHome: t.home,
          menuFavorites: t.favorite,
          menuApps: t.profile,
          menuSettings: t.settings,

          // التصنيفات
          categoryProductivity: t.productivity,
          categoryEntertainment: t.entertainment,
          categoryTools: t.tools,
          categoryCommunication: t.communication,
          categoryMedia: t.media,
          quickCategoriesTitle: t.quickCategories,

          // أزرار التصنيفات
          allAppsBtn: t.allApps,
          productivityBtn: t.productivity,
          entertainmentBtn: t.entertainment,
          toolsBtn: t.tools,
          communicationBtn: t.communication,
          mediaBtn: t.media,

          // أقسام الصفحة الرئيسية
          mostUsedTitle: t.mostUsed,
          topRatedTitle: t.topRated,
          newestTitle: t.newest,
          featuredGamesTitle: t.featuredGames,
          browseAllAppsBtn: t.browseAllApps,
          discoverMoreText: t.discoverMore,

          // أزرار عرض الكل
          mostUsedViewAll: t.viewAll + " →",
          topRatedViewAll: t.viewAll + " →",
          newestViewAll: t.viewAll + " →",
          featuredGamesViewAll: t.viewAll + " →",

          // صفحة المفضلة المحدثة
          emptyFavoritesTitle: t.emptyFavoritesTitle,
          emptyFavoritesDesc: t.emptyFavoritesDesc,
          addAppsBtn: t.addAppsBtn,
          addAppsDesc: t.addAppsDesc,

          // رسائل عدم وجود نتائج
          noResultsTitle: t.noResults,
          noResultsDesc: t.noResultsDesc,
          categoryNoResultsTitle: t.noResults,
          categoryNoResultsDesc: t.noResultsDesc,

          // شريط التنقل السفلي
          navHome: t.home,
          navFavorites: t.favorite,
          navApps: t.profile,
          navSettings: t.settings,

          // الإعدادات
          quickSettingsTitle: t.quickSettings,
          generalSettingsTitle: t.generalSettings,
          darkModeLabel: t.darkMode,
          animationsLabel: t.animations,
          compactViewLabel: t.compactView,
          languageLabel: t.language,
          themeLabel: t.theme,
          displayLabel: t.display,

          // النافذة المنبثقة
          modalTitle: t.appDetails,
          openAppBtn: t.openApp,
          favoriteText: t.addFavorite,
          downloadsLabel: t.downloads,
          ratingLabel: t.rating,
          developerLabel: t.developer,
          versionLabel: t.version,
          sizeLabel: t.size,
          lastUpdateLabel: t.lastUpdate,
          languageDetailLabel: t.language,
          requirementsLabel: t.requirements,
          screenshotsLabel: t.screenshots,

          // نظام الصفحات الجديد
          loadingText: t.loadingApps,
          categoryLoadingText: t.loadingApps,
          goToPageLabel: t.goToPage,
          goToPageBtn: t.jumpToPage,
          categoryGoToPageLabel: t.goToPage,
          categoryGoToPageBtn: t.jumpToPage,

          // صفحة الأقسام المميزة
          backToHomeBtn: t.backToHome,
        };

        Object.entries(elements).forEach(([id, text]) => {
          const element = document.getElementById(id);
          if (element) {
            element.textContent = text;
          }
        });

        // تحديث placeholders
        const searchInputs = document.querySelectorAll(
          "#searchInput, #homeSearchInput"
        );
        searchInputs.forEach((input) => {
          input.placeholder = t.searchPlaceholder;
        });

        const categorySearchInput = document.getElementById(
          "categorySearchInput"
        );
        if (categorySearchInput) {
          categorySearchInput.placeholder = t.categorySearchPlaceholder;
        }

        // تحديث العرض الحالي للإعدادات
        const currentDisplay = document.getElementById("currentDisplay");
        if (currentDisplay) {
          if (
            appSettings.display === "شبكة" ||
            appSettings.display === "Grid" ||
            appSettings.display === "Grille"
          ) {
            currentDisplay.textContent = t.grid;
          } else {
            currentDisplay.textContent = t.list;
          }
        }

        // تحديث المظهر الحالي
        const currentTheme = document.getElementById("currentTheme");
        if (currentTheme) {
          if (isDarkMode) {
            currentTheme.textContent = t.dark;
          } else {
            currentTheme.textContent = t.light;
          }
        }

        // تحديث معلومات الصفحة
        updatePageInfo();
        updateCategoryPageInfo();
      }

      // وظائف القائمة الجانبية
      function toggleSideMenu() {
        const sideMenu = document.getElementById("sideMenu");
        const menuOverlay = document.getElementById("menuOverlay");
        const hamburgerBtn = document.getElementById("hamburgerBtn");

        sideMenu.classList.toggle("active");
        menuOverlay.classList.toggle("active");
        hamburgerBtn.classList.toggle("active");

        if (sideMenu.classList.contains("active")) {
          document.body.style.overflow = "hidden";
        } else {
          document.body.style.overflow = "auto";
        }
      }

      function closeSideMenu() {
        const sideMenu = document.getElementById("sideMenu");
        const menuOverlay = document.getElementById("menuOverlay");
        const hamburgerBtn = document.getElementById("hamburgerBtn");

        sideMenu.classList.remove("active");
        menuOverlay.classList.remove("active");
        hamburgerBtn.classList.remove("active");
        document.body.style.overflow = "auto";
      }

      function navigateToSection(sectionId) {
        // تحديث القائمة الجانبية
        document.querySelectorAll(".side-menu .menu-item").forEach((item) => {
          item.classList.remove("active");
        });
        const menuItem = document.querySelector(
          `[data-section="${sectionId}"]`
        );
        if (menuItem) {
          menuItem.classList.add("active");
        }

        // تحديث شريط التنقل السفلي
        switchSection(sectionId);

        // إغلاق القائمة
        closeSideMenu();
      }

      // دالة جديدة للانتقال من المفضلة إلى التطبيقات
      function navigateToAppsFromFavorites() {
        const t = translations[appSettings.language];

        // التنقل لصفحة التطبيقات
        navigateToSection("profileSection");

        // إظهار إشعار
        setTimeout(() => {
          showNotification(t.browseAllApps + " - " + t.addAppsDesc);
        }, 500);
      }

      function quickFilterCategory(category) {
        // التنقل إلى صفحة التطبيقات
        navigateToSection("profileSection");

        // تطبيق الفلتر
        setTimeout(() => {
          filterByCategory(category);
        }, 100);
      }

      // وظائف أزرار الملف الشخصي - محدثة لتعمل فقط عند الضغط على التبديل مع الـ Switches الجديدة
      function toggleDarkMode(event) {
        if (event) {
          event.stopPropagation(); // منع انتشار الحدث
        }

        isDarkMode = !isDarkMode;
        appSettings.darkMode = isDarkMode;

        if (isDarkMode) {
          document.documentElement.classList.add("dark");
        } else {
          document.documentElement.classList.remove("dark");
        }

        updateToggleSwitchModern("darkModeToggle", isDarkMode);
        updateDarkModeIcons();
        updateCurrentThemeDisplay();

        const t = translations[appSettings.language];
        showNotification(
          (isDarkMode ? "تم تفعيل" : "تم إيقاف") + " " + t.darkMode
        );
      }

      function toggleAnimations(event) {
        if (event) {
          event.stopPropagation();
        }

        appSettings.animations = !appSettings.animations;
        updateToggleSwitchModern("animationsToggle", appSettings.animations);

        // تطبيق/إلغاء التأثيرات المتحركة
        const elements = document.querySelectorAll(
          ".app-card, .category-btn, .nav-item, .settings-item"
        );
        elements.forEach((element) => {
          if (appSettings.animations) {
            element.style.transition = "";
          } else {
            element.style.transition = "none";
          }
        });

        const t = translations[appSettings.language];
        showNotification(
          (appSettings.animations ? "تم تفعيل" : "تم إيقاف") +
            " " +
            t.animations
        );
      }

      function toggleCompactView(event) {
        if (event) {
          event.stopPropagation();
        }

        appSettings.compactView = !appSettings.compactView;
        saveCompactView();
        saveAppSettings();
        updateToggleSwitchModern("compactViewToggle", appSettings.compactView);

        // تطبيق/إلغاء العرض المضغوط
        const appsGrid = document.getElementById("appsGrid");
        if (appsGrid && appSettings.compactView) {
          appsGrid.className =
            "grid grid-cols-3 md:grid-cols-4 lg:grid-cols-5 xl:grid-cols-6 gap-4 mb-8";
        } else if (appsGrid) {
          appsGrid.className = "apps-grid-enhanced mb-8";
        }

        // إعادة عرض التطبيقات بالتخطيط الجديد
        displayApps();

        const t = translations[appSettings.language];
        showNotification(
          (appSettings.compactView ? "تم تفعيل" : "تم إيقاف") +
            " " +
            t.compactView
        );
      }

      function updateToggleSwitchModern(toggleId, isActive) {
        const toggle = document.getElementById(toggleId);
        if (!toggle) return;

        const circle = toggle.querySelector(".toggle-circle-modern");

        if (isActive) {
          toggle.classList.add("active");
          toggle.classList.remove("inactive");
          circle.classList.add("left");
          circle.classList.remove("right");
        } else {
          toggle.classList.remove("active");
          toggle.classList.add("inactive");
          circle.classList.remove("left");
          circle.classList.add("right");
        }
      }

      function updateToggleSwitch(toggleId, isActive) {
        const toggle = document.getElementById(toggleId);
        if (!toggle) return;

        const circle = toggle.querySelector(".toggle-circle");

        if (isActive) {
          toggle.classList.add("active");
          toggle.classList.remove("inactive");
          circle.classList.add("left");
          circle.classList.remove("right");
        } else {
          toggle.classList.remove("active");
          toggle.classList.add("inactive");
          circle.classList.remove("left");
          circle.classList.add("right");
        }
      }

      function updateDarkModeToggle() {
        updateToggleSwitchModern("darkModeToggle", isDarkMode);
      }

      // وظائف أزرار الإعدادات مع دعم اللغات المتعددة
      function openLanguageSettings() {
        const t = translations[appSettings.language];
        showSettingsModal(
          t.language + " " + t.settings,
          `
                  <div class="space-y-3">
                      <div class="flex items-center justify-between p-3 rounded-lg border border-gray-200 dark:border-gray-600 cursor-pointer ${
                        appSettings.language === "العربية"
                          ? "bg-primary text-white"
                          : "hover:bg-gray-50 dark:hover:bg-gray-700"
                      }" onclick="changeLanguage('العربية')">
                          <span>العربية</span>
                          ${
                            appSettings.language === "العربية"
                              ? "<span>✓</span>"
                              : ""
                          }
                      </div>
                      <div class="flex items-center justify-between p-3 rounded-lg border border-gray-200 dark:border-gray-600 cursor-pointer ${
                        appSettings.language === "English"
                          ? "bg-primary text-white"
                          : "hover:bg-gray-50 dark:hover:bg-gray-700"
                      }" onclick="changeLanguage('English')">
                          <span>English</span>
                          ${
                            appSettings.language === "English"
                              ? "<span>✓</span>"
                              : ""
                          }
                      </div>
                      <div class="flex items-center justify-between p-3 rounded-lg border border-gray-200 dark:border-gray-600 cursor-pointer ${
                        appSettings.language === "Français"
                          ? "bg-primary text-white"
                          : "hover:bg-gray-50 dark:hover:bg-gray-700"
                      }" onclick="changeLanguage('Français')">
                          <span>Français</span>
                          ${
                            appSettings.language === "Français"
                              ? "<span>✓</span>"
                              : ""
                          }
                      </div>
                  </div>
              `
        );
      }

      function openThemeSettings() {
        const t = translations[appSettings.language];
        showSettingsModal(
          t.theme + " " + t.settings,
          `
                  <div class="space-y-3">
                      <div class="flex items-center justify-between p-3 rounded-lg border border-gray-200 dark:border-gray-600 cursor-pointer ${
                        appSettings.theme === "تلقائي" ||
                        appSettings.theme === "Auto" ||
                        appSettings.theme === "Automatique"
                          ? "bg-primary text-white"
                          : "hover:bg-gray-50 dark:hover:bg-gray-700"
                      }" onclick="changeTheme('تلقائي', '${t.auto}')">
                          <span>${t.auto}</span>
                          ${
                            appSettings.theme === "تلقائي" ||
                            appSettings.theme === "Auto" ||
                            appSettings.theme === "Automatique"
                              ? "<span>✓</span>"
                              : ""
                          }
                      </div>
                      <div class="flex items-center justify-between p-3 rounded-lg border border-gray-200 dark:border-gray-600 cursor-pointer ${
                        appSettings.theme === "فاتح" ||
                        appSettings.theme === "Light" ||
                        appSettings.theme === "Clair"
                          ? "bg-primary text-white"
                          : "hover:bg-gray-50 dark:hover:bg-gray-700"
                      }" onclick="changeTheme('فاتح', '${t.light}')">
                          <span>${t.light}</span>
                          ${
                            appSettings.theme === "فاتح" ||
                            appSettings.theme === "Light" ||
                            appSettings.theme === "Clair"
                              ? "<span>✓</span>"
                              : ""
                          }
                      </div>
                      <div class="flex items-center justify-between p-3 rounded-lg border border-gray-200 dark:border-gray-600 cursor-pointer ${
                        appSettings.theme === "مظلم" ||
                        appSettings.theme === "Dark" ||
                        appSettings.theme === "Sombre"
                          ? "bg-primary text-white"
                          : "hover:bg-gray-50 dark:hover:bg-gray-700"
                      }" onclick="changeTheme('مظلم', '${t.dark}')">
                          <span>${t.dark}</span>
                          ${
                            appSettings.theme === "مظلم" ||
                            appSettings.theme === "Dark" ||
                            appSettings.theme === "Sombre"
                              ? "<span>✓</span>"
                              : ""
                          }
                      </div>
                  </div>
              `
        );
      }

      function openDisplaySettings() {
        const t = translations[appSettings.language];
        showSettingsModal(
          t.display + " " + t.settings,
          `
                  <div class="space-y-3">
                      <div class="flex items-center justify-between p-3 rounded-lg border border-gray-200 dark:border-gray-600 cursor-pointer ${
                        appSettings.display === "شبكة" ||
                        appSettings.display === "Grid" ||
                        appSettings.display === "Grille"
                          ? "bg-primary text-white"
                          : "hover:bg-gray-50 dark:hover:bg-gray-700"
                      }" onclick="changeDisplay('شبكة', '${t.grid}')">
                          <span>${t.grid}</span>
                          ${
                            appSettings.display === "شبكة" ||
                            appSettings.display === "Grid" ||
                            appSettings.display === "Grille"
                              ? "<span>✓</span>"
                              : ""
                          }
                      </div>
                      <div class="flex items-center justify-between p-3 rounded-lg border border-gray-200 dark:border-gray-600 cursor-pointer ${
                        appSettings.display === "قائمة" ||
                        appSettings.display === "List" ||
                        appSettings.display === "Liste"
                          ? "bg-primary text-white"
                          : "hover:bg-gray-50 dark:hover:bg-gray-700"
                      }" onclick="changeDisplay('قائمة', '${t.list}')">
                          <span>${t.list}</span>
                          ${
                            appSettings.display === "قائمة" ||
                            appSettings.display === "List" ||
                            appSettings.display === "Liste"
                              ? "<span>✓</span>"
                              : ""
                          }
                      </div>
                  </div>
              `
        );
      }

      // وظائف تغيير الإعدادات مع دعم الترجمة
      function changeLanguage(language) {
        appSettings.language = language;
        const currentLanguageElement =
          document.getElementById("currentLanguage");
        if (currentLanguageElement) {
          currentLanguageElement.textContent = language;
        }

        // تطبيق الترجمة الجديدة
        applyLanguage(language);

        closeSettingsModal();
        showNotification(
          translations[language].languageChanged + " " + language
        );
      }

      function changeTheme(theme, displayText) {
        appSettings.theme = displayText || theme;
        document.getElementById("currentTheme").textContent =
          displayText || theme;

        if (
          theme === "فاتح" ||
          displayText === "Light" ||
          displayText === "Clair"
        ) {
          document.documentElement.classList.remove("dark");
          isDarkMode = false;
        } else if (
          theme === "مظلم" ||
          displayText === "Dark" ||
          displayText === "Sombre"
        ) {
          document.documentElement.classList.add("dark");
          isDarkMode = true;
        } else {
          // تلقائي - حسب إعدادات النظام
          if (
            window.matchMedia &&
            window.matchMedia("(prefers-color-scheme: dark)").matches
          ) {
            document.documentElement.classList.add("dark");
            isDarkMode = true;
          } else {
            document.documentElement.classList.remove("dark");
            isDarkMode = false;
          }
        }

        updateDarkModeToggle();
        updateDarkModeIcons();
        closeSettingsModal();

        const t = translations[appSettings.language];
        showNotification(
          t.languageChanged.replace("اللغة", t.theme) +
            " " +
            (displayText || theme)
        );
      }

      function changeDisplay(display, displayText) {
        appSettings.display = displayText || display;
        document.getElementById("currentDisplay").textContent =
          displayText || display;
        closeSettingsModal();

        const t = translations[appSettings.language];
        showNotification(
          t.languageChanged.replace("اللغة", t.display) +
            " " +
            (displayText || display)
        );
      }

      // وظائف النوافذ المنبثقة للإعدادات
      function showSettingsModal(title, content) {
        document.getElementById("settingsModalTitle").textContent = title;
        document.getElementById("settingsModalContent").innerHTML = content;
        document.getElementById("settingsModal").classList.remove("hidden");
        document.body.style.overflow = "hidden";
      }

      function closeSettingsModal() {
        document.getElementById("settingsModal").classList.add("hidden");
        document.body.style.overflow = "auto";
      }

      // دالة إظهار الإشعارات المحسنة للوضع المظلم
      function showNotification(message) {
        // إنشاء عنصر الإشعار
        const notification = document.createElement("div");
        notification.className =
          "notification fixed top-20 right-4 bg-primary dark:bg-gray-700 text-white px-4 py-3 rounded-lg shadow-lg z-[60] transform translate-x-full transition-transform duration-300";
        notification.textContent = message;

        // تغيير موقع الإشعار حسب اللغة
        if (
          appSettings.language === "English" ||
          appSettings.language === "Français"
        ) {
          notification.style.right = "auto";
          notification.style.left = "1rem";
          notification.classList.remove("translate-x-full");
          notification.classList.add("-translate-x-full");
        }

        document.body.appendChild(notification);

        // إظهار الإشعار
        setTimeout(() => {
          if (
            appSettings.language === "English" ||
            appSettings.language === "Français"
          ) {
            notification.classList.remove("-translate-x-full");
          } else {
            notification.classList.remove("translate-x-full");
          }
        }, 100);

        // إخفاء الإشعار بعد 3 ثوانِ
        setTimeout(() => {
          if (
            appSettings.language === "English" ||
            appSettings.language === "Français"
          ) {
            notification.classList.add("-translate-x-full");
          } else {
            notification.classList.add("translate-x-full");
          }
          setTimeout(() => {
            if (notification.parentNode) {
              document.body.removeChild(notification);
            }
          }, 300);
        }, 3000);
      }

      // بيانات التطبيقات مع التصنيفات والتفاصيل
      const apps = [
        {
          id: 1,
          name: "الآلة الحاسبة",
          category: "tools",
          url: "https://marwannndea.github.io/equation-solver/",
          image:
            "https://marketplace.canva.com/EOHgQ/MAGyKiEOHgQ/1/tl/canva-calculator-icon-illustration-MAGyKiEOHgQ.png",
          description:
            "تطبيق حاسبة قوي يدعم العمليات الأساسية والمتقدمة مع واجهة سهلة الاستخدام وتصميم حديث",
          version: "2.1.0",
          size: "5.2 ميجابايت",
          categoryName: "أدوات",
          developer: "TechApps Inc",
          rating: 4.8,
          downloads: "2.5M+",
          lastUpdate: "2024/11/15",
          language: "العربية، الإنجليزية",
          requirements: "Android 5.0+",
          screenshots: [
            "https://picsum.photos/200/400?random=1",
            "https://picsum.photos/200/400?random=2",
            "https://picsum.photos/200/400?random=3",
          ],
        },
        {
          id: 2,
          name: "المفكرة",
          category: "productivity",
          image:
            "https://upload.wikimedia.org/wikipedia/commons/c/c9/Windows_Notepad_icon.png",
          description:
            "مفكرة بسيطة لكتابة الملاحظات والأفكار مع إمكانية الحفظ والتنظيم",
          version: "1.8.5",
          size: "3.1 ميجابايت",
          categoryName: "إنتاجية",
          developer: "SimpleApps",
          rating: 4.5,
          downloads: "1.2M+",
          lastUpdate: "2024/10/28",
          language: "العربية، الإنجليزية",
          requirements: "Android 4.0+",
          screenshots: [
            "https://picsum.photos/200/400?random=10",
            "https://picsum.photos/200/400?random=11",
          ],
        },
        {
          id: 3,
          name: "التقويم",
          category: "productivity",
          image: "https://picsum.photos/300/300?random=3",
          description: "تطبيق تقويم شامل لإدارة المواعيد والأحداث مع تذكير ذكي",
          version: "3.0.2",
          size: "8.7 ميجابايت",
          categoryName: "إنتاجية",
          developer: "CalendarPro",
          rating: 4.7,
          downloads: "3.8M+",
          lastUpdate: "2024/11/10",
          language: "العربية، الإنجليزية",
          requirements: "Android 6.0+",
          screenshots: [
            "https://picsum.photos/200/400?random=12",
            "https://picsum.photos/200/400?random=13",
            "https://picsum.photos/200/400?random=14",
          ],
        },
        {
          id: 4,
          name: "الطقس",
          category: "tools",
          image:
            "https://upload.wikimedia.org/wikipedia/commons/1/1e/Weather_%28iOS%29.png",
          description:
            "تطبيق طقس دقيق يعرض حالة الطقس الحالية والتوقعات للأيام القادمة",
          version: "4.2.1",
          size: "12.5 ميجابايت",
          categoryName: "أدوات",
          developer: "WeatherTech",
          rating: 4.6,
          downloads: "5.1M+",
          lastUpdate: "2024/11/20",
          language: "العربية، الإنجليزية",
          requirements: "Android 5.0+",
          screenshots: [
            "https://picsum.photos/200/400?random=15",
            "https://picsum.photos/200/400?random=16",
          ],
        },
        {
          id: 5,
          name: "الساعة",
          category: "tools",
          image:
            "https://videos.openai.com/az/vg-assets/task_01kam8wg4de7vrt7nz5gmnzac1%2F1763764549_img_0.webp?se=2025-11-26T00%3A00%3A00Z&sp=r&sv=2024-08-04&sr=b&skoid=8ffff87a-01f1-47c9-9090-32999d4d6380&sktid=a48cca56-e6da-484e-a814-9c849652bcb3&skt=2025-11-21T01%3A09%3A51Z&ske=2025-11-28T01%3A14%3A51Z&sks=b&skv=2024-08-04&sig=wI6yUphpJQSsyVBzOvAmZ22ccQotkZp0W4/3NxL5HuA%3D&ac=oaivgprodscus2",
          description: "ساعة رقمية مع منبه وموقت ومؤقت عد تنازلي",
          version: "2.5.0",
          size: "4.3 ميجابايت",
          categoryName: "أدوات",
          developer: "TimeApps",
          rating: 4.4,
          downloads: "900K+",
          lastUpdate: "2024/09/15",
          language: "العربية، الإنجليزية",
          requirements: "Android 4.4+",
          screenshots: ["https://picsum.photos/200/400?random=17"],
        },
        {
          id: 6,
          name: "الكاميرا",
          category: "media",
          image:
            "https://play-lh.googleusercontent.com/djyVyf494z2-Ik7BSp-eBnfAmzsdZ24txehytJGbAGLxAIrAZ37kYRrfbL_NkXM8mcrDZtGG3bXD3tFF5TC7luo",
          description:
            "تطبيق كاميرا متقدم لالتقاط الصور ومقاطع الفيديو بجودة عالية",
          version: "5.1.3",
          size: "25.8 ميجابايت",
          categoryName: "وسائط",
          developer: "CameraPlus",
          rating: 4.8,
          downloads: "10M+",
          lastUpdate: "2024/11/18",
          language: "العربية، الإنجليزية",
          requirements: "Android 7.0+",
          screenshots: [
            "https://picsum.photos/200/400?random=18",
            "https://picsum.photos/200/400?random=19",
            "https://picsum.photos/200/400?random=20",
            "https://picsum.photos/200/400?random=21",
          ],
        },
        {
          id: 7,
          name: "الموسيقى",
          category: "media",
          image:
            "https://videos.openai.com/az/vg-assets/task_01kankegqafc4r4b3nvws4wfv6%2F1763809174_img_0.webp?se=2025-11-26T00%3A00%3A00Z&sp=r&sv=2024-08-04&sr=b&skoid=cfbc986b-d2bc-4088-8b71-4f962129715b&sktid=a48cca56-e6da-484e-a814-9c849652bcb3&skt=2025-11-22T01%3A09%3A13Z&ske=2025-11-29T01%3A14%3A13Z&sks=b&skv=2024-08-04&sig=qXUCCTGjXu6ui8dPytiZi5P0EL2aShp7hech4BROw9Y%3D&ac=oaivgprodscus2",
          description: "مشغل موسيقى قوي يدعم جميع صيغ الصوت مع واجهة جميلة",
          version: "3.7.2",
          size: "18.4 ميجابايت",
          categoryName: "وسائط",
          developer: "MusicPro",
          rating: 4.7,
          downloads: "7.2M+",
          lastUpdate: "2024/11/05",
          language: "العربية، الإنجليزية",
          requirements: "Android 6.0+",
          screenshots: [
            "https://picsum.photos/200/400?random=22",
            "https://picsum.photos/200/400?random=23",
          ],
        },
        {
          id: 8,
          name: "الخرائط",
          category: "tools",
          image:
            "https://videos.openai.com/az/vg-assets/task_01kankvfnpfkr9kgnzndcnt8hw%2F1763809608_img_0.webp?se=2025-11-26T00%3A00%3A00Z&sp=r&sv=2024-08-04&sr=b&skoid=cfbc986b-d2bc-4088-8b71-4f962129715b&sktid=a48cca56-e6da-484e-a814-9c849652bcb3&skt=2025-11-22T01%3A09%3A13Z&ske=2025-11-29T01%3A14%3A13Z&sks=b&skv=2024-08-04&sig=Zeprsjeh2i71tRlGOeBu35KZc56d8TL3ekaHHp%2B5ieI%3D&ac=oaivgprodscus2",
          description: "تطبيق خرائط تفاعلي مع نظام تنقل ذكي وتحديد المواقع",
          version: "6.0.1",
          size: "45.2 ميجابايت",
          categoryName: "أدوات",
          developer: "MapTech",
          rating: 4.5,
          downloads: "15M+",
          lastUpdate: "2024/11/12",
          language: "العربية، الإنجليزية",
          requirements: "Android 8.0+",
          screenshots: [
            "https://picsum.photos/200/400?random=24",
            "https://picsum.photos/200/400?random=25",
            "https://picsum.photos/200/400?random=26",
          ],
        },
        {
          id: 9,
          name: "الإعدادات",
          category: "tools",
          image: "https://picsum.photos/300/300?random=9",
          description: "تطبيق إعدادات شامل للتحكم في جميع خصائص النظام",
          version: "1.0.0",
          size: "2.8 ميجابايت",
          categoryName: "أدوات",
          developer: "SystemApps",
          rating: 4.2,
          downloads: "500K+",
          lastUpdate: "2024/08/20",
          language: "العربية، الإنجليزية",
          requirements: "Android 5.0+",
          screenshots: ["https://picsum.photos/200/400?random=27"],
        },
        {
          id: 10,
          name: "البريد الإلكتروني",
          category: "communication",
          image: "https://picsum.photos/300/300?random=10",
          description:
            "عميل بريد إلكتروني متقدم يدعم عدة حسابات وتنظيم الرسائل",
          version: "4.5.6",
          size: "22.1 ميجابايت",
          categoryName: "تواصل",
          developer: "EmailPro",
          rating: 4.6,
          downloads: "6.3M+",
          lastUpdate: "2024/11/08",
          language: "العربية، الإنجليزية",
          requirements: "Android 6.0+",
          screenshots: [
            "https://picsum.photos/200/400?random=28",
            "https://picsum.photos/200/400?random=29",
          ],
        },
        {
          id: 11,
          name: "المتصفح",
          category: "productivity",
          image: "https://picsum.photos/300/300?random=11",
          description: "متصفح إنترنت سريع وآمن مع حماية الخصوصية",
          version: "8.2.0",
          size: "35.7 ميجابايت",
          categoryName: "إنتاجية",
          developer: "BrowserTech",
          rating: 4.7,
          downloads: "12M+",
          lastUpdate: "2024/11/22",
          language: "العربية، الإنجليزية",
          requirements: "Android 7.0+",
          screenshots: [
            "https://picsum.photos/200/400?random=30",
            "https://picsum.photos/200/400?random=31",
            "https://picsum.photos/200/400?random=32",
          ],
        },
        {
          id: 12,
          name: "المعرض",
          category: "media",
          image: "https://picsum.photos/300/300?random=12",
          description: "عارض صور ومقاطع فيديو مع إمكانيات التحرير الأساسية",
          version: "2.9.1",
          size: "15.3 ميجابايت",
          categoryName: "وسائط",
          developer: "GalleryApps",
          rating: 4.4,
          downloads: "4.1M+",
          lastUpdate: "2024/10/30",
          language: "العربية، الإنجليزية",
          requirements: "Android 5.0+",
          screenshots: [
            "https://picsum.photos/200/400?random=33",
            "https://picsum.photos/200/400?random=34",
          ],
        },
        {
          id: 13,
          name: "محرر النصوص",
          category: "productivity",
          image: "https://picsum.photos/300/300?random=13",
          description: "محرر نصوص قوي يدعم البرمجة والتنسيق المتقدم",
          version: "7.1.4",
          size: "28.9 ميجابايت",
          categoryName: "إنتاجية",
          developer: "TextEditor Inc",
          rating: 4.5,
          downloads: "2.8M+",
          lastUpdate: "2024/11/01",
          language: "العربية، الإنجليزية",
          requirements: "Android 6.0+",
          screenshots: [
            "https://picsum.photos/200/400?random=35",
            "https://picsum.photos/200/400?random=36",
            "https://picsum.photos/200/400?random=37",
          ],
        },
        {
          id: 14,
          name: "مشغل الفيديو",
          category: "media",
          image: "https://picsum.photos/300/300?random=14",
          description: "مشغل فيديو متقدم يدعم جميع صيغ الفيديو والترجمة",
          version: "4.8.2",
          size: "31.6 ميجابايت",
          categoryName: "وسائط",
          developer: "VideoPlayer Pro",
          rating: 4.6,
          downloads: "8.5M+",
          lastUpdate: "2024/11/14",
          language: "العربية، الإنجليزية",
          requirements: "Android 6.0+",
          screenshots: [
            "https://picsum.photos/200/400?random=38",
            "https://picsum.photos/200/400?random=39",
          ],
        },
        {
          id: 15,
          name: "الألعاب",
          category: "entertainment",
          image: "https://picsum.photos/300/300?random=15",
          description: "مجموعة ألعاب مسلية ومتنوعة لجميع الأعمار",
          version: "1.5.7",
          size: "67.4 ميجابايت",
          categoryName: "ترفيه",
          developer: "GameStudio",
          rating: 4.3,
          downloads: "11M+",
          lastUpdate: "2024/11/06",
          language: "العربية، الإنجليزية",
          requirements: "Android 7.0+",
          screenshots: [
            "https://picsum.photos/200/400?random=40",
            "https://picsum.photos/200/400?random=41",
            "https://picsum.photos/200/400?random=42",
          ],
        },
        {
          id: 16,
          name: "التسوق",
          category: "entertainment",
          image: "https://picsum.photos/300/300?random=16",
          description: "تطبيق تسوق إلكتروني آمن مع عروض حصرية",
          version: "3.3.8",
          size: "19.2 ميجابايت",
          categoryName: "ترفيه",
          developer: "ShopApp",
          rating: 4.4,
          downloads: "9.7M+",
          lastUpdate: "2024/11/16",
          language: "العربية، الإنجليزية",
          requirements: "Android 6.0+",
          screenshots: [
            "https://picsum.photos/200/400?random=43",
            "https://picsum.photos/200/400?random=44",
          ],
        },
        {
          id: 17,
          name: "الأخبار",
          category: "communication",
          image: "https://picsum.photos/300/300?random=17",
          description: "تطبيق أخبار شامل يجمع الأخبار من مصادر موثوقة",
          version: "5.6.0",
          size: "14.8 ميجابايت",
          categoryName: "تواصل",
          developer: "NewsNetwork",
          rating: 4.5,
          downloads: "6.8M+",
          lastUpdate: "2024/11/19",
          language: "العربية، الإنجليزية",
          requirements: "Android 5.0+",
          screenshots: [
            "https://picsum.photos/200/400?random=45",
            "https://picsum.photos/200/400?random=46",
            "https://picsum.photos/200/400?random=47",
          ],
        },
        {
          id: 18,
          name: "الرياضة",
          category: "entertainment",
          image:
            "https://img.kwcdn.com/product/fancy/67b885d7-cfb2-4685-bf5f-6b873803de34.jpg",
          description: "تطبيق رياضي للمتابعة المباشرة للمباريات والنتائج",
          version: "2.4.3",
          size: "21.7 ميجابايت",
          categoryName: "ترفيه",
          developer: "SportsApp",
          rating: 4.2,
          downloads: "4.3M+",
          lastUpdate: "2024/11/11",
          language: "العربية، الإنجليزية",
          requirements: "Android 5.0+",
          screenshots: [
            "https://picsum.photos/200/400?random=48",
            "https://picsum.photos/200/400?random=49",
          ],
        },
      ];

      // متغيرات التحكم في الصفحات والبحث والفلترة المحسنة
      let currentPage = 1;
      const appsPerPage = 12;
      let filteredApps = [...apps];
      let isSearching = false;
      let activeCategory = "all";
      let currentAppIndex = -1;
      let totalAppsCount = apps.length;

      // متغيرات خاصة بصفحة الأقسام المميزة
      let currentCategoryPage = 1;
      let filteredCategoryApps = [];
      let currentCategoryType = "";
      let isCategorySearching = false;

      // المفضلة - نستخدم مصفوفة لحفظ معرفات التطبيقات المفضلة
      let favoriteApps = [];

      // دالة التنقل بين الأقسام
      function switchSection(targetSectionId) {
        // إخفاء جميع الأقسام
        document.querySelectorAll(".content-section").forEach((section) => {
          section.classList.remove("active");
        });

        // إظهار القسم المحدد
        document.getElementById(targetSectionId).classList.add("active");

        // تحديث شريط التنقل
        document.querySelectorAll(".nav-item").forEach((item) => {
          item.classList.remove("active");
        });

        const navItem = document.querySelector(
          `[data-section="${targetSectionId}"]`
        );
        if (navItem) {
          navItem.classList.add("active");
        }

        // تحديث المحتوى حسب القسم
        if (targetSectionId === "favoritesSection") {
          displayFavorites();
        } else if (targetSectionId === "profileSection") {
          // تشغيل التطبيقات في صفحة التطبيقات
          setTimeout(() => {
            displayApps();
            updatePagination();
          }, 100);
        } else if (targetSectionId === "categorySection") {
          // إذا كان هناك قسم محدد، قم بتحديث البيانات
          if (currentCategoryType) {
            displayCategoryApps();
            updateCategoryPagination();
          }
        }
      }

      // دالة إنشاء كارت التطبيق
      function createAppCard(app, index) {
        return `
                  <div class="app-card bg-white dark:bg-dark-card rounded-xl shadow-md p-5 cursor-pointer border border-gray-200 dark:border-gray-700 aspect-square flex flex-col" onclick="openAppModal(${index})">
                      <img src="${app.image}" alt="${app.name}" class="w-full flex-1 object-cover rounded-lg mb-3">
                      <h3 class="text-center text-gray-900 dark:text-white font-medium text-sm">${app.name}</h3>
                  </div>
              `;
      }

      // دالة إنشاء كارت التطبيق للفئة المميزة
      function createCategoryAppCard(app, index) {
        return `
                  <div class="app-card bg-white dark:bg-dark-card rounded-xl shadow-md p-5 cursor-pointer border border-gray-200 dark:border-gray-700 aspect-square flex flex-col" onclick="openCategoryAppModal(${index})">
                      <img src="${app.image}" alt="${app.name}" class="w-full flex-1 object-cover rounded-lg mb-3">
                      <h3 class="text-center text-gray-900 dark:text-white font-medium text-sm">${app.name}</h3>
                  </div>
              `;
      }

      // دالة إنشاء كارت التطبيق المفضل
      function createFavoriteCard(app) {
        const t = translations[appSettings.language];
        return `
                  <div class="app-card bg-white dark:bg-dark-card rounded-xl shadow-md p-4 border border-gray-200 dark:border-gray-700">
                      <img src="${app.image}" alt="${app.name}" class="w-full h-24 object-cover rounded-lg mb-3">
                      <h3 class="text-center text-gray-900 dark:text-white font-medium text-sm mb-2">${app.name}</h3>
                      <button onclick="removeFromFavorites(${app.id})" class="w-full bg-red-500 text-white py-2 px-4 rounded-lg text-xs hover:bg-red-600 transition-colors">
                          ${t.removeFavorite}
                      </button>
                  </div>
              `;
      }

      // دالة إنشاء النجوم
      function createStars(rating) {
        const stars = [];
        const fullStars = Math.floor(rating);
        const hasHalfStar = rating % 1 !== 0;

        for (let i = 0; i < 5; i++) {
          if (i < fullStars) {
            stars.push('<span class="text-yellow-400">★</span>');
          } else if (i === fullStars && hasHalfStar) {
            stars.push('<span class="text-yellow-400">☆</span>');
          } else {
            stars.push(
              '<span class="text-gray-300 dark:text-gray-600">☆</span>'
            );
          }
        }
        return stars.join("");
      }

      // دالة إنشاء لقطات الشاشة
      function createScreenshots(screenshots) {
        const t = translations[appSettings.language];
        if (!screenshots || screenshots.length === 0) {
          return `<p class="text-gray-500 dark:text-gray-400 text-sm">لا توجد لقطات شاشة متاحة</p>`;
        }

        return screenshots
          .map(
            (screenshot, index) => `
                  <div class="flex-shrink-0">
                      <img src="${screenshot}" 
                           alt="لقطة شاشة ${index + 1}" 
                           class="w-20 h-32 object-cover rounded-lg border border-gray-200 dark:border-gray-700 cursor-pointer hover:shadow-lg transition-shadow"
                           onclick="showFullScreenshot('${screenshot}')">
                  </div>
              `
          )
          .join("");
      }

      // دالة عرض لقطة الشاشة بالحجم الكامل
      function showFullScreenshot(imageUrl) {
        const fullscreenModal = document.createElement("div");
        fullscreenModal.className =
          "fixed inset-0 z-[60] bg-black bg-opacity-90 flex items-center justify-center p-4";
        fullscreenModal.innerHTML = `
                  <div class="relative max-w-sm max-h-full">
                      <img src="${imageUrl}" alt="لقطة شاشة" class="max-w-full max-h-full object-contain rounded-lg">
                      <button class="absolute top-4 right-4 text-white bg-black bg-opacity-50 rounded-full p-2 hover:bg-opacity-70 transition-colors" onclick="this.closest('.fixed').remove()">
                          <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12"></path>
                          </svg>
                      </button>
                  </div>
              `;

        // إغلاق عند النقر خارج الصورة
        fullscreenModal.addEventListener("click", (e) => {
          if (e.target === fullscreenModal) {
            fullscreenModal.remove();
          }
        });

        document.body.appendChild(fullscreenModal);
      }

      // دالة فتح النافذة المنبثقة بمعرف التطبيق (للـ carousel)
      function openAppModalById(appId) {
        const app = apps.find((a) => a.id === appId);
        if (!app) return;

        currentAppIndex = -1; // تعيين خاص للـ carousel

        // المعلومات الأساسية
        document.getElementById("modalAppName").textContent = app.name;
        document.getElementById("modalCategory").textContent = app.categoryName;
        document.getElementById("modalDescription").textContent =
          app.description;
        document.getElementById("modalImage").src = app.image;
        document.getElementById("modalImage").alt = app.name;

        // التقييم والنجوم
        if (app.rating) {
          document.getElementById("modalRating").innerHTML = createStars(
            app.rating
          );
          document.getElementById(
            "modalRatingText"
          ).textContent = `(${app.rating}/5.0)`;
          document.getElementById("modalRatingDisplay").textContent =
            app.rating;
        } else {
          document.getElementById("modalRating").innerHTML = createStars(0);
          document.getElementById("modalRatingText").textContent = "(غير مقيم)";
          document.getElementById("modalRatingDisplay").textContent = "N/A";
        }

        // الإحصائيات
        document.getElementById("modalDownloads").textContent =
          app.downloads || "غير متوفر";

        // المعلومات التفصيلية
        document.getElementById("modalDeveloper").textContent =
          app.developer || "غير محدد";
        document.getElementById("modalVersion").textContent = app.version;
        document.getElementById("modalSize").textContent = app.size;
        document.getElementById("modalLastUpdate").textContent =
          app.lastUpdate || "غير محدد";
        document.getElementById("modalLanguage").textContent =
          app.language || "غير محدد";
        document.getElementById("modalRequirements").textContent =
          app.requirements || "غير محدد";

        // لقطات الشاشة
        document.getElementById("modalScreenshots").innerHTML =
          createScreenshots(app.screenshots);

        // تحديث زر المفضلة
        updateFavoriteButton(app.id);

        document.getElementById("appModal").classList.remove("hidden");
        document.body.style.overflow = "hidden";
      }

      // دالة فتح النافذة المنبثقة من صفحة الأقسام المميزة
      function openCategoryAppModal(appIndex) {
        const app = filteredCategoryApps[appIndex];
        currentAppIndex = -1; // نفس منطق carousel

        // المعلومات الأساسية
        document.getElementById("modalAppName").textContent = app.name;
        document.getElementById("modalCategory").textContent = app.categoryName;
        document.getElementById("modalDescription").textContent =
          app.description;
        document.getElementById("modalImage").src = app.image;
        document.getElementById("modalImage").alt = app.name;

        // التقييم والنجوم
        if (app.rating) {
          document.getElementById("modalRating").innerHTML = createStars(
            app.rating
          );
          document.getElementById(
            "modalRatingText"
          ).textContent = `(${app.rating}/5.0)`;
          document.getElementById("modalRatingDisplay").textContent =
            app.rating;
        } else {
          document.getElementById("modalRating").innerHTML = createStars(0);
          document.getElementById("modalRatingText").textContent = "(غير مقيم)";
          document.getElementById("modalRatingDisplay").textContent = "N/A";
        }

        // الإحصائيات
        document.getElementById("modalDownloads").textContent =
          app.downloads || "غير متوفر";

        // المعلومات التفصيلية
        document.getElementById("modalDeveloper").textContent =
          app.developer || "غير محدد";
        document.getElementById("modalVersion").textContent = app.version;
        document.getElementById("modalSize").textContent = app.size;
        document.getElementById("modalLastUpdate").textContent =
          app.lastUpdate || "غير محدد";
        document.getElementById("modalLanguage").textContent =
          app.language || "غير محدد";
        document.getElementById("modalRequirements").textContent =
          app.requirements || "غير محدد";

        // لقطات الشاشة
        document.getElementById("modalScreenshots").innerHTML =
          createScreenshots(app.screenshots);

        // تحديث زر المفضلة
        updateFavoriteButton(app.id);

        document.getElementById("appModal").classList.remove("hidden");
        document.body.style.overflow = "hidden";
      }

      // دالة فتح النافذة المنبثقة
      function openAppModal(appIndex) {
        const app = filteredApps[appIndex];
        currentAppIndex = appIndex;

        // المعلومات الأساسية
        document.getElementById("modalAppName").textContent = app.name;
        document.getElementById("modalCategory").textContent = app.categoryName;
        document.getElementById("modalDescription").textContent =
          app.description;
        document.getElementById("modalImage").src = app.image;
        document.getElementById("modalImage").alt = app.name;

        // التقييم والنجوم
        if (app.rating) {
          document.getElementById("modalRating").innerHTML = createStars(
            app.rating
          );
          document.getElementById(
            "modalRatingText"
          ).textContent = `(${app.rating}/5.0)`;
          document.getElementById("modalRatingDisplay").textContent =
            app.rating;
        } else {
          document.getElementById("modalRating").innerHTML = createStars(0);
          document.getElementById("modalRatingText").textContent = "(غير مقيم)";
          document.getElementById("modalRatingDisplay").textContent = "N/A";
        }

        // الإحصائيات
        document.getElementById("modalDownloads").textContent =
          app.downloads || "غير متوفر";

        // المعلومات التفصيلية
        document.getElementById("modalDeveloper").textContent =
          app.developer || "غير محدد";
        document.getElementById("modalVersion").textContent = app.version;
        document.getElementById("modalSize").textContent = app.size;
        document.getElementById("modalLastUpdate").textContent =
          app.lastUpdate || "غير محدد";
        document.getElementById("modalLanguage").textContent =
          app.language || "غير محدد";
        document.getElementById("modalRequirements").textContent =
          app.requirements || "غير محدد";

        // لقطات الشاشة
        document.getElementById("modalScreenshots").innerHTML =
          createScreenshots(app.screenshots);

        // تحديث زر المفضلة
        updateFavoriteButton(app.id);

        document.getElementById("appModal").classList.remove("hidden");
        document.body.style.overflow = "hidden";
      }

      // دالة إغلاق النافذة المنبثقة
      function closeAppModal() {
        document.getElementById("appModal").classList.add("hidden");
        document.body.style.overflow = "auto";
      }

      // دالة تحديث زر المفضلة
      function updateFavoriteButton(appId) {
        const favoriteBtn = document.getElementById("favoriteBtn");
        const isFavorite = favoriteApps.includes(appId);
        const t = translations[appSettings.language];

        if (isFavorite) {
          favoriteBtn.innerHTML = `
                      <svg class="w-4 h-4" fill="currentColor" stroke="currentColor" viewBox="0 0 24 24">
                          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4.318 6.318a4.5 4.5 0 000 6.364L12 20.364l7.682-7.682a4.5 4.5 0 00-6.364-6.364L12 7.636l-1.318-1.318a4.5 4.5 0 00-6.364 0z"></path>
                      </svg>
                      <span>${t.addFavorite}</span>
                  `;
          favoriteBtn.classList.add("bg-red-500", "text-white");
          favoriteBtn.classList.remove(
            "border-gray-300",
            "dark:border-gray-600",
            "text-gray-700",
            "dark:text-gray-300"
          );
        } else {
          favoriteBtn.innerHTML = `
                      <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4.318 6.318a4.5 4.5 0 000 6.364L12 20.364l7.682-7.682a4.5 4.5 0 00-6.364-6.364L12 7.636l-1.318-1.318a4.5 4.5 0 00-6.364 0z"></path>
                      </svg>
                      <span>${t.addFavorite}</span>
                  `;
          favoriteBtn.classList.remove("bg-red-500", "text-white");
          favoriteBtn.classList.add(
            "border-gray-300",
            "dark:border-gray-600",
            "text-gray-700",
            "dark:text-gray-300"
          );
        }
      }

      // دالة إضافة/إزالة من المفضلة (محدثة للتعامل مع الحالتين)
      function toggleFavorite() {
        let appId;

        if (currentAppIndex === -1) {
          // إذا كانت النافذة مفتوحة من carousel أو category، ابحث عن التطبيق بالاسم
          const appName = document.getElementById("modalAppName").textContent;
          const app = apps.find((a) => a.name === appName);
          if (!app) return;
          appId = app.id;
        } else {
          // إذا كانت النافذة مفتوحة من الشبكة العادية
          const app = filteredApps[currentAppIndex];
          if (!app) return;
          appId = app.id;
        }

        const isFavorite = favoriteApps.includes(appId);

        if (isFavorite) {
          favoriteApps = favoriteApps.filter((id) => id !== appId);
        } else {
          favoriteApps.push(appId);
        }

        updateFavoriteButton(appId);

        // إذا كنا في صفحة المفضلة، حدث العرض
        if (
          document
            .getElementById("favoritesSection")
            .classList.contains("active")
        ) {
          displayFavorites();
        }
      }

      // دالة إزالة من المفضلة
      function removeFromFavorites(appId) {
        favoriteApps = favoriteApps.filter((id) => id !== appId);
        displayFavorites();
      }

      // دالة عرض المفضلة
      function displayFavorites() {
        const favoritesGrid = document.getElementById("favoritesGrid");
        const emptyFavorites = document.getElementById("emptyFavorites");

        if (favoriteApps.length === 0) {
          favoritesGrid.style.display = "none";
          emptyFavorites.style.display = "block";
        } else {
          favoritesGrid.style.display = "grid";
          emptyFavorites.style.display = "none";

          const favoriteAppsData = apps.filter((app) =>
            favoriteApps.includes(app.id)
          );
          favoritesGrid.innerHTML = favoriteAppsData
            .map((app) => createFavoriteCard(app))
            .join("");
        }
      }

      // دالة إظهار مؤشر التحميل
      function showLoadingIndicator() {
        const loadingIndicator = document.getElementById("loadingIndicator");
        const appsGrid = document.getElementById("appsGrid");
        const noResultsMessage = document.getElementById("noResultsMessage");

        if (loadingIndicator) loadingIndicator.classList.remove("hidden");
        if (appsGrid) appsGrid.innerHTML = "";
        if (noResultsMessage) noResultsMessage.classList.add("hidden");
      }

      // دالة إخفاء مؤشر التحميل
      function hideLoadingIndicator() {
        const loadingIndicator = document.getElementById("loadingIndicator");
        if (loadingIndicator) loadingIndicator.classList.add("hidden");
      }

      // دالة إظهار مؤشر التحميل للفئة
      function showCategoryLoadingIndicator() {
        const loadingIndicator = document.getElementById(
          "categoryLoadingIndicator"
        );
        const appsGrid = document.getElementById("categoryAppsGrid");
        const noResultsMessage = document.getElementById(
          "categoryNoResultsMessage"
        );

        if (loadingIndicator) loadingIndicator.classList.remove("hidden");
        if (appsGrid) appsGrid.innerHTML = "";
        if (noResultsMessage) noResultsMessage.classList.add("hidden");
      }

      // دالة إخفاء مؤشر التحميل للفئة
      function hideCategoryLoadingIndicator() {
        const loadingIndicator = document.getElementById(
          "categoryLoadingIndicator"
        );
        if (loadingIndicator) loadingIndicator.classList.add("hidden");
      }

      // دالة الفلترة الشاملة (بحث + تصنيف) المحسنة
      function applyFilters() {
        // إظهار مؤشر التحميل
        showLoadingIndicator();

        // تأخير للمحاكاة (يمكن إزالة هذا في الإنتاج)
        setTimeout(() => {
          let result = [...apps];

          // فلترة حسب التصنيف
          if (activeCategory !== "all") {
            result = result.filter((app) => app.category === activeCategory);
          }

          // فلترة حسب البحث
          const searchTerm =
            document.getElementById("searchInput")?.value.trim() || "";
          if (searchTerm) {
            result = result.filter((app) => app.name.includes(searchTerm));
            isSearching = true;
          } else {
            isSearching = false;
          }

          filteredApps = result;
          totalAppsCount = result.length;
          currentPage = 1;

          // إخفاء مؤشر التحميل
          hideLoadingIndicator();

          displayApps();
          updatePagination();

          // إظهار أو إخفاء رسالة عدم وجود نتائج
          const noResultsMessage = document.getElementById("noResultsMessage");
          if (noResultsMessage) {
            if (filteredApps.length === 0) {
              noResultsMessage.classList.remove("hidden");
            } else {
              noResultsMessage.classList.add("hidden");
            }
          }
        }, 500); // محاكاة وقت التحميل
      }

      // دالة الفلترة للفئات المميزة
      function applyCategoryFilters() {
        showCategoryLoadingIndicator();

        setTimeout(() => {
          let result = getSortedApps(currentCategoryType, 100); // جلب أكثر من التطبيقات الافتراضية

          // فلترة حسب البحث
          const searchTerm =
            document.getElementById("categorySearchInput")?.value.trim() || "";
          if (searchTerm) {
            result = result.filter((app) => app.name.includes(searchTerm));
            isCategorySearching = true;
          } else {
            isCategorySearching = false;
          }

          filteredCategoryApps = result;
          currentCategoryPage = 1;

          hideCategoryLoadingIndicator();

          displayCategoryApps();
          updateCategoryPagination();

          // إظهار أو إخفاء رسالة عدم وجود نتائج
          const noResultsMessage = document.getElementById(
            "categoryNoResultsMessage"
          );
          if (noResultsMessage) {
            if (filteredCategoryApps.length === 0) {
              noResultsMessage.classList.remove("hidden");
            } else {
              noResultsMessage.classList.add("hidden");
            }
          }
        }, 500);
      }

      // دالة البحث (محدثة لتتكامل مع الفلترة)
      function searchApps(searchTerm) {
        applyFilters();
      }

      // دالة تبديل وظيفة البحث
      function toggleSearch() {
        const searchInput = document.getElementById("searchInput");

        // إذا كنا في صفحة التطبيقات
        if (
          document.getElementById("profileSection").classList.contains("active")
        ) {
          // التركيز على مربع البحث والتمرير إليه
          if (searchInput) {
            searchInput.focus();
            searchInput.scrollIntoView({ behavior: "smooth", block: "center" });
          }
        } else {
          // التنقل إلى صفحة التطبيقات أولاً
          navigateToSection("profileSection");
          // ثم التركيز على مربع البحث بعد تحديث الصفحة
          setTimeout(() => {
            if (searchInput) {
              searchInput.focus();
              searchInput.scrollIntoView({
                behavior: "smooth",
                block: "center",
              });
            }
          }, 100);
        }
      }

      // دالة فلترة حسب التصنيف
      function filterByCategory(category) {
        activeCategory = category;

        // تحديث شكل الأزرار
        document.querySelectorAll(".category-btn").forEach((btn) => {
          btn.classList.remove("active");
        });
        document
          .querySelector(`[data-category="${category}"]`)
          ?.classList.add("active");

        applyFilters();
      }

      // دالة عرض التطبيقات للصفحة الحالية
      function displayApps() {
        const totalPages = Math.ceil(filteredApps.length / appsPerPage);
        const startIndex = (currentPage - 1) * appsPerPage;
        const endIndex = startIndex + appsPerPage;
        const currentApps = filteredApps.slice(startIndex, endIndex);

        const appsGrid = document.getElementById("appsGrid");
        if (appsGrid) {
          appsGrid.innerHTML = currentApps
            .map((app, localIndex) =>
              createAppCard(app, startIndex + localIndex)
            )
            .join("");
        }
      }

      // دالة عرض التطبيقات للفئة المميزة
      function displayCategoryApps() {
        const totalPages = Math.ceil(filteredCategoryApps.length / appsPerPage);
        const startIndex = (currentCategoryPage - 1) * appsPerPage;
        const endIndex = startIndex + appsPerPage;
        const currentApps = filteredCategoryApps.slice(startIndex, endIndex);

        const appsGrid = document.getElementById("categoryAppsGrid");
        if (appsGrid) {
          appsGrid.innerHTML = currentApps
            .map((app, localIndex) =>
              createCategoryAppCard(app, startIndex + localIndex)
            )
            .join("");
        }
      }

      // دالة تحديث معلومات الصفحة
      function updatePageInfo() {
        const t = translations[appSettings.language];
        const totalPages = Math.ceil(filteredApps.length / appsPerPage);

        // تحديث معلومات الصفحة
        const pageInfoElement = document.getElementById("pageInfo");
        const totalAppsInfoElement = document.getElementById("totalAppsInfo");

        if (pageInfoElement) {
          pageInfoElement.textContent = t.pageOf
            .replace("{page}", currentPage)
            .replace("{total}", totalPages || 1);
        }

        if (totalAppsInfoElement) {
          totalAppsInfoElement.textContent = t.totalApps.replace(
            "{total}",
            filteredApps.length
          );
        }
      }

      // دالة تحديث معلومات الصفحة للفئة
      function updateCategoryPageInfo() {
        const t = translations[appSettings.language];
        const totalPages = Math.ceil(filteredCategoryApps.length / appsPerPage);

        // تحديث معلومات الصفحة
        const pageInfoElement = document.getElementById("categoryPageInfo");
        const totalAppsInfoElement = document.getElementById(
          "categoryTotalAppsInfo"
        );

        if (pageInfoElement) {
          pageInfoElement.textContent = t.pageOf
            .replace("{page}", currentCategoryPage)
            .replace("{total}", totalPages || 1);
        }

        if (totalAppsInfoElement) {
          totalAppsInfoElement.textContent = t.totalApps.replace(
            "{total}",
            filteredCategoryApps.length
          );
        }
      }

      // دالة إنشاء أرقام الصفحات المحسنة
      function createPageNumbers() {
        const totalPages = Math.ceil(filteredApps.length / appsPerPage);
        const pageNumbers = document.getElementById("pageNumbers");
        if (!pageNumbers) return;

        pageNumbers.innerHTML = "";

        let startPage = 1;
        let endPage = totalPages;

        // إذا كان هناك أكثر من 5 صفحات، أظهر نطاق محدود
        if (totalPages > 5) {
          if (currentPage <= 3) {
            startPage = 1;
            endPage = 5;
          } else if (currentPage >= totalPages - 2) {
            startPage = totalPages - 4;
            endPage = totalPages;
          } else {
            startPage = currentPage - 2;
            endPage = currentPage + 2;
          }
        }

        // إضافة نقاط في البداية إذا لزم الأمر
        if (startPage > 1) {
          const firstPageButton = document.createElement("button");
          firstPageButton.textContent = "1";
          firstPageButton.className =
            "page-btn px-3 py-2 rounded-lg text-sm font-medium transition-all hover:bg-gray-100 dark:hover:bg-gray-700 text-gray-700 dark:text-gray-300";
          firstPageButton.addEventListener("click", () => goToPage(1));
          pageNumbers.appendChild(firstPageButton);

          if (startPage > 2) {
            const ellipsis = document.createElement("span");
            ellipsis.textContent = "...";
            ellipsis.className = "px-2 py-2 text-gray-500 dark:text-gray-400";
            pageNumbers.appendChild(ellipsis);
          }
        }

        // إضافة أزرار الصفحات في النطاق المحدد
        for (let i = startPage; i <= endPage; i++) {
          const pageButton = document.createElement("button");
          pageButton.textContent = i;
          pageButton.className = `page-btn px-3 py-2 rounded-lg text-sm font-medium transition-all ${
            i === currentPage
              ? "active bg-primary text-white shadow-lg"
              : "hover:bg-gray-100 dark:hover:bg-gray-700 text-gray-700 dark:text-gray-300"
          }`;
          pageButton.addEventListener("click", () => goToPage(i));
          pageNumbers.appendChild(pageButton);
        }

        // إضافة نقاط في النهاية إذا لزم الأمر
        if (endPage < totalPages) {
          if (endPage < totalPages - 1) {
            const ellipsis = document.createElement("span");
            ellipsis.textContent = "...";
            ellipsis.className = "px-2 py-2 text-gray-500 dark:text-gray-400";
            pageNumbers.appendChild(ellipsis);
          }

          const lastPageButton = document.createElement("button");
          lastPageButton.textContent = totalPages;
          lastPageButton.className =
            "page-btn px-3 py-2 rounded-lg text-sm font-medium transition-all hover:bg-gray-100 dark:hover:bg-gray-700 text-gray-700 dark:text-gray-300";
          lastPageButton.addEventListener("click", () => goToPage(totalPages));
          pageNumbers.appendChild(lastPageButton);
        }
      }

      // دالة إنشاء أرقام الصفحات للفئة
      function createCategoryPageNumbers() {
        const totalPages = Math.ceil(filteredCategoryApps.length / appsPerPage);
        const pageNumbers = document.getElementById("categoryPageNumbers");
        if (!pageNumbers) return;

        pageNumbers.innerHTML = "";

        let startPage = 1;
        let endPage = totalPages;

        // إذا كان هناك أكثر من 5 صفحات، أظهر نطاق محدود
        if (totalPages > 5) {
          if (currentCategoryPage <= 3) {
            startPage = 1;
            endPage = 5;
          } else if (currentCategoryPage >= totalPages - 2) {
            startPage = totalPages - 4;
            endPage = totalPages;
          } else {
            startPage = currentCategoryPage - 2;
            endPage = currentCategoryPage + 2;
          }
        }

        // إضافة نقاط في البداية إذا لزم الأمر
        if (startPage > 1) {
          const firstPageButton = document.createElement("button");
          firstPageButton.textContent = "1";
          firstPageButton.className =
            "page-btn px-3 py-2 rounded-lg text-sm font-medium transition-all hover:bg-gray-100 dark:hover:bg-gray-700 text-gray-700 dark:text-gray-300";
          firstPageButton.addEventListener("click", () => goToCategoryPage(1));
          pageNumbers.appendChild(firstPageButton);

          if (startPage > 2) {
            const ellipsis = document.createElement("span");
            ellipsis.textContent = "...";
            ellipsis.className = "px-2 py-2 text-gray-500 dark:text-gray-400";
            pageNumbers.appendChild(ellipsis);
          }
        }

        // إضافة أزرار الصفحات في النطاق المحدد
        for (let i = startPage; i <= endPage; i++) {
          const pageButton = document.createElement("button");
          pageButton.textContent = i;
          pageButton.className = `page-btn px-3 py-2 rounded-lg text-sm font-medium transition-all ${
            i === currentCategoryPage
              ? "active bg-primary text-white shadow-lg"
              : "hover:bg-gray-100 dark:hover:bg-gray-700 text-gray-700 dark:text-gray-300"
          }`;
          pageButton.addEventListener("click", () => goToCategoryPage(i));
          pageNumbers.appendChild(pageButton);
        }

        // إضافة نقاط في النهاية إذا لزم الأمر
        if (endPage < totalPages) {
          if (endPage < totalPages - 1) {
            const ellipsis = document.createElement("span");
            ellipsis.textContent = "...";
            ellipsis.className = "px-2 py-2 text-gray-500 dark:text-gray-400";
            pageNumbers.appendChild(ellipsis);
          }

          const lastPageButton = document.createElement("button");
          lastPageButton.textContent = totalPages;
          lastPageButton.className =
            "page-btn px-3 py-2 rounded-lg text-sm font-medium transition-all hover:bg-gray-100 dark:hover:bg-gray-700 text-gray-700 dark:text-gray-300";
          lastPageButton.addEventListener("click", () =>
            goToCategoryPage(totalPages)
          );
          pageNumbers.appendChild(lastPageButton);
        }
      }

      // دالة الانتقال إلى صفحة معينة
      function goToPage(page) {
        const totalPages = Math.ceil(filteredApps.length / appsPerPage);
        if (page >= 1 && page <= totalPages) {
          currentPage = page;

          // إظهار مؤشر التحميل أثناء التنقل
          showLoadingIndicator();

          setTimeout(() => {
            displayApps();
            updatePagination();
            hideLoadingIndicator();

            // التمرير إلى أعلى الصفحة
            document.getElementById("profileSection").scrollIntoView({
              behavior: "smooth",
              block: "start",
            });
          }, 300);
        }
      }

      // دالة الانتقال إلى صفحة معينة في الفئة
      function goToCategoryPage(page) {
        const totalPages = Math.ceil(filteredCategoryApps.length / appsPerPage);
        if (page >= 1 && page <= totalPages) {
          currentCategoryPage = page;

          showCategoryLoadingIndicator();

          setTimeout(() => {
            displayCategoryApps();
            updateCategoryPagination();
            hideCategoryLoadingIndicator();

            document.getElementById("categorySection").scrollIntoView({
              behavior: "smooth",
              block: "start",
            });
          }, 300);
        }
      }

      // دالة الانتقال السريع لصفحة
      function jumpToPage() {
        const pageInput = document.getElementById("pageJumpInput");
        const targetPage = parseInt(pageInput.value);
        const totalPages = Math.ceil(filteredApps.length / appsPerPage);

        if (targetPage >= 1 && targetPage <= totalPages) {
          goToPage(targetPage);
          pageInput.value = "";
        } else {
          // إظهار رسالة خطأ
          const t = translations[appSettings.language];
          showNotification(
            `${t.error || "خطأ"}: ${
              t.invalidPage || "رقم صفحة غير صالح"
            } (1-${totalPages})`
          );
        }
      }

      // دالة الانتقال السريع لصفحة في الفئة
      function jumpToCategoryPage() {
        const pageInput = document.getElementById("categoryPageJumpInput");
        const targetPage = parseInt(pageInput.value);
        const totalPages = Math.ceil(filteredCategoryApps.length / appsPerPage);

        if (targetPage >= 1 && targetPage <= totalPages) {
          goToCategoryPage(targetPage);
          pageInput.value = "";
        } else {
          const t = translations[appSettings.language];
          showNotification(
            `${t.error || "خطأ"}: ${
              t.invalidPage || "رقم صفحة غير صالح"
            } (1-${totalPages})`
          );
        }
      }

      // دالة تحديث أزرار التنقل المحسنة
      function updatePagination() {
        const totalPages = Math.ceil(filteredApps.length / appsPerPage);
        const paginationContainer = document.getElementById(
          "paginationContainer"
        );

        if (!paginationContainer) return;

        // إخفاء التنقل إذا لم تكن هناك صفحات متعددة
        if (totalPages <= 1) {
          paginationContainer.classList.add("hidden");
          return;
        } else {
          paginationContainer.classList.remove("hidden");
        }

        // تحديث معلومات الصفحة
        updatePageInfo();

        // تحديث أرقام الصفحات
        createPageNumbers();

        // تحديث أزرار التنقل
        const firstPageBtn = document.getElementById("firstPageBtn");
        const prevBtn = document.getElementById("prevBtn");
        const nextBtn = document.getElementById("nextBtn");
        const lastPageBtn = document.getElementById("lastPageBtn");
        const pageJumpInput = document.getElementById("pageJumpInput");

        // تحديث حالة الأزرار
        if (firstPageBtn && prevBtn && nextBtn && lastPageBtn) {
          firstPageBtn.disabled = currentPage === 1;
          prevBtn.disabled = currentPage === 1;
          nextBtn.disabled = currentPage === totalPages;
          lastPageBtn.disabled = currentPage === totalPages;

          // تحديث الكلاسات للأزرار المعطلة
          [firstPageBtn, prevBtn].forEach((btn) => {
            if (currentPage === 1) {
              btn.classList.add("opacity-50", "cursor-not-allowed");
              btn.classList.remove(
                "hover:text-primary",
                "hover:border-primary"
              );
            } else {
              btn.classList.remove("opacity-50", "cursor-not-allowed");
              btn.classList.add("hover:text-primary", "hover:border-primary");
            }
          });

          [nextBtn, lastPageBtn].forEach((btn) => {
            if (currentPage === totalPages) {
              btn.classList.add("opacity-50", "cursor-not-allowed");
              btn.classList.remove(
                "hover:text-primary",
                "hover:border-primary"
              );
            } else {
              btn.classList.remove("opacity-50", "cursor-not-allowed");
              btn.classList.add("hover:text-primary", "hover:border-primary");
            }
          });
        }

        // تحديث مدخل الانتقال السريع
        if (pageJumpInput) {
          pageJumpInput.max = totalPages;
          pageJumpInput.placeholder = `1-${totalPages}`;
        }
      }

      // دالة تحديث التنقل للفئة
      function updateCategoryPagination() {
        const totalPages = Math.ceil(filteredCategoryApps.length / appsPerPage);
        const paginationContainer = document.getElementById(
          "categoryPaginationContainer"
        );

        if (!paginationContainer) return;

        if (totalPages <= 1) {
          paginationContainer.classList.add("hidden");
          return;
        } else {
          paginationContainer.classList.remove("hidden");
        }

        updateCategoryPageInfo();
        createCategoryPageNumbers();

        const firstPageBtn = document.getElementById("categoryFirstPageBtn");
        const prevBtn = document.getElementById("categoryPrevBtn");
        const nextBtn = document.getElementById("categoryNextBtn");
        const lastPageBtn = document.getElementById("categoryLastPageBtn");
        const pageJumpInput = document.getElementById("categoryPageJumpInput");

        if (firstPageBtn && prevBtn && nextBtn && lastPageBtn) {
          firstPageBtn.disabled = currentCategoryPage === 1;
          prevBtn.disabled = currentCategoryPage === 1;
          nextBtn.disabled = currentCategoryPage === totalPages;
          lastPageBtn.disabled = currentCategoryPage === totalPages;

          [firstPageBtn, prevBtn].forEach((btn) => {
            if (currentCategoryPage === 1) {
              btn.classList.add("opacity-50", "cursor-not-allowed");
              btn.classList.remove(
                "hover:text-primary",
                "hover:border-primary"
              );
            } else {
              btn.classList.remove("opacity-50", "cursor-not-allowed");
              btn.classList.add("hover:text-primary", "hover:border-primary");
            }
          });

          [nextBtn, lastPageBtn].forEach((btn) => {
            if (currentCategoryPage === totalPages) {
              btn.classList.add("opacity-50", "cursor-not-allowed");
              btn.classList.remove(
                "hover:text-primary",
                "hover:border-primary"
              );
            } else {
              btn.classList.remove("opacity-50", "cursor-not-allowed");
              btn.classList.add("hover:text-primary", "hover:border-primary");
            }
          });
        }

        if (pageJumpInput) {
          pageJumpInput.max = totalPages;
          pageJumpInput.placeholder = `1-${totalPages}`;
        }
      }

      // دالة إنشاء كارت التطبيق carousel (محدثة للعمل مع الـ ID)
      function createCarouselAppCard(app, badge = null) {
        return `
                  <div class="carousel-app-card bg-white dark:bg-dark-card rounded-xl shadow-md p-4 cursor-pointer border border-gray-200 dark:border-gray-700 relative" onclick="openAppModalById(${
                    app.id
                  })">
                      ${
                        badge
                          ? `<div class="carousel-app-badge">${badge}</div>`
                          : ""
                      }
                      <img src="${app.image}" alt="${
          app.name
        }" class="carousel-app-image mb-3">
                      <h3 class="text-center text-gray-900 dark:text-white font-medium text-sm mb-1">${
                        app.name
                      }</h3>
                      <div class="flex items-center justify-center space-x-1 space-x-reverse mb-1">
                          ${createStars(app.rating)}
                      </div>
                      <p class="text-xs text-gray-500 dark:text-gray-400 text-center">${
                        app.downloads
                      }</p>
                  </div>
              `;
      }

      // دالة تمرير carousel
      function scrollCarousel(carouselId, scrollAmount) {
        const carousel = document.getElementById(carouselId);
        if (carousel) {
          carousel.scrollBy({
            left: scrollAmount,
            behavior: "smooth",
          });
        }
      }

      // دالة ترتيب التطبيقات حسب معايير مختلفة
      function getSortedApps(criteria, limit = 6) {
        let sortedApps = [...apps];

        switch (criteria) {
          case "most-used":
            // ترتيب حسب عدد التحميلات
            sortedApps.sort((a, b) => {
              const aDownloads = parseFloat(a.downloads.replace(/[^\d.]/g, ""));
              const bDownloads = parseFloat(b.downloads.replace(/[^\d.]/g, ""));
              return bDownloads - aDownloads;
            });
            break;

          case "top-rated":
            // ترتيب حسب التقييم
            sortedApps.sort((a, b) => (b.rating || 0) - (a.rating || 0));
            break;

          case "newest":
            // ترتيب حسب تاريخ آخر تحديث
            sortedApps.sort((a, b) => {
              const aDate = new Date(a.lastUpdate || "2020/01/01");
              const bDate = new Date(b.lastUpdate || "2020/01/01");
              return bDate - aDate;
            });
            break;

          case "featured-games":
            // فلترة الألعاب وترتيب حسب التقييم
            sortedApps = sortedApps.filter(
              (app) => app.category === "entertainment"
            );
            sortedApps.sort((a, b) => (b.rating || 0) - (a.rating || 0));
            break;
        }

        return sortedApps.slice(0, limit);
      }

      // دالة تحديث carousel الأقسام
      function updateCarouselSections() {
        // الأكثر استعمالاً
        const mostUsedApps = getSortedApps("most-used");
        const mostUsedCarousel = document.getElementById("mostUsedCarousel");
        if (mostUsedCarousel) {
          mostUsedCarousel.querySelector(".flex").innerHTML = mostUsedApps
            .map((app) => createCarouselAppCard(app, "🔥"))
            .join("");
        }

        // الأعلى تقييماً
        const topRatedApps = getSortedApps("top-rated");
        const topRatedCarousel = document.getElementById("topRatedCarousel");
        if (topRatedCarousel) {
          topRatedCarousel.querySelector(".flex").innerHTML = topRatedApps
            .map((app) => createCarouselAppCard(app, "⭐"))
            .join("");
        }

        // الأحدث
        const newestApps = getSortedApps("newest");
        const newestCarousel = document.getElementById("newestCarousel");
        if (newestCarousel) {
          newestCarousel.querySelector(".flex").innerHTML = newestApps
            .map((app) => createCarouselAppCard(app, "🆕"))
            .join("");
        }

        // الألعاب المميزة
        const featuredGames = getSortedApps("featured-games");
        const featuredGamesCarousel = document.getElementById(
          "featuredGamesCarousel"
        );
        if (featuredGamesCarousel) {
          featuredGamesCarousel.querySelector(".flex").innerHTML = featuredGames
            .map((app) => createCarouselAppCard(app, "🎮"))
            .join("");
        }
      }

      // دالة عرض جميع التطبيقات في فئة معينة (محدثة للصفحة الجديدة)
      function showAllInCategory(category) {
        const t = translations[appSettings.language];

        // تحديد نوع الفئة
        currentCategoryType = category;

        // تحديث عنوان وصفحة الفئة
        let categoryTitle = "";
        let categorySubtitle = "";

        switch (category) {
          case "most-used":
            categoryTitle = t.mostUsed;
            categorySubtitle = t.categoryMostUsedDesc;
            break;
          case "top-rated":
            categoryTitle = t.topRated;
            categorySubtitle = t.categoryTopRatedDesc;
            break;
          case "newest":
            categoryTitle = t.newest;
            categorySubtitle = t.categoryNewestDesc;
            break;
          case "featured-games":
            categoryTitle = t.featuredGames;
            categorySubtitle = t.categoryFeaturedGamesDesc;
            break;
        }

        // تحديث العناوين
        document.getElementById("categoryTitle").textContent = categoryTitle;
        document.getElementById("categorySubtitle").textContent =
          categorySubtitle;

        // إعداد البيانات المفلترة
        filteredCategoryApps = getSortedApps(category, 100);
        currentCategoryPage = 1;

        // التنقل لصفحة الأقسام المميزة
        navigateToSection("categorySection");

        // تحديث العرض
        setTimeout(() => {
          displayCategoryApps();
          updateCategoryPagination();

          // مسح البحث
          const categorySearchInput = document.getElementById(
            "categorySearchInput"
          );
          if (categorySearchInput) {
            categorySearchInput.value = "";
          }

          document
            .getElementById("categorySection")
            .scrollIntoView({ behavior: "smooth" });
        }, 100);
      }

      // تشغيل التطبيق
      document.addEventListener("DOMContentLoaded", () => {
        loadDarkMode();
        loadCompactView(); // أضف هذا السطر
        // تهيئة الوضع المظلم
        initializeDarkMode();

        // تطبيق الترجمة الافتراضية
        applyLanguage(appSettings.language);

        // عرض التطبيقات في الصفحة الرئيسية (لا يوجد شبكة هناك الآن)
        filteredApps = [...apps]; // تهيئة أساسية
        totalAppsCount = apps.length;

        // تحديث أزرار التبديل الأولية مع Switches الجديدة
        updateToggleSwitchModern("darkModeToggle", appSettings.darkMode);
        updateToggleSwitchModern("animationsToggle", appSettings.animations);
        updateToggleSwitchModern("compactViewToggle", appSettings.compactView);
        // تطبيق العرض المضغوط المحفوظ
        applyCompactView(); // أضف هذا السطر

        // إعداد أزرار التصنيفات (في صفحة التطبيقات فقط)
        document
          .querySelectorAll("#categoryFilter .category-btn")
          .forEach((btn) => {
            btn.addEventListener("click", () => {
              const category = btn.getAttribute("data-category");
              filterByCategory(category);
            });
          });

        // إعداد شريط البحث في صفحة التطبيقات
        const searchInput = document.getElementById("searchInput");
        if (searchInput) {
          searchInput.addEventListener("input", (e) => {
            applyFilters();
          });
        }

        // إعداد شريط البحث في صفحة الأقسام المميزة
        const categorySearchInput = document.getElementById(
          "categorySearchInput"
        );
        if (categorySearchInput) {
          categorySearchInput.addEventListener("input", (e) => {
            applyCategoryFilters();
          });
        }

        // إعداد أزرار التنقل المحسنة
        const firstPageBtn = document.getElementById("firstPageBtn");
        const prevBtn = document.getElementById("prevBtn");
        const nextBtn = document.getElementById("nextBtn");
        const lastPageBtn = document.getElementById("lastPageBtn");
        const goToPageBtn = document.getElementById("goToPageBtn");
        const pageJumpInput = document.getElementById("pageJumpInput");

        if (firstPageBtn) {
          firstPageBtn.addEventListener("click", () => goToPage(1));
        }

        if (prevBtn) {
          prevBtn.addEventListener("click", () => {
            if (currentPage > 1) goToPage(currentPage - 1);
          });
        }

        if (nextBtn) {
          nextBtn.addEventListener("click", () => {
            const totalPages = Math.ceil(filteredApps.length / appsPerPage);
            if (currentPage < totalPages) goToPage(currentPage + 1);
          });
        }

        if (lastPageBtn) {
          lastPageBtn.addEventListener("click", () => {
            const totalPages = Math.ceil(filteredApps.length / appsPerPage);
            goToPage(totalPages);
          });
        }

        if (goToPageBtn) {
          goToPageBtn.addEventListener("click", jumpToPage);
        }

        if (pageJumpInput) {
          pageJumpInput.addEventListener("keypress", (e) => {
            if (e.key === "Enter") {
              jumpToPage();
            }
          });
        }

        // إعداد أزرار التنقل للفئة المميزة
        const categoryFirstPageBtn = document.getElementById(
          "categoryFirstPageBtn"
        );
        const categoryPrevBtn = document.getElementById("categoryPrevBtn");
        const categoryNextBtn = document.getElementById("categoryNextBtn");
        const categoryLastPageBtn = document.getElementById(
          "categoryLastPageBtn"
        );
        const categoryGoToPageBtn = document.getElementById(
          "categoryGoToPageBtn"
        );
        const categoryPageJumpInput = document.getElementById(
          "categoryPageJumpInput"
        );

        if (categoryFirstPageBtn) {
          categoryFirstPageBtn.addEventListener("click", () =>
            goToCategoryPage(1)
          );
        }

        if (categoryPrevBtn) {
          categoryPrevBtn.addEventListener("click", () => {
            if (currentCategoryPage > 1)
              goToCategoryPage(currentCategoryPage - 1);
          });
        }

        if (categoryNextBtn) {
          categoryNextBtn.addEventListener("click", () => {
            const totalPages = Math.ceil(
              filteredCategoryApps.length / appsPerPage
            );
            if (currentCategoryPage < totalPages)
              goToCategoryPage(currentCategoryPage + 1);
          });
        }

        if (categoryLastPageBtn) {
          categoryLastPageBtn.addEventListener("click", () => {
            const totalPages = Math.ceil(
              filteredCategoryApps.length / appsPerPage
            );
            goToCategoryPage(totalPages);
          });
        }

        if (categoryGoToPageBtn) {
          categoryGoToPageBtn.addEventListener("click", jumpToCategoryPage);
        }

        if (categoryPageJumpInput) {
          categoryPageJumpInput.addEventListener("keypress", (e) => {
            if (e.key === "Enter") {
              jumpToCategoryPage();
            }
          });
        }

        // إعداد النافذة المنبثقة
        document
          .getElementById("closeModal")
          .addEventListener("click", closeAppModal);

        // إعداد زر المفضلة
        document
          .getElementById("favoriteBtn")
          .addEventListener("click", toggleFavorite);

        // إغلاق النافذة المنبثقة عند النقر خارجها
        document.getElementById("appModal").addEventListener("click", (e) => {
          if (e.target === document.getElementById("appModal")) {
            closeAppModal();
          }
        });

        // إغلاق النافذة المنبثقة للإعدادات عند النقر خارجها
        document
          .getElementById("settingsModal")
          .addEventListener("click", (e) => {
            if (e.target === document.getElementById("settingsModal")) {
              closeSettingsModal();
            }
          });

        // إغلاق النافذة المنبثقة بالضغط على Escape
        document.addEventListener("keydown", (e) => {
          if (e.key === "Escape") {
            if (
              !document.getElementById("appModal").classList.contains("hidden")
            ) {
              closeAppModal();
            } else if (
              !document
                .getElementById("settingsModal")
                .classList.contains("hidden")
            ) {
              closeSettingsModal();
            } else if (
              document.getElementById("sideMenu").classList.contains("active")
            ) {
              closeSideMenu();
            }
          }
        });

        // إعداد شريط التنقل السفلي
        document.querySelectorAll(".nav-item").forEach((item) => {
          item.addEventListener("click", () => {
            const targetSection = item.getAttribute("data-section");
            switchSection(targetSection);
          });
        });

        // تحديث carousel الأقسام
        updateCarouselSections();

        // تحديث التطبيقات والصفحات في البداية
        updatePagination();
      });
    </script>
    <script>
      document.addEventListener("DOMContentLoaded", () => {
        const navItems = document.querySelectorAll(".bottom-nav .nav-item");

        navItems.forEach((item) => {
          item.addEventListener("click", () => {
            // إزالة اللون الأزرق من كل العناصر
            navItems.forEach((el) => el.classList.remove("active"));
            // إضافة اللون الأزرق للزر المضغوط
            item.classList.add("active");
          });
        });
      });
    </script>
    <script>
      // تحميل المفضلة عند فتح الصفحة
      function loadFavorites() {
        const saved = localStorage.getItem("favoriteApps");
        favoriteApps = saved ? JSON.parse(saved) : [];
      }

      // حفظ المفضلة بعد أي تعديل
      function saveFavorites() {
        localStorage.setItem("favoriteApps", JSON.stringify(favoriteApps));
      }

      // تبديل حالة المفضلة
      function toggleFavorite() {
        let appId;

        if (currentAppIndex === -1) {
          const appName = document.getElementById("modalAppName").textContent;
          const app = apps.find((a) => a.name === appName);
          if (!app) return;
          appId = app.id;
        } else {
          const app = filteredApps[currentAppIndex];
          if (!app) return;
          appId = app.id;
        }

        const isFavorite = favoriteApps.includes(appId);

        if (isFavorite) {
          favoriteApps = favoriteApps.filter((id) => id !== appId);
        } else {
          favoriteApps.push(appId);
        }

        saveFavorites(); // حفظ التغييرات
        updateFavoriteButton(appId);
        displayFavorites();
        updateCarouselSections(); // تحديث أي Carousel فيه أي badge
      }

      // إزالة من المفضلة
      function removeFromFavorites(appId) {
        favoriteApps = favoriteApps.filter((id) => id !== appId);
        saveFavorites();
        displayFavorites();
        updateCarouselSections();
      }

      // عرض المفضلة
      function displayFavorites() {
        const favoritesGrid = document.getElementById("favoritesGrid");
        const emptyFavorites = document.getElementById("emptyFavorites");

        if (favoriteApps.length === 0) {
          favoritesGrid.style.display = "none";
          emptyFavorites.style.display = "block";
        } else {
          favoritesGrid.style.display = "grid";
          emptyFavorites.style.display = "none";

          const favoriteAppsData = apps.filter((app) =>
            favoriteApps.includes(app.id)
          );
          favoritesGrid.innerHTML = favoriteAppsData
            .map((app) => createFavoriteCard(app))
            .join("");
        }
      }

      // تحديث زر المفضلة في المودال والكروت
      function updateFavoriteButton(appId) {
        const btn = document.getElementById("favoriteBtn");
        if (!btn) return;

        if (favoriteApps.includes(appId)) {
          btn.classList.add("active");
          btn.textContent = "حُبّ";
        } else {
          btn.classList.remove("active");
          btn.textContent = "أضف للمفضلة";
        }
      }

      // تشغيل عند تحميل الصفحة
      document.addEventListener("DOMContentLoaded", () => {
        loadFavorites();
        displayFavorites();
        updateCarouselSections();
      });
      function updateFavoriteButton(appId) {
        const btn = document.getElementById("favoriteBtn");
        if (!btn) return;

        if (favoriteApps.includes(appId)) {
          btn.classList.add("active"); // يظهر مضاف لكن النص يبقى كما هو
        } else {
          btn.classList.remove("active");
        }
      }
      function updateFavoriteButton(appId) {
        const btn = document.getElementById("favoriteBtn");
        if (!btn) return;

        // نشوفو واش التطبيق موجود في المفضلة
        if (favoriteApps.includes(appId)) {
          btn.classList.add("active"); // يظهر مفعل
        } else {
          btn.classList.remove("active"); // يبقى طبيعي
        }

        // تأكد أن الزر قابل للضغط
        btn.disabled = false;
      }
      function updateFavoriteButtons() {
        document.querySelectorAll(".favoriteBtn").forEach((btn) => {
          const appId = parseInt(btn.getAttribute("data-app-id"));
          if (favoriteApps.includes(appId)) {
            btn.classList.add("active"); // التطبيق في المفضلة
          } else {
            btn.classList.remove("active");
          }
        });
      }
      document.querySelectorAll(".favoriteBtn").forEach((btn) => {
        btn.addEventListener("click", () => {
          const appId = parseInt(btn.getAttribute("data-app-id"));
          if (favoriteApps.includes(appId)) {
            favoriteApps = favoriteApps.filter((id) => id !== appId);
          } else {
            favoriteApps.push(appId);
          }
          updateFavoriteButtons();
          displayFavorites(); // إذا كنت في صفحة المفضلة
        });
      });
    </script>
    <script>
      // دالة إنشاء أيقونة احترافية للتطبيق
      function createAppBadge(badgeType) {
        const badges = {
          fire: {
            bgColor: "bg-red-50 dark:bg-red-900/20",
            iconColor: "text-red-600 dark:text-red-400",
            svg: `<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17.657 18.657A8 8 0 016.343 7.343S7 9 9 10c0-2 .5-5 2.986-7C14 5 16.09 5.777 17.656 7.343A7.975 7.975 0 0120 13a7.975 7.975 0 01-2.343 5.657z"></path>`,
          },
          star: {
            bgColor: "bg-yellow-50 dark:bg-yellow-900/20",
            iconColor: "text-yellow-600 dark:text-yellow-400",
            svg: `<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M11.049 2.927c.3-.921 1.603-.921 1.902 0l1.519 4.674a1 1 0 00.95.69h4.915c.969 0 1.371 1.24.588 1.81l-3.976 2.888a1 1 0 00-.363 1.118l1.518 4.674c.3.922-.755 1.688-1.538 1.118l-3.976-2.888a1 1 0 00-1.176 0l-3.976 2.888c-.783.57-1.838-.197-1.538-1.118l1.518-4.674a1 1 0 00-.363-1.118l-3.976-2.888c-.784-.57-.38-1.81.588-1.81h4.914a1 1 0 00.951-.69l1.519-4.674z"></path>`,
          },
          new: {
            bgColor: "bg-emerald-50 dark:bg-emerald-900/20",
            iconColor: "text-emerald-600 dark:text-emerald-400",
            svg: `<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 10V3L4 14h7v7l9-11h-7z"></path>`,
          },
          game: {
            bgColor: "bg-purple-50 dark:bg-purple-900/20",
            iconColor: "text-purple-600 dark:text-purple-400",
            svg: `<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M11 4a2 2 0 114 0v1a1 1 0 001 1h3a1 1 0 011 1v3a1 1 0 01-1 1h-1a2 2 0 100 4h1a1 1 0 011 1v3a1 1 0 01-1 1h-3a1 1 0 01-1-1v-1a2 2 0 10-4 0v1a1 1 0 01-1 1H7a1 1 0 01-1-1v-3a1 1 0 011-1h1a2 2 0 100-4H7a1 1 0 01-1-1V7a1 1 0 011-1h3a1 1 0 001-1V4z"></path>`,
          },
        };

        const badge = badges[badgeType];
        if (!badge) return "";

        return `
          <div class="absolute top-2 right-2 w-8 h-8 rounded-full ${badge.bgColor} flex items-center justify-center shadow-md z-10">
              <svg class="w-4 h-4 ${badge.iconColor}" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                  ${badge.svg}
              </svg>
          </div>
      `;
      }
      // تغيير من badge = null إلى badgeType = null
      function createCarouselAppCard(app, badgeType = null) {
        return `
          <div class="carousel-app-card bg-white dark:bg-dark-card rounded-xl shadow-md p-4 cursor-pointer border border-gray-200 dark:border-gray-700 relative" onclick="openAppModalById(${
            app.id
          })">
              ${badgeType ? createAppBadge(badgeType) : ""}
              <img src="${app.image}" alt="${
          app.name
        }" class="carousel-app-image mb-3">
              <h3 class="text-center text-gray-900 dark:text-white font-medium text-sm mb-1">${
                app.name
              }</h3>
              <div class="flex items-center justify-center space-x-1 space-x-reverse mb-1">
                  ${createStars(app.rating)}
              </div>
              <p class="text-xs text-gray-500 dark:text-gray-400 text-center">${
                app.downloads
              }</p>
          </div>
      `;
      }
      function updateCarouselSections() {
        // الأكثر استعمالاً - نار حمراء
        const mostUsedApps = getSortedApps("most-used");
        const mostUsedCarousel = document.getElementById("mostUsedCarousel");
        if (mostUsedCarousel) {
          mostUsedCarousel.querySelector(".flex").innerHTML = mostUsedApps
            .map(
              (app) => createCarouselAppCard(app, "fire") // 🔥 → fire
            )
            .join("");
        }

        // الأعلى تقييماً - نجمة صفراء
        const topRatedApps = getSortedApps("top-rated");
        const topRatedCarousel = document.getElementById("topRatedCarousel");
        if (topRatedCarousel) {
          topRatedCarousel.querySelector(".flex").innerHTML = topRatedApps
            .map(
              (app) => createCarouselAppCard(app, "star") // ⭐ → star
            )
            .join("");
        }

        // الأحدث - برق أخضر
        const newestApps = getSortedApps("newest");
        const newestCarousel = document.getElementById("newestCarousel");
        if (newestCarousel) {
          newestCarousel.querySelector(".flex").innerHTML = newestApps
            .map(
              (app) => createCarouselAppCard(app, "new") // 🆕 → new
            )
            .join("");
        }

        // الألعاب المميزة - لعبة بنفسجية
        const featuredGames = getSortedApps("featured-games");
        const featuredGamesCarousel = document.getElementById(
          "featuredGamesCarousel"
        );
        if (featuredGamesCarousel) {
          featuredGamesCarousel.querySelector(".flex").innerHTML = featuredGames
            .map(
              (app) => createCarouselAppCard(app, "game") // 🎮 → game
            )
            .join("");
        }
      }
    </script>
    <script>
      // 1. أولاً، أضف هاتين الدالتين في قسم الـ JavaScript

      // دالة فتح النافذة المنبثقة للتطبيقات المفضلة
      function openFavoriteAppModal(appId) {
        const app = apps.find((a) => a.id === appId);
        if (!app) return;

        currentAppIndex = -1; // تعيين خاص للمفضلة

        // المعلومات الأساسية
        document.getElementById("modalAppName").textContent = app.name;
        document.getElementById("modalCategory").textContent = app.categoryName;
        document.getElementById("modalDescription").textContent =
          app.description;
        document.getElementById("modalImage").src = app.image;
        document.getElementById("modalImage").alt = app.name;

        // التقييم والنجوم
        if (app.rating) {
          document.getElementById("modalRating").innerHTML = createStars(
            app.rating
          );
          document.getElementById(
            "modalRatingText"
          ).textContent = `(${app.rating}/5.0)`;
          document.getElementById("modalRatingDisplay").textContent =
            app.rating;
        } else {
          document.getElementById("modalRating").innerHTML = createStars(0);
          document.getElementById("modalRatingText").textContent = "(غير مقيم)";
          document.getElementById("modalRatingDisplay").textContent = "N/A";
        }

        // الإحصائيات
        document.getElementById("modalDownloads").textContent =
          app.downloads || "غير متوفر";

        // المعلومات التفصيلية
        document.getElementById("modalDeveloper").textContent =
          app.developer || "غير محدد";
        document.getElementById("modalVersion").textContent = app.version;
        document.getElementById("modalSize").textContent = app.size;
        document.getElementById("modalLastUpdate").textContent =
          app.lastUpdate || "غير محدد";
        document.getElementById("modalLanguage").textContent =
          app.language || "غير محدد";
        document.getElementById("modalRequirements").textContent =
          app.requirements || "غير محدد";

        // لقطات الشاشة
        document.getElementById("modalScreenshots").innerHTML =
          createScreenshots(app.screenshots);

        // تحديث زر المفضلة
        updateFavoriteButton(app.id);

        document.getElementById("appModal").classList.remove("hidden");
        document.body.style.overflow = "hidden";
      }

      // دالة إزالة من المفضلة مع منع انتشار الحدث
      function removeFavoriteWithStop(event, appId) {
        event.stopPropagation(); // منع فتح النافذة المنبثقة
        removeFromFavorites(appId);
      }

      // 2. ثم غيّر دالة createFavoriteCard لتصبح كالتالي:

      function createFavoriteCard(app) {
        const t = translations[appSettings.language];
        return `
          <div class="app-card bg-white dark:bg-dark-card rounded-xl shadow-md p-4 border border-gray-200 dark:border-gray-700 cursor-pointer" onclick="openFavoriteAppModal(${app.id})">
              <img src="${app.image}" alt="${app.name}" class="w-full h-24 object-cover rounded-lg mb-3">
              <h3 class="text-center text-gray-900 dark:text-white font-medium text-sm mb-2">${app.name}</h3>
              <button onclick="removeFavoriteWithStop(event, ${app.id})" class="w-full bg-red-500 text-white py-2 px-4 rounded-lg text-xs hover:bg-red-600 transition-colors">
                  ${t.removeFavorite}
              </button>
          </div>
      `;
      }
    </script>
    <script>
      // أضف هذا الكود بعد تعريف appSettings مباشرة:

      // دالة حفظ الإعدادات
      function saveAppSettings() {
        localStorage.setItem("appSettings", JSON.stringify(appSettings));
      }

      // دالة تحميل الإعدادات
      function loadAppSettings() {
        const saved = localStorage.getItem("appSettings");
        if (saved) {
          const savedSettings = JSON.parse(saved);
          appSettings = { ...appSettings, ...savedSettings };
        }
      }
      // عدّل دالة changeLanguage لتصبح:
      function changeLanguage(language) {
        appSettings.language = language;
        const currentLanguageElement =
          document.getElementById("currentLanguage");
        if (currentLanguageElement) {
          currentLanguageElement.textContent = language;
        }

        // تطبيق الترجمة الجديدة
        applyLanguage(language);

        // حفظ الإعداد الجديد
        saveAppSettings();

        closeSettingsModal();
        showNotification(
          translations[language].languageChanged + " " + language
        );
      }
      // عدّل بداية DOMContentLoaded لتصبح:
      document.addEventListener("DOMContentLoaded", () => {
        // تحميل الإعدادات المحفوظة
        loadAppSettings();

        // تهيئة الوضع المظلم
        initializeDarkMode();

        // تطبيق الترجمة المحفوظة
        applyLanguage(appSettings.language);

        // باقي الكود...
      });
      // تحديث اسم اللغة الحالية
      const currentLanguage = document.getElementById("currentLanguage");
      if (currentLanguage) {
        const languageNames = {
          العربية: {
            العربية: "العربية",
            English: "Arabic",
            Français: "Arabe",
          },
          English: {
            العربية: "الإنجليزية",
            English: "English",
            Français: "Anglais",
          },
          Français: {
            العربية: "الفرنسية",
            English: "French",
            Français: "Français",
          },
        };

        currentLanguage.textContent =
          languageNames[appSettings.language][language] || appSettings.language;
      }
      // دالة حفظ حالة الوضع المظلم
      function saveDarkMode() {
        localStorage.setItem("darkMode", isDarkMode);
      }

      // دالة تحميل حالة الوضع المظلم
      function loadDarkMode() {
        const saved = localStorage.getItem("darkMode");
        if (saved !== null) {
          isDarkMode = saved === "true";
        }
      }
      // دالة حفظ حالة العرض المضغوط
      function saveCompactView() {
        localStorage.setItem("compactView", appSettings.compactView);
      }

      // دالة تحميل حالة العرض المضغوط
      function loadCompactView() {
        const saved = localStorage.getItem("compactView");
        if (saved !== null) {
          appSettings.compactView = saved === "true";
        }
      }
      document.querySelectorAll(".category-btn").forEach((btn) => {
        btn.addEventListener("click", () => {
          document
            .querySelectorAll(".category-btn")
            .forEach((b) => b.classList.remove("active"));
          btn.classList.add("active");
          const cat = btn.getAttribute("data-category");
          const map = {
            productivity: "#059669",
            entertainment: "#7c3aed",
            tools: "#ea580c",
            communication: "#4f46e5",
            media: "#db2777",
            all: "#0098DA",
          };
          const w8 = btn.querySelector(".w-8");
          if (w8) {
            w8.style.background = ""; // تحط قيمة لو بغيتي ثابتة
            w8.style.color = map[cat] || "#0098DA";
            const svg = w8.querySelector("svg");
            if (svg) {
              svg.style.color = map[cat];
              svg.style.stroke = map[cat];
              svg.style.fill = "none";
            }
          }
        });
      });
      // دالة تطبيق العرض المضغوط
      function applyCompactView() {
        const appsGrid = document.getElementById("appsGrid");
        const categoryAppsGrid = document.getElementById("categoryAppsGrid");

        if (appSettings.compactView) {
          // تطبيق العرض المضغوط
          if (appsGrid) {
            appsGrid.className =
              "grid grid-cols-3 md:grid-cols-4 lg:grid-cols-5 xl:grid-cols-6 gap-4 mb-8";
          }
          if (categoryAppsGrid) {
            categoryAppsGrid.className =
              "grid grid-cols-3 md:grid-cols-4 lg:grid-cols-5 xl:grid-cols-6 gap-4 mb-8";
          }
        } else {
          // العرض العادي
          if (appsGrid) {
            appsGrid.className = "apps-grid-enhanced mb-8";
          }
          if (categoryAppsGrid) {
            categoryAppsGrid.className = "apps-grid-enhanced mb-8";
          }
        }

        // إعادة عرض التطبيقات بالتخطيط الجديد
        if (
          document
            .getElementById("profileSection")
            ?.classList.contains("active")
        ) {
          displayApps();
        }
        if (
          document
            .getElementById("categorySection")
            ?.classList.contains("active")
        ) {
          displayCategoryApps();
        }
      }

      // تحديث دالة toggleCompactView
      function toggleCompactView(event) {
        if (event) {
          event.stopPropagation();
        }

        appSettings.compactView = !appSettings.compactView;
        saveCompactView();
        saveAppSettings();
        updateToggleSwitchModern("compactViewToggle", appSettings.compactView);

        // تطبيق العرض المضغوط
        applyCompactView();

        const t = translations[appSettings.language];
        showNotification(
          (appSettings.compactView ? "تم تفعيل" : "تم إيقاف") +
            " " +
            t.compactView
        );
      }

      // إضافة استدعاء تحميل وتطبيق العرض المضغوط عند تحميل الصفحة
      document.addEventListener("DOMContentLoaded", function () {
        // تحميل الإعدادات المحفوظة
        loadCompactView();

        // تطبيق العرض المضغوط المحفوظ بعد تحميل كامل للصفحة
        setTimeout(() => {
          applyCompactView();
          updateToggleSwitchModern(
            "compactViewToggle",
            appSettings.compactView
          );
        }, 200);
      });
      // دالة إنشاء أيقونة احترافية للتطبيق
      function createAppBadge(badgeType) {
        const badges = {
          fire: {
            bgColor: "bg-red-50 dark:bg-red-800",
            iconColor: "text-red-600 dark:text-red-200",
            svg: `<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17.657 18.657A8 8 0 016.343 7.343S7 9 9 10c0-2 .5-5 2.986-7C14 5 16.09 5.777 17.656 7.343A7.975 7.975 0 0120 13a7.975 7.975 0 01-2.343 5.657z"></path>`,
          },
          star: {
            bgColor: "bg-yellow-50 dark:bg-yellow-800",
            iconColor: "text-yellow-600 dark:text-yellow-200",
            svg: `<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M11.049 2.927c.3-.921 1.603-.921 1.902 0l1.519 4.674a1 1 0 00.95.69h4.915c.969 0 1.371 1.24.588 1.81l-3.976 2.888a1 1 0 00-.363 1.118l1.518 4.674c.3.922-.755 1.688-1.538 1.118l-3.976-2.888a1 1 0 00-1.176 0l-3.976 2.888c-.783.57-1.838-.197-1.538-1.118l1.518-4.674a1 1 0 00-.363-1.118l-3.976-2.888c-.784-.57-.38-1.81.588-1.81h4.914a1 1 0 00.951-.69l1.519-4.674z"></path>`,
          },
          new: {
            bgColor: "bg-emerald-50 dark:bg-emerald-800",
            iconColor: "text-emerald-600 dark:text-emerald-200",
            svg: `<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 10V3L4 14h7v7l9-11h-7z"></path>`,
          },
          game: {
            bgColor: "bg-purple-50 dark:bg-purple-800",
            iconColor: "text-purple-600 dark:text-purple-200",
            svg: `<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M11 4a2 2 0 114 0v1a1 1 0 001 1h3a1 1 0 011 1v3a1 1 0 01-1 1h-1a2 2 0 100 4h1a1 1 0 011 1v3a1 1 0 01-1 1h-3a1 1 0 01-1-1v-1a2 2 0 10-4 0v1a1 1 0 01-1 1H7a1 1 0 01-1-1v-3a1 1 0 011-1h1a2 2 0 100-4H7a1 1 0 01-1-1V7a1 1 0 011-1h3a1 1 0 001-1V4z"></path>`,
          },
        };

        const badge = badges[badgeType];
        if (!badge) return "";

        return `
          <div class="absolute top-2 right-2 w-8 h-8 rounded-full ${badge.bgColor} flex items-center justify-center shadow-lg z-10 border border-gray-200 dark:border-gray-600">
              <svg class="w-4 h-4 ${badge.iconColor}" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                  ${badge.svg}
              </svg>
          </div>
      `;
      }
      function toggleNotifications() {
        const panel = document.getElementById("notificationsPanel");
        panel.classList.toggle("hidden");
      }
      document.addEventListener("click", function (e) {
        const panel = document.getElementById("notificationsPanel");
        const btn = document.getElementById("notificationToggle");

        if (!panel.contains(e.target) && !btn.contains(e.target)) {
          panel.classList.add("hidden");
        }
      });
      function closeNotifications() {
        const panel = document.getElementById("notificationsPanel");
        if (panel) {
          panel.classList.add("hidden");
        }
      }
      document.addEventListener("click", function (event) {
        const panel = document.getElementById("notificationsPanel");
        const button = document.getElementById("quickDarkModeToggle");

        if (!panel || panel.classList.contains("hidden")) return;

        if (!panel.contains(event.target) && !button.contains(event.target)) {
          closeNotifications();
        }
      });
      function renderLanguageCarousel(languages) {
        const langSpan = document.getElementById("modalLanguage");
        if (!langSpan) return;

        // إذا ما كانتش array أو فيها عنصر واحد
        if (!Array.isArray(languages) || languages.length <= 1) {
          langSpan.textContent = languages ? languages[0] : "";
          return;
        }

        // أكثر من لغة → كاروسيل
        langSpan.innerHTML = ""; // نفرغ القديم

        const wrapper = document.createElement("div");
        wrapper.className = "flex gap-2 overflow-x-auto py-1 max-w-full";

        languages.forEach((lang) => {
          const badge = document.createElement("span");
          badge.className =
            "whitespace-nowrap px-2 py-1 text-xs rounded-full bg-gray-200 dark:bg-gray-700 text-gray-700 dark:text-gray-200";
          badge.textContent = lang;
          wrapper.appendChild(badge);
        });

        langSpan.appendChild(wrapper);
      }
    </script>
<script>
(function () {
  const shareBtn = document.getElementById("shareBtn");
  const sheet = document.getElementById("shareSheet");
  const content = document.getElementById("shareContent");

  if (!shareBtn || !sheet || !content) {
    console.error("عنصر ناقص");
    return;
  }

  const url = encodeURIComponent(window.location.href);
  const text = encodeURIComponent("جرّب هذا التطبيق");

  document.getElementById("wa").href =
    "https://wa.me/?text=" + text + "%20" + url;
  document.getElementById("fb").href =
    "https://www.facebook.com/sharer/sharer.php?u=" + url;
  document.getElementById("tg").href =
    "https://t.me/share/url?url=" + url + "&text=" + text;
  document.getElementById("tw").href =
    "https://twitter.com/intent/tweet?url=" + url + "&text=" + text;

  shareBtn.onclick = function () {
    sheet.style.display = "block";
    setTimeout(() => {
      content.style.transform = "translateY(0)";
    }, 10);
  };

  window.closeShare = function () {
    content.style.transform = "translateY(100%)";
    setTimeout(() => {
      sheet.style.display = "none";
    }, 300);
  };

  sheet.addEventListener("click", function (e) {
    if (e.target === sheet) closeShare();
  });
})();
</script>
  </body>
</html>

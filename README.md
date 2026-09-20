<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Alislamiah-Tube</title>
  <link rel="icon" href="icon.png" type="image/png">
  <link href="https://googleapis.com" rel="stylesheet">
  <style>
    *{margin:0;padding:0;box-sizing:border-box}
    body{font-family:'Cairo',sans-serif;background:#0f0f0f;color:#fff;min-height:100vh;padding-bottom:80px}
    .header{background:#1a1a1a;padding:12px 20px;position:sticky;top:0;z-index:100;border-bottom:1px solid #333;display:flex;align-items:center;gap:12px}
    .app-icon{width:42px;height:42px;border-radius:10px;object-fit:cover}
    .header h1{font-size:1.4rem;font-weight:700;color:#4ade80}
    .main-content{padding:20px;max-width:1200px;margin:0 auto}
    .section-title{font-size:1.3rem;margin-bottom:20px;color:#e5e5e5}
    .videos-grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(280px,1fr));gap:20px}
    .video-card{background:#1a1a1a;border-radius:12px;overflow:hidden;text-decoration:none;color:#fff;display:block}
    .video-thumbnail{width:100%;aspect-ratio:16/9;background:#000}
    .video-thumbnail video{width:100%;height:100%;object-fit:cover;pointer-events:none}
    .video-info{padding:14px}
    .video-title{font-size:1rem;font-weight:600;line-height:1.4;margin-bottom:6px}
    .video-meta{font-size:0.85rem;color:#888}
    .bottom-nav{position:fixed;bottom:0;left:0;right:0;background:#1a1a1a;display:flex;justify-content:space-around;padding:10px 0;border-top:1px solid #333;z-index:100}
    .nav-item{display:flex;flex-direction:column;align-items:center;text-decoration:none;color:#888;font-size:0.8rem;gap:4px}
    .nav-item.active{color:#4ade80}
    .nav-item .icon{font-size:1.4rem}
    
    /* تنسيق زر تحويل اللغة في الهيدر */
    .lang-toggle-btn {margin-right:auto; background:#4ade80; color:#000; border:none; padding:6px 14px; border-radius:8px; font-family:'Cairo',sans-serif; font-weight:700; cursor:pointer; font-size:0.85rem; transition:0.2s}
    .lang-toggle-btn:hover {background:#3bbd6c}
    /* عند قلب الاتجاه للغة الإنجليزية يندفع الزر لليسار تلقائيًا */
    html[dir="ltr"] .lang-toggle-btn {margin-left:auto; margin-right:0}
  </style>
</head>
<body>
  <header class="header">
    <img src="icon.png" class="app-icon" alt="Alislamiah-Tube Icon">
    <h1>Alislamiah-Tube</h1>
    
    <!-- زر تبديل اللغة المضاف ذكياً وبحفظ تلقائي 🌐 -->
    <button id="lang-btn" class="lang-toggle-btn" onclick="toggleLanguage()">EN</button>
  </header>

  <main class="main-content">
    <h2 class="section-title" id="main-section-title">أحدث الفيديوهات</h2>
    <div class="videos-grid">
      
      <!-- فيديو 1 -->
      <a href="watch.html?v=IMG_20260814_164242_861.mp4&title=ما تيسر من سورة إبراهيم" class="video-card">
        <div class="video-thumbnail">
          <video preload="metadata" muted autoplay loop playsinline>
            <source src="IMG_20260814_164242_861.mp4" type="video/mp4">
          </video>
        </div>
        <div class="video-info">
          <div class="video-title">ما تيسر من سورة إبراهيم</div>
          <div class="video-meta">Alislamiah-Tube</div>
        </div>
      </a>

      <!-- فيديو 2 -->
      <a href="watch.html?v=lv_0_20260824111719.mp4&title=آيات من سورة مريم بصوت مشاري راشد العفاسي" class="video-card">
        <div class="video-thumbnail">
          <video preload="metadata" muted autoplay loop playsinline>
            <source src="lv_0_20260824111719.mp4" type="video/mp4">
          </video>
        </div>
        <div class="video-info">
          <div class="video-title">آيات من سورة مريم بصوت مشاري راشد العفاسي</div>
          <div class="video-meta">Alislamiah-Tube</div>
        </div>
      </a>

      <!-- فيديو 3 -->
      <a href="watch.html?v=surah-yasin.mp4&title=ما تيسر من سورة يس" class="video-card">
        <div class="video-thumbnail">
          <video preload="metadata" muted autoplay loop playsinline>
            <source src="surah-yasin.mp4" type="video/mp4">
          </video>
        </div>
        <div class="video-info">
          <div class="video-title">ما تيسر من سورة يس</div>
          <div class="video-meta">Alislamiah-Tube</div>
        </div>
      </a>

      <!-- فيديو 4 -->
      <a href="watch.html?v=فرض الفصل الثالث سنة ثالثة متوسط في العلوم الفيزيائية (1).mp4&title=فرض الفصل الثالث سنة ثالثة متوسط في العلوم الفيزيائية (1)" class="video-card">
        <div class="video-thumbnail">
          <video preload="metadata" muted autoplay loop playsinline>
            <source src="فرض الفصل الثالث سنة ثالثة متوسط في العلوم الفيزيائية (1).mp4" type="video/mp4">
          </video>
        </div>
        <div class="video-info">
          <div class="video-title">فرض الفصل الثالث سنة ثالثة متوسط في العلوم الفيزيائية (1)</div>
          <div class="video-meta">Alislamiah-Tube</div>
        </div>
      </a>

      <!-- فيديو 5 -->
      <a href="watch.html?v=فرض الفصل الثالث سنة ثالثة متوسط في العلوم الفيزيائية.mp4&title=فرض الفصل الثالث سنة ثالثة متوسط في العلوم الفيزيائية" class="video-card">
        <div class="video-thumbnail">
          <video preload="metadata" muted autoplay loop playsinline>
            <source src="فرض الفصل الثالث سنة ثالثة متوسط في العلوم الفيزيائية.mp4" type="video/mp4">
          </video>
        </div>
        <div class="video-info">
          <div class="video-title">فرض الفصل الثالث سنة ثالثة متوسط في العلوم الفيزيائية</div>
          <div class="video-meta">Alislamiah-Tube</div>
        </div>
      </a>

      <!-- فيديو 6 -->
      <a href="watch.html?v=فرض الفصل الثالث في ماده العلوم الفيزيائيه السنه اولى متوسط.mp4&title=فرض الفصل الثالث في مادة العلوم الفيزيائية السنة الأولى متوسط" class="video-card">
        <div class="video-thumbnail">
          <video preload="metadata" muted autoplay loop playsinline>
            <source src="فرض الفصل الثالث في ماده العلوم الفيزيائيه السنه اولى متوسط.mp4" type="video/mp4">
          </video>
        </div>
        <div class="video-info">
          <div class="video-title">فرض الفصل الثالث في مادة العلوم الفيزيائية السنة الأولى متوسط</div>
          <div class="video-meta">Alislamiah-Tube</div>
        </div>
      </a>

      <!-- فيديو 7 -->
      <a href="watch.html?v=نموذج مقترح فرض الفصل الثالث سنة ثالثة متوسط.mp4&title=نموذج مقترح فرض الفصل الثالث سنة ثالثة متوسط" class="video-card">
        <div class="video-thumbnail">
          <video preload="metadata" muted autoplay loop playsinline>
            <source src="نموذج مقترح فرض الفصل الثالث سنة ثالثة متوسط.mp4" type="video/mp4">
          </video>
        </div>
        <div class="video-info">
          <div class="video-title">نموذج مقترح فرض الفصل الثالث سنة ثالثة متوسط</div>
          <div class="video-meta">Alislamiah-Tube</div>
        </div>
      </a>

      <!-- فيديو 8 -->
      <a href="watch.html?v=شرح درس الخطاب المباشر والغير مباشر مكتوب.mp4&title=شرح درس الخطاب المباشر والغير مباشر مكتوب" class="video-card">
        <div class="video-thumbnail">
          <video preload="metadata" muted autoplay loop playsinline>
            <source src="شرح درس الخطاب المباشر والغير مباشر مكتوب.mp4" type="video/mp4">
          </video>
        </div>
        <div class="video-info">
          <div class="video-title">شرح درس الخطاب المباشر والغير مباشر مكتوب</div>
          <div class="video-meta">Alislamiah-Tube</div>
        </div>
      </a>

    </div>
  </main>

  <!-- القائمة السفلية المعدلة بتبديل جيميناي بصفحة الإعدادات ⚙️ -->
  <nav class="bottom-nav">
    <a href="index.html" class="nav-item active"><span class="icon">🏠</span><span id="nav-home">الرئيسية</span></a>
    <a href="search.html" class="nav-item"><span class="icon">🔍</span><span id="nav-search">البحث</span></a>
    <a href="Settings.html" class="nav-item"><span class="icon">⚙️</span><span id="nav-settings">الإعدادات</span></a>
  </nav>

  <script>
    // قاموس اللغات لتبديل النصوص والاتجاهات
    const translations = {
      ar: {
        title: "أحدث الفيديوهات",
        home: "الرئيسية",
        search: "البحث",
        settings: "الإعدادات",
        btn: "EN",
        dir: "rtl"
      },
      en: {
        title: "Latest Videos",
        home: "Home",
        search: "Search",
        settings: "Settings",
        btn: "AR",
        dir: "ltr"
      }
    };

    let currentLang = localStorage.getItem('app_lang') || 'ar';

    function applyLanguage(lang) {
      document.documentElement.setAttribute('dir', translations[lang].dir);
      document.documentElement.setAttribute('lang', lang);

      if(document.getElementById('main-section-title')) {
        document.getElementById('main-section-title').innerText = translations[lang].title;
      }
      if(document.getElementById('nav-home')) {
        document.getElementById('nav-home').innerText = translations[lang].home;
      }
      if(document.getElementById('nav-search')) {
        document.getElementById('nav-search').innerText = translations[lang].search;
      }
      if(document.getElementById('nav-settings')) {
        document.getElementById('nav-settings').innerText = translations[lang].settings;
      }
      
      document.getElementById('lang-btn').innerText = translations[lang].btn;
    }

    function toggleLanguage() {
      currentLang = currentLang === 'ar' ? 'en' : 'ar';
      localStorage.setItem('app_lang', currentLang);
      applyLanguage(currentLang);
    }

    // تفعيل اللغة مباشرة فور فتح التطبيق
    applyLanguage(currentLang);
  </script>
</body>
</html>

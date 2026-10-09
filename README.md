<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Alislamiah-Tube</title>

  <link rel="icon" href="icon.png" type="image/png">
  <link href="https://fonts.googleapis.com/css2?family=Cairo:wght@400;600;700&display=swap" rel="stylesheet">

  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; -webkit-tap-highlight-color: transparent; }
    body { font-family: 'Cairo', Arial, sans-serif; background: #07111f; color: #fff; min-height: 100vh; padding-bottom: 90px; }
    
    /* ========== شاشة الترحيب والتأثير (Splash Screen) ========== */
    .splash-screen {
      position: fixed;
      inset: 0;
      background: #07111f;
      display: flex;
      justify-content: center;
      align-items: center;
      z-index: 9999;
      transition: opacity 0.6s ease, visibility 0.6s ease;
    }

    .splash-screen.hidden {
      opacity: 0;
      visibility: hidden;
    }

    /* الحاوية الدائرية التي تدور محيط الأيقونة */
    .icon-spinner-wrapper {
      position: relative;
      width: 120px;
      height: 120px;
      display: flex;
      align-items: center;
      justify-content: center;
      border-radius: 28px;
    }

    /* حلقة الألوان الدوارة على المحيط */
    .icon-spinner-wrapper::before {
      content: '';
      position: absolute;
      inset: -6px;
      border-radius: 32px;
      background: conic-gradient(from 0deg, #087fff, #00c3ff, #6fb7ff, #3d9cff, #087fff);
      animation: rotateBorder 1.8s linear infinite;
    }

    /* غطاء خلفي لفصل الأيقونة عن الإطار */
    .icon-spinner-wrapper::after {
      content: '';
      position: absolute;
      inset: -2px;
      background: #07111f;
      border-radius: 30px;
    }

    /* صورة الأيقونة بداخل الإطار */
    .splash-icon {
      position: relative;
      z-index: 2;
      width: 100px;
      height: 100px;
      border-radius: 22px;
      object-fit: cover;
      box-shadow: 0 10px 30px rgba(8, 127, 255, 0.35);
    }

    @keyframes rotateBorder {
      0% { transform: rotate(0deg); }
      100% { transform: rotate(360deg); }
    }

    /* ========== باقي تنسيقات الصفحة الرئيسية ========== */
    .header { background: #0a1728; padding: 12px 20px; position: sticky; top: 0; z-index: 100; border-bottom: 1px solid #18304b; display: flex; align-items: center; gap: 12px; }
    .app-icon { width: 42px; height: 42px; border-radius: 10px; object-fit: cover; }
    .header h1 { font-size: 1.35rem; font-weight: 700; color: #6fb7ff; }
    .main-content { padding: 24px 16px 30px; max-width: 1200px; margin: 0 auto; }
    .section-title { font-size: 1.3rem; margin-bottom: 20px; color: #ffffff; font-weight: 700; }
    .videos-grid { display: grid; grid-template-columns: repeat(auto-fill, minmax(280px, 1fr)); gap: 20px; }
    .video-card { background: #0b1a2c; border: 1px solid #173553; border-radius: 12px; overflow: hidden; text-decoration: none; color: #fff; display: block; box-shadow: 0 8px 25px rgba(0,0,0,0.25); transition: transform 0.2s ease; }
    .video-card:hover { transform: translateY(-3px); }
    .video-thumbnail { width: 100%; aspect-ratio: 16/9; background: #000; }
    .video-thumbnail video { width: 100%; height: 100%; object-fit: cover; pointer-events: none; }
    .video-info { padding: 14px; }
    .video-title { font-size: 1rem; font-weight: 600; line-height: 1.4; margin-bottom: 6px; color: #f5f9ff; }
    .video-meta { font-size: 0.85rem; color: #718ba6; }
    .bottom-nav { position: fixed; bottom: 0; left: 0; right: 0; background: #081525; display: flex; justify-content: space-around; padding: 10px 0; border-top: 1px solid #17304a; z-index: 100; }
    .nav-item { display: flex; flex-direction: column; align-items: center; justify-content: center; text-decoration: none; color: #718096; font-size: 0.78rem; gap: 4px; min-width: 70px; }
    .nav-item.active { color: #62b4ff; }
    .nav-item .icon { font-size: 1.35rem; }
  </style>
</head>
<body>

  <!-- شاشة الترحيب المؤقتة قبل فتح الرئيسية -->
  <div class="splash-screen" id="splash">
    <div class="icon-spinner-wrapper">
      <img src="icon.png" class="splash-icon" alt="Logo" onerror="this.src='data:image/svg+xml;utf8,<svg xmlns=\'http://www.w3.org/2000/svg\' viewBox=\'0 0 100 100\'><rect width=\'100\' height=\'100\' rx=\'20\' fill=\'%23087fff\'/><text x=\'50\' y=\'65\' font-size=\'50\' text-anchor=\'middle\' fill=\'white\'>▶</text></svg>'">
    </div>
  </div>

  <header class="header">
    <img src="icon.png" class="app-icon" alt="Alislamiah">
    <h1 id="header-title">Alislamiah-Tube</h1>
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
      <a href="watch.html?v=IMG_20260812_142700_033.mp4&title=بل الساعة موعدهم والساعة أدهى وأمر تلاوة عطرة بصوت الشيخ مشاري العفاسي" class="video-card">
        <div class="video-thumbnail">
          <video preload="metadata" muted autoplay loop playsinline>
            <source src="IMG_20260812_142700_033.mp4" type="video/mp4">
          </video>
        </div>
        <div class="video-info">
          <div class="video-title">بل الساعة موعدهم والساعة أدهى وأمر تلاوة عطرة بصوت الشيخ مشاري العفاسي</div>
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

  <nav class="bottom-nav">
    <a href="index.html" class="nav-item active">
      <span class="icon">🏠</span>
      <span id="nav-home">الرئيسية</span>
    </a>
    <a href="search.html" class="nav-item">
      <span class="icon">🔍</span>
      <span id="nav-search">البحث</span>
    </a>
    <a href="Settings.html" class="nav-item">
      <span class="icon">⚙️</span>
      <span id="nav-settings">الإعدادات</span>
    </a>
  </nav>

  <script>
    // مؤقت الخمس ثوانٍ لإخفاء شاشة الترحيب
    window.addEventListener("DOMContentLoaded", () => {
      setTimeout(() => {
        const splash = document.getElementById("splash");
        if (splash) {
          splash.classList.add("hidden");
        }
      }, 5000); // 5000 ميلي ثانية = 5 ثوانٍ
    });

    const translations = {
      ar: { dir: "rtl", header: "Alislamiah-Tube", title: "أحدث الفيديوهات", home: "الرئيسية", search: "البحث", settings: "الإعدادات" },
      fr: { dir: "ltr", header: "Alislamiah-Tube", title: "Dernières Vidéos", home: "Accueil", search: "Recherche", settings: "Paramètres" },
      en: { dir: "ltr", header: "Alislamiah-Tube", title: "Latest Videos", home: "Home", search: "Search", settings: "Settings" }
    };

    let currentLang = localStorage.getItem("app_lang") || "ar";

    function applyLanguage(lang) {
      if (!translations[lang]) lang = "ar";
      const t = translations[lang];

      document.documentElement.setAttribute("lang", lang);
      document.documentElement.setAttribute("dir", t.dir);

      document.getElementById("header-title").textContent = t.header;
      document.getElementById("main-section-title").textContent = t.title;
      document.getElementById("nav-home").textContent = t.home;
      document.getElementById("nav-search").textContent = t.search;
      document.getElementById("nav-settings").textContent = t.settings;
    }

    applyLanguage(currentLang);
  </script>
</body>
</html>

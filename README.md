<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Alislamiah-Tube</title>
  <link rel="icon" href="icon.png" type="image/png">
  <link href="https://googleapis.com" rel="stylesheet">
  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; -webkit-tap-highlight-color: transparent; }
    body { font-family: Arial, Tahoma, sans-serif; background: #07111f; color: #fff; min-height: 100vh; padding-bottom: 90px; }
    .header { background: #0a1728; padding: 12px 20px; position: sticky; top: 0; z-index: 100; border-bottom: 1px solid #18304b; display: flex; align-items: center; gap: 12px; }
    .app-icon { width: 42px; height: 42px; border-radius: 10px; object-fit: cover; }
    .header h1 { font-size: 1.35rem; font-weight: 700; color: #6fb7ff; }
    .main-content { padding: 24px 16px 30px; max-width: 1200px; margin: 0 auto; }
    .section-title { font-size: 1.3rem; margin-bottom: 20px; color: #ffffff; font-weight: 700; }
    .videos-grid { display: grid; grid-template-columns: repeat(auto-fill, minmax(280px, 1fr)); gap: 20px; }
    .video-card { background: #0b1a2c; border: 1px solid #173553; border-radius: 12px; overflow: hidden; text-decoration: none; color: #fff; display: block; box-shadow: 0 8px 25px rgba(0,0,0,0.25); }
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

      <!-- فيديو 3: تم إرجاع فيديو بل الساعة موعدهم هنا بنجاح ✅ -->
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

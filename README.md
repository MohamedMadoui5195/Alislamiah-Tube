<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Alislamiah-Tube</title>
  <!-- تم تصحيح مسار أيقونة التبويب العلوي لتستدعى من المستودع مباشرة ✅ -->
  <link rel="icon" href="icon.png" type="image/png">
  <link href="https://fonts.googleapis.com/css2?family=Cairo:wght@400;600;700&display=swap" rel="stylesheet">
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
  </style>
</head>
<body>
  <header class="header">
    <!-- تم تصحيح مسار الأيقونة هنا وحذف المجلدات الزائدة التي لم تكن موجودة في ريبو GitHub ✅ -->
    <img src="icon.png" class="app-icon" alt="Alislamiah-Tube Icon">
    <h1>Alislamiah-Tube</h1>
  </header>

  <main class="main-content">
    <h2 class="section-title">أحدث الفيديوهات</h2>
    <div class="videos-grid">
      
      <!-- الفيديو الأول: تم تعديل الرابط ليمرر اسم الفيديو والعنوان لصفحة watch.html وتصحيح مسار السورس ليعمل كمعاينة صامتة ✅ -->
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

      <!-- الفيديو الثاني: تم تعديل الرابط وتصحيح مسار السورس لتشغيل المعاينة مباشرة من جذر المستودع ✅ -->
      <a href="watch.html?v=lv_0_20260824111719.mp4&title=آيات من سورة مريم بصوت مشاري راشد العفاسي" class="video-card">
        <div class="video-thumbnail">
          <video preload="metadata" muted autoplay loop playsinline>
            <source src="lv_0_20260824111719.mp4" type="video/mp4">
          </video>
        </div>
        <div class="video-info">
          <div class="video-title">آيات من سورة مريم بصوت مشاري راشد العفاسي</div>
          <div

 class="video-meta">Alislamiah-Tube</div>
        </div>
      </a>

      <!-- الفيديو الثالث: بل الساعة موعدهم - الشيخ مشاري العفاسي 🌟 -->
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
      <!-- فيديو 4: فرض الفصل الثالث سنة ثالثة متوسط في العلوم الفيزيائية (1) -->
      <a href="watch.html?v=فرض الفصل الثالث سنة ثالثة متوسط في العلوم الفيزيائية (1).mp4&title=فرض الفصل الثالث سنة ثالثة متوسط في العلوم الفيزيائية (1)" class="video-card">
        <div class="video-thumbnail">
          <video preload="metadata" muted autoplay loop playsinline>
            <source src="فرض الفصل الثالث سنة ثالثة متوسط in العلوم الفيزيائية (1).mp4" type="video/mp4">
          </video>
        </div>
        <div class="video-info">
          <div class="video-title">فرض الفصل الثالث سنة ثالثة متوسط في العلوم الفيزيائية (1)</div>
          <div class="video-meta">Alislamiah-Tube</div>
        </div>
      </a>

      <!-- فيديو 5: فرض الفصل الثالث سنة ثالثة متوسط في العلوم الفيزيائية -->
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

      <!-- فيديو 6: فرض الفصل الثالث في ماده العلوم الفيزيائيه السنه اولى متوسط -->
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

      <!-- فيديو 7: نموذج مقترح فرض الفصل الثالث سنة ثالثة متوسط -->
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

      <!-- فيديو 8: شرح درس الخطاب المباشر والغير مباشر مكتوب -->
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
    <a href="index.html" class="nav-item active"><span class="icon">🏠</span><span>الرئيسية</span></a>
    <a href="search.html" class="nav-item"><span class="icon">🔍</span><span>البحث</span></a>
    <a href="https://gemini.google.com" target="_blank" class="nav-item"><span class="icon">✨</span><span>Gemini</span></a>
  </nav>
</body>
</html>

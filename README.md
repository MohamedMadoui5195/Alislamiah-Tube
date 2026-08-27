<!DOCTYPE html>
<html lang="ar" dir="rtl">

<head>

<meta charset="UTF-8">

<meta name="viewport"
content="width=device-width, initial-scale=1.0">

<meta name="theme-color" content="#0f0f0f">

<title>Alislamiah tube</title>

<style>

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:Arial, sans-serif;
}

body{

    background:#0f0f0f;

    color:white;

    min-height:100vh;

    padding-bottom:80px;

}


/* =========================
   HEADER
========================= */

.header{

    position:sticky;

    top:0;

    z-index:1000;

    background:#0f0f0f;

    border-bottom:1px solid #292929;

    padding:10px 15px;

}


/* LOGO */

.logo-area{

    display:flex;

    justify-content:center;

    align-items:center;

    margin-bottom:12px;

}

.logo{

    width:180px;

    height:auto;

    max-height:85px;

    object-fit:contain;

}


/* SEARCH */

.search-area{

    display:flex;

    align-items:center;

    gap:8px;

    max-width:700px;

    margin:auto;

}

.search-box{

    flex:1;

    background:#222;

    border:1px solid #333;

    border-radius:25px;

    height:45px;

    display:flex;

    align-items:center;

    padding:0 15px;

}

.search-box input{

    width:100%;

    background:none;

    border:none;

    outline:none;

    color:white;

    font-size:16px;

    text-align:right;

}

.search-box input::placeholder{

    color:#aaa;

}

.search-button{

    width:45px;

    height:45px;

    border-radius:50%;

    border:none;

    background:#272727;

    color:white;

    font-size:20px;

    cursor:pointer;

}


/* =========================
   CATEGORIES
========================= */

.categories{

    display:flex;

    gap:10px;

    overflow-x:auto;

    padding:15px;

    scrollbar-width:none;

}

.categories::-webkit-scrollbar{

    display:none;

}

.category{

    white-space:nowrap;

    background:#272727;

    border:none;

    color:white;

    padding:9px 18px;

    border-radius:20px;

    cursor:pointer;

    font-size:14px;

}

.category.active{

    background:white;

    color:black;

}


/* =========================
   CONTENT
========================= */

.container{

    max-width:1200px;

    margin:auto;

    padding:5px 15px 30px;

}


/* VIDEO GRID */

.video-grid{

    display:grid;

    grid-template-columns:
    repeat(auto-fill,minmax(260px,1fr));

    gap:25px 18px;

}


/* VIDEO CARD */

.video-card{

    cursor:pointer;

    transition:transform .2s;

}

.video-card:hover{

    transform:translateY(-3px);

}


/* THUMBNAIL */

.thumbnail{

    width:100%;

    aspect-ratio:16/9;

    background:#202020;

    border-radius:12px;

    overflow:hidden;

    position:relative;

}

.thumbnail img{

    width:100%;

    height:100%;

    object-fit:cover;

}

.duration{

    position:absolute;

    bottom:8px;

    left:8px;

    background:rgba(0,0,0,.85);

    padding:4px 7px;

    border-radius:4px;

    font-size:12px;

}


/* VIDEO INFO */

.video-info{

    display:flex;

    gap:10px;

    padding-top:10px;

}

.channel-icon{

    width:38px;

    height:38px;

    border-radius:50%;

    background:#222;

    display:flex;

    align-items:center;

    justify-content:center;

    overflow:hidden;

    flex:none;

}

.channel-icon img{

    width:100%;

    height:100%;

    object-fit:cover;

}

.video-text{

    flex:1;

}

.video-title{

    font-size:16px;

    line-height:1.5;

    font-weight:bold;

    display:-webkit-box;

    -webkit-line-clamp:2;

    -webkit-box-orient:vertical;

    overflow:hidden;

}

.video-meta{

    color:#aaa;

    font-size:13px;

    margin-top:5px;

}


/* =========================
   EMPTY SEARCH
========================= */

.no-results{

    text-align:center;

    padding:70px 20px;

    display:none;

}

.no-results-icon{

    font-size:55px;

    margin-bottom:15px;

}

.no-results h2{

    margin-bottom:8px;

}

.no-results p{

    color:#aaa;

}


/* =========================
   BOTTOM NAVIGATION
========================= */

.bottom-nav{

    position:fixed;

    bottom:0;

    left:0;

    right:0;

    height:70px;

    background:#0f0f0f;

    border-top:1px solid #292929;

    display:flex;

    justify-content:space-around;

    align-items:center;

    z-index:2000;

}

.nav-item{

    background:none;

    border:none;

    color:#aaa;

    cursor:pointer;

    display:flex;

    flex-direction:column;

    align-items:center;

    gap:5px;

    font-size:12px;

}

.nav-icon{

    font-size:23px;

}

.nav-item.active{

    color:white;

}


/* =========================
   VIDEO MODAL
========================= */

.video-modal{

    position:fixed;

    inset:0;

    background:rgba(0,0,0,.96);

    z-index:3000;

    display:none;

    overflow-y:auto;

    padding:20px;

}

.modal-content{

    max-width:900px;

    margin:30px auto;

}

.close-button{

    position:fixed;

    top:15px;

    right:20px;

    width:45px;

    height:45px;

    border-radius:50%;

    background:#222;

    color:white;

    border:none;

    font-size:25px;

    cursor:pointer;

}

.player{

    width:100%;

    aspect-ratio:16/9;

    background:black;

    border-radius:12px;

    overflow:hidden;

}

.player iframe{

    width:100%;

    height:100%;

    border:none;

}

.modal-title{

    font-size:22px;

    margin-top:20px;

}

.modal-description{

    color:#aaa;

    margin-top:10px;

    line-height:1.8;

}


/* ACTIONS */

.actions{

    display:flex;

    gap:10px;

    margin-top:20px;

}

.action-button{

    background:#272727;

    border:none;

    color:white;

    padding:10px 18px;

    border-radius:22px;

    cursor:pointer;

}


/* =========================
   RESPONSIVE
========================= */

@media(max-width:600px){

    .logo{

        width:145px;

        max-height:70px;

    }

    .video-grid{

        grid-template-columns:1fr;

        gap:25px;

    }

    .container{

        padding-left:10px;

        padding-right:10px;

    }

    .video-title{

        font-size:15px;

    }

}

</style>

</head>


<body>


<!-- =========================
     HEADER
========================= -->

<header class="header">

    <div class="logo-area">

        <img
        src="1787868766350.png"
        class="logo"
        alt="Alislamiah tube">

    </div>


    <div class="search-area">

        <div class="search-box">

            <input
            type="text"
            id="searchInput"
            placeholder="ابحث في Alislamiah tube..."
            oninput="searchVideos()">

        </div>

        <button
        class="search-button"
        onclick="searchVideos()">

            🔍

        </button>

    </div>

</header>



<!-- =========================
     CATEGORIES
========================= -->

<div class="categories">

    <button
    class="category active"
    onclick="filterVideos('all',this)">
        الكل
    </button>

    <button
    class="category"
    onclick="filterVideos('quran',this)">
        القرآن الكريم
    </button>

    <button
    class="category"
    onclick="filterVideos('islamic',this)">
        إسلاميات
    </button>

    <button
    class="category"
    onclick="filterVideos('english',this)">
        الإنجليزية
    </button>

    <button
    class="category"
    onclick="filterVideos('education',this)">
        التعليم
    </button>

    <button
    class="category"
    onclick="filterVideos('shorts',this)">
        Shorts
    </button>

</div>



<!-- =========================
     VIDEOS
========================= -->

<main class="container">

<div class="video-grid" id="videoGrid">


<!-- VIDEO 1 -->

<div
class="video-card"
data-category="quran"
data-title="تلاوة القرآن الكريم سورة الفاتحة"
onclick="openVideo(
'https://www.youtube.com/embed/dQw4w9WgXcQ',
'تلاوة القرآن الكريم - سورة الفاتحة',
'Alislamiah tube'
)">

    <div class="thumbnail">

        <img
        src="https://images.unsplash.com/photo-1609599006353-e629aaabfeae?auto=format&fit=crop&w=900&q=80"
        alt="القرآن الكريم">

        <span class="duration">
            12:45
        </span>

    </div>


    <div class="video-info">

        <div class="channel-icon">

            <img
            src="1000019187.png"
            alt="Alislamiah">

        </div>

        <div class="video-text">

            <div class="video-title">
                تلاوة القرآن الكريم - سورة الفاتحة
            </div>

            <div class="video-meta">
                Alislamiah tube
                • 1.2K مشاهدة
                • منذ يومين
            </div>

        </div>

    </div>

</div>



<!-- VIDEO 2 -->

<div
class="video-card"
data-category="islamic"
data-title="أجمل الأذكار اليومية"
onclick="openVideo(
'https://www.youtube.com/embed/dQw4w9WgXcQ',
'أجمل الأذكار اليومية',
'Alislamiah tube'
)">

    <div class="thumbnail">

        <img
        src="https://images.unsplash.com/photo-1519817650390-64a93db51149?auto=format&fit=crop&w=900&q=80"
        alt="الأذكار">

        <span class="duration">
            08:32
        </span>

    </div>


    <div class="video-info">

        <div class="channel-icon">

            <img
            src="1000019187.png"
            alt="Alislamiah">

        </div>

        <div class="video-text">

            <div class="video-title">
                أجمل الأذكار اليومية
            </div>

            <div class="video-meta">
                Alislamiah tube
                • 850 مشاهدة
                • منذ 5 أيام
            </div>

        </div>

    </div>

</div>



<!-- VIDEO 3 -->

<div
class="video-card"
data-category="english"
data-title="تعلم الإنجليزية بطريقة سهلة"
onclick="openVideo(
'https://www.youtube.com/embed/dQw4w9WgXcQ',
'تعلم الإنجليزية بطريقة سهلة',
'Alislamiah tube'
)">

    <div class="thumbnail">

        <img
        src="https://images.unsplash.com/photo-1546410531-bb4caa6b424d?auto=format&fit=crop&w=900&q=80"
        alt="English">

        <span class="duration">
            15:20
        </span>

    </div>


    <div class="video-info">

        <div class="channel-icon">

            <img
            src="1000019187.png"
            alt="Alislamiah">

        </div>

        <div class="video-text">

            <div class="video-title">
                تعلم الإنجليزية بطريقة سهلة
            </div>

            <div class="video-meta">
                Alislamiah tube
                • 2.4K مشاهدة
                • منذ أسبوع
            </div>

        </div>

    </div>

</div>



<!-- VIDEO 4 -->

<div
class="video-card"
data-category="education"
data-title="درس جديد لطلاب البكالوريا"
onclick="openVideo(
'https://www.youtube.com/embed/dQw4w9WgXcQ',
'درس جديد لطلاب البكالوريا',
'Alislamiah tube'
)">

    <div class="thumbnail">

        <img
        src="https://images.unsplash.com/photo-1503676260728-1c00da094a0b?auto=format&fit=crop&w=900&q=80"
        alt="Education">

        <span class="duration">
            20:10
        </span>

    </div>


    <div class="video-info">

        <div class="channel-icon">

            <img
            src="1000019187.png"
            alt="Alislamiah">

        </div>

        <div class="video-text">

            <div class="video-title">
                درس جديد لطلاب البكالوريا
            </div>

            <div class="video-meta">
                Alislamiah tube
                • 3.1K مشاهدة
                • منذ أسبوعين
            </div>

        </div>

    </div>

</div>


</div>


<!-- NO RESULTS -->

<div
class="no-results"
id="noResults">

    <div class="no-results-icon">
        🔍
    </div>

    <h2>
        لم نجد أي نتيجة
    </h2>

    <p>
        جرّب البحث بكلمة أخرى
    </p>

</div>


</main>



<!-- =========================
     BOTTOM NAV
========================= -->

<nav class="bottom-nav">

    <button
    class="nav-item active"
    onclick="goHome(this)">

        <span class="nav-icon">
            🏠
        </span>

        الرئيسية

    </button>


    <button
    class="nav-item"
    onclick="focusSearch(this)">

        <span class="nav-icon">
            🔍
        </span>

        بحث

    </button>


    <button
    class="nav-item"
    onclick="showMessage('سيتم إضافة الاشتراكات قريبًا')">

        <span class="nav-icon">
            📺
        </span>

        الاشتراكات

    </button>


    <button
    class="nav-item"
    onclick="showMessage('سيتم إضافة المكتبة قريبًا')">

        <span class="nav-icon">
            📚
        </span>

        المكتبة

    </button>

</nav>



<!-- =========================
     VIDEO MODAL
========================= -->

<div
class="video-modal"
id="videoModal">

    <button
    class="close-button"
    onclick="closeVideo()">

        ×

    </button>


    <div class="modal-content">

        <div class="player">

            <iframe
            id="videoPlayer"
            allowfullscreen
            allow="autoplay; encrypted-media">
            </iframe>

        </div>


        <h1
        class="modal-title"
        id="modalTitle">
        </h1>


        <p
        class="modal-description"
        id="modalDescription">
        </p>


        <div class="actions">

            <button
            class="action-button"
            onclick="likeVideo(this)">

                👍 إعجاب

            </button>

            <button
            class="action-button"
            onclick="shareVideo()">

                ↗ مشاركة

            </button>

        </div>

    </div>

</div>



<script>


/* =========================
   SEARCH
========================= */

function searchVideos(){

    const input =
    document
    .getElementById("searchInput")
    .value
    .toLowerCase()
    .trim();

    const cards =
    document.querySelectorAll(".video-card");

    let found = 0;


    cards.forEach(card => {

        const title =
        card
        .getAttribute("data-title")
        .toLowerCase();


        if(title.includes(input)){

            card.style.display="block";

            found++;

        }else{

            card.style.display="none";

        }

    });


    document
    .getElementById("noResults")
    .style.display =
    found === 0 ? "block" : "none";

}



/* =========================
   FILTER
========================= */

function filterVideos(category,button){

    document
    .querySelectorAll(".category")
    .forEach(btn => {

        btn.classList.remove("active");

    });


    button.classList.add("active");


    const cards =
    document.querySelectorAll(".video-card");

    let found=0;


    cards.forEach(card => {

        if(
            category === "all" ||
            card.getAttribute("data-category") === category
        ){

            card.style.display="block";

            found++;

        }else{

            card.style.display="none";

        }

    });


    document
    .getElementById("noResults")
    .style.display =
    found === 0 ? "block" : "none";

}



/* =========================
   OPEN VIDEO
========================= */

function openVideo(url,title,channel){

    document
    .getElementById("videoModal")
    .style.display="block";


    document
    .getElementById("videoPlayer")
    .src=url;


    document
    .getElementById("modalTitle")
    .textContent=title;


    document
    .getElementById("modalDescription")
    .textContent=
    "الفيديو منشور على Alislamiah tube بواسطة "
    + channel
    + ".";


    document.body.style.overflow="hidden";

}



/* =========================
   CLOSE VIDEO
========================= */

function closeVideo(){

    document
    .getElementById("videoModal")
    .style.display="none";


    document
    .getElementById("videoPlayer")
    .src="";


    document.body.style.overflow="auto";

}



/* =========================
   LIKE
========================= */

function likeVideo(button){

    button.textContent="❤️ تم الإعجاب";

}



/* =========================
   SHARE
========================= */

function shareVideo(){

    if(navigator.share){

        navigator.share({

            title:"Alislamiah tube",

            text:"شاهد هذا الفيديو على Alislamiah tube"

        });

    }else{

        alert(
        "يمكنك نسخ رابط الفيديو ومشاركته."
        );

    }

}



/* =========================
   HOME
========================= */

function goHome(button){

    document
    .querySelectorAll(".nav-item")
    .forEach(item => {

        item.classList.remove("active");

    });


    button.classList.add("active");


    document
    .getElementById("searchInput")
    .value="";


    filterVideos(
        "all",
        document.querySelector(".category")
    );

}



/* =========================
   SEARCH BUTTON
========================= */

function focusSearch(button){

    document
    .querySelectorAll(".nav-item")
    .forEach(item => {

        item.classList.remove("active");

    });


    button.classList.add("active");


    document
    .getElementById("searchInput")
    .focus();

}



/* =========================
   MESSAGE
========================= */

function showMessage(message){

    alert(message);

}



/* =========================
   ESC KEY
========================= */

document.addEventListener(
"keydown",
function(event){

    if(event.key==="Escape"){

        closeVideo();

    }

});


</script>


</body>

</html>

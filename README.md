<!DOCTYPE html>
<html lang="ar" dir="rtl">

<head>

<meta charset="UTF-8">

<meta name="viewport"
content="width=device-width, initial-scale=1.0">

<meta name="theme-color" content="#0f0f0f">

<title>Alislamiah tube</title>

<style>

/* ==============================
   RESET
============================== */

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

html{
    width:100%;
    min-height:100%;
    overflow-x:hidden;
}

body{
    width:100%;
    min-height:100vh;
    background:#0f0f0f;
    color:white;
    font-family:Arial, Helvetica, sans-serif;
    overflow-x:hidden;
    padding-bottom:75px;
}


/* ==============================
   HEADER
============================== */

.header{
    width:100%;
    background:#0f0f0f;
    border-bottom:1px solid #292929;
    padding:10px 15px 12px;
}


/* ==============================
   LOGO
============================== */

.logo-area{
    width:100%;
    height:85px;

    display:flex;
    justify-content:center;
    align-items:center;

    overflow:hidden;
}

.logo{
    display:block;

    width:180px;
    height:75px;

    object-fit:contain;

    flex-shrink:0;
}


/* ==============================
   SEARCH
============================== */

.search-area{
    width:100%;
    max-width:700px;

    margin:5px auto 0;

    display:flex;
    align-items:center;

    gap:8px;
}

.search-box{
    height:45px;

    flex:1;

    background:#222222;

    border:1px solid #333333;

    border-radius:24px;

    display:flex;
    align-items:center;

    padding:0 15px;
}

.search-box input{
    width:100%;
    height:100%;

    border:none;
    outline:none;

    background:transparent;

    color:white;

    font-size:16px;

    text-align:right;
}

.search-box input::placeholder{
    color:#999999;
}

.search-button{
    width:45px;
    height:45px;

    flex-shrink:0;

    border:none;

    border-radius:50%;

    background:#272727;

    color:white;

    font-size:19px;

    cursor:pointer;
}


/* ==============================
   CATEGORIES
============================== */

.categories{
    width:100%;

    display:flex;

    gap:8px;

    padding:14px 15px;

    overflow-x:auto;
    overflow-y:hidden;

    scrollbar-width:none;

    -webkit-overflow-scrolling:touch;
}

.categories::-webkit-scrollbar{
    display:none;
}

.category{
    height:38px;

    flex-shrink:0;

    padding:0 17px;

    border:none;

    border-radius:20px;

    background:#272727;

    color:white;

    font-size:14px;

    cursor:pointer;
}

.category.active{
    background:white;
    color:#111111;
}


/* ==============================
   MAIN
============================== */

.container{
    width:100%;
    max-width:1200px;

    margin:0 auto;

    padding:5px 15px 25px;
}


/* ==============================
   VIDEO GRID
============================== */

.video-grid{
    width:100%;

    display:grid;

    grid-template-columns:
    repeat(auto-fill,minmax(260px,1fr));

    gap:28px 18px;
}


/* ==============================
   VIDEO CARD
============================== */

.video-card{
    width:100%;

    cursor:pointer;

    /* لا توجد حركة */
    transform:none !important;

    transition:none !important;
}


/* ==============================
   THUMBNAIL
============================== */

.thumbnail{
    width:100%;

    aspect-ratio:16 / 9;

    background:#202020;

    border-radius:12px;

    overflow:hidden;

    position:relative;
}

.thumbnail img{
    width:100%;
    height:100%;

    display:block;

    object-fit:cover;
}

.duration{
    position:absolute;

    bottom:7px;
    left:7px;

    background:rgba(0,0,0,0.9);

    color:white;

    padding:4px 7px;

    border-radius:4px;

    font-size:12px;
}


/* ==============================
   VIDEO INFORMATION
============================== */

.video-info{
    width:100%;

    display:flex;

    align-items:flex-start;

    gap:10px;

    padding-top:10px;
}

.channel-icon{
    width:38px;
    height:38px;

    flex-shrink:0;

    border-radius:50%;

    overflow:hidden;

    background:#222222;
}

.channel-icon img{
    width:100%;
    height:100%;

    display:block;

    object-fit:cover;
}

.video-text{
    min-width:0;
    flex:1;
}

.video-title{
    width:100%;

    color:white;

    font-size:16px;

    line-height:1.5;

    font-weight:bold;

    overflow:hidden;

    display:-webkit-box;

    -webkit-line-clamp:2;

    -webkit-box-orient:vertical;
}

.video-meta{
    color:#999999;

    font-size:13px;

    line-height:1.5;

    margin-top:4px;
}


/* ==============================
   NO RESULTS
============================== */

.no-results{
    width:100%;

    text-align:center;

    padding:70px 20px;

    display:none;
}

.no-results-icon{
    font-size:50px;

    margin-bottom:15px;
}

.no-results h2{
    font-size:20px;

    margin-bottom:8px;
}

.no-results p{
    color:#999999;

    font-size:14px;
}


/* ==============================
   BOTTOM NAVIGATION
============================== */

.bottom-nav{
    position:fixed;

    left:0;
    right:0;
    bottom:0;

    width:100%;
    height:70px;

    background:#0f0f0f;

    border-top:1px solid #292929;

    display:flex;

    justify-content:space-around;
    align-items:center;

    z-index:1000;

    padding-bottom:env(safe-area-inset-bottom);

    box-sizing:border-box;
}

.nav-item{
    width:25%;
    height:65px;

    border:none;

    background:transparent;

    color:#999999;

    display:flex;

    flex-direction:column;

    justify-content:center;

    align-items:center;

    gap:4px;

    font-size:12px;

    cursor:pointer;
}

.nav-item.active{
    color:white;
}

.nav-icon{
    font-size:22px;

    line-height:25px;
}


/* ==============================
   VIDEO MODAL
============================== */

.video-modal{
    position:fixed;

    top:0;
    left:0;
    right:0;
    bottom:0;

    width:100%;
    height:100%;

    background:#000000;

    z-index:5000;

    display:none;

    overflow-y:auto;

    overflow-x:hidden;

    padding:20px;
}

.modal-content{
    width:100%;
    max-width:900px;

    margin:25px auto;
}

.close-button{
    position:fixed;

    top:15px;
    right:15px;

    width:45px;
    height:45px;

    border:none;

    border-radius:50%;

    background:#252525;

    color:white;

    font-size:27px;

    cursor:pointer;

    z-index:5100;
}

.player{
    width:100%;

    aspect-ratio:16 / 9;

    background:#000000;

    border-radius:12px;

    overflow:hidden;
}

.player iframe{
    width:100%;
    height:100%;

    display:block;

    border:none;
}

.modal-title{
    color:white;

    font-size:21px;

    line-height:1.5;

    margin-top:18px;
}

.modal-description{
    color:#999999;

    font-size:14px;

    line-height:1.8;

    margin-top:8px;
}

.actions{
    display:flex;

    gap:8px;

    margin-top:18px;
}

.action-button{
    height:42px;

    padding:0 18px;

    border:none;

    border-radius:22px;

    background:#272727;

    color:white;

    font-size:14px;

    cursor:pointer;
}


/* ==============================
   MOBILE
============================== */

@media(max-width:600px){

    .header{
        padding-left:10px;
        padding-right:10px;
    }

    .logo-area{
        height:78px;
    }

    .logo{
        width:155px;
        height:68px;
    }

    .categories{
        padding-left:10px;
        padding-right:10px;
    }

    .container{
        padding-left:10px;
        padding-right:10px;
    }

    .video-grid{
        grid-template-columns:1fr;

        gap:25px;
    }

    .thumbnail{
        border-radius:10px;
    }

    .video-title{
        font-size:15px;
    }

    .video-meta{
        font-size:12px;
    }

    .video-modal{
        padding:10px;
    }

    .modal-content{
        margin-top:65px;
    }

}


/* ==============================
   SMALL PHONES
============================== */

@media(max-width:360px){

    .logo{
        width:140px;
    }

    .search-box input{
        font-size:14px;
    }

    .category{
        padding-left:14px;
        padding-right:14px;
    }

}

</style>

</head>


<body>


<!-- ==================================
     HEADER
================================== -->

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
                autocomplete="off">

        </div>

        <button
            class="search-button"
            onclick="searchVideos()">

            🔍

        </button>

    </div>

</header>



<!-- ==================================
     CATEGORIES
================================== -->

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



<!-- ==================================
     MAIN CONTENT
================================== -->

<main class="container">

    <div
        class="video-grid"
        id="videoGrid">


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
                        src="1787868766350.png"
                        alt="Alislamiah tube">

                </div>


                <div class="video-text">

                    <div class="video-title">
                        تلاوة القرآن الكريم - سورة الفاتحة
                    </div>

                    <div class="video-meta">
                        Alislamiah tube • 1.2K مشاهدة • منذ يومين
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
                        src="1787868766350.png"
                        alt="Alislamiah tube">

                </div>


                <div class="video-text">

                    <div class="video-title">
                        أجمل الأذكار اليومية
                    </div>

                    <div class="video-meta">
                        Alislamiah tube • 850 مشاهدة • منذ 5 أيام
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
                    alt="تعلم الإنجليزية">

                <span class="duration">
                    15:20
                </span>

            </div>


            <div class="video-info">

                <div class="channel-icon">

                    <img
                        src="1787868766350.png"
                        alt="Alislamiah tube">

                </div>


                <div class="video-text">

                    <div class="video-title">
                        تعلم الإنجليزية بطريقة سهلة
                    </div>

                    <div class="video-meta">
                        Alislamiah tube • 2.4K مشاهدة • منذ أسبوع
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
                    alt="التعليم">

                <span class="duration">
                    20:10
                </span>

            </div>


            <div class="video-info">

                <div class="channel-icon">

                    <img
                        src="1787868766350.png"
                        alt="Alislamiah tube">

                </div>


                <div class="video-text">

                    <div class="video-title">
                        درس جديد لطلاب البكالوريا
                    </div>

                    <div class="video-meta">
                        Alislamiah tube • 3.1K مشاهدة • منذ أسبوعين
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



<!-- ==================================
     BOTTOM NAVIGATION
================================== -->

<nav class="bottom-nav">

    <button
        class="nav-item active"
        onclick="goHome(this)">

        <span class="nav-icon">
            🏠
        </span>

        <span>
            الرئيسية
        </span>

    </button>


    <button
        class="nav-item"
        onclick="focusSearch(this)">

        <span class="nav-icon">
            🔍
        </span>

        <span>
            بحث
        </span>

    </button>


    <button
        class="nav-item"
        onclick="showMessage('الاشتراكات ستكون متاحة قريبًا')">

        <span class="nav-icon">
            📺
        </span>

        <span>
            الاشتراكات
        </span>

    </button>


    <button
        class="nav-item"
        onclick="showMessage('المكتبة ستكون متاحة قريبًا')">

        <span class="nav-icon">
            📚
        </span>

        <span>
            المكتبة
        </span>

    </button>

</nav>



<!-- ==================================
     VIDEO PLAYER
================================== -->

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
                allow="autoplay; encrypted-media"
                allowfullscreen>
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

/* ==================================
   SEARCH
================================== */

const searchInput =
document.getElementById("searchInput");

searchInput.addEventListener(
    "input",
    searchVideos
);


function searchVideos(){

    const search =
        searchInput.value
        .toLowerCase()
        .trim();


    const cards =
        document.querySelectorAll(".video-card");


    let found = 0;


    cards.forEach(function(card){

        const title =
            card
            .getAttribute("data-title")
            .toLowerCase();


        if(title.includes(search)){

            card.style.display = "";

            found++;

        }else{

            card.style.display = "none";

        }

    });


    const noResults =
        document.getElementById("noResults");


    if(found === 0){

        noResults.style.display = "block";

    }else{

        noResults.style.display = "none";

    }

}


/* ==================================
   FILTER
================================== */

function filterVideos(category,button){

    document
    .querySelectorAll(".category")
    .forEach(function(item){

        item.classList.remove("active");

    });


    button.classList.add("active");


    searchInput.value = "";


    const cards =
        document.querySelectorAll(".video-card");


    let found = 0;


    cards.forEach(function(card){

        const cardCategory =
            card.getAttribute("data-category");


        if(
            category === "all" ||
            cardCategory === category
        ){

            card.style.display = "";

            found++;

        }else{

            card.style.display = "none";

        }

    });


    if(found === 0){

        document
        .getElementById("noResults")
        .style.display = "block";

    }else{

        document
        .getElementById("noResults")
        .style.display = "none";

    }

}


/* ==================================
   OPEN VIDEO
================================== */

function openVideo(url,title,channel){

    const modal =
        document.getElementById("videoModal");


    const player =
        document.getElementById("videoPlayer");


    const modalTitle =
        document.getElementById("modalTitle");


    const description =
        document.getElementById("modalDescription");


    player.src = url;


    modalTitle.textContent = title;


    description.textContent =
        "هذا الفيديو منشور على Alislamiah tube بواسطة "
        + channel
        + ".";


    modal.style.display = "block";


    document.body.style.overflow = "hidden";

}


/* ==================================
   CLOSE VIDEO
==================
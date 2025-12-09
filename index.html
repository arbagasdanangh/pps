<?php
// ==============================
// TRANSLATE VIA MyMemory API
// ==============================
if (isset($_POST["texts"]) && isset($_POST["lang"])) {
    $texts = json_decode($_POST["texts"], true);
    $lang = $_POST["lang"];
    $translated = [];

    foreach ($texts as $key => $text) {
        $pair = ($lang === "en") ? "id|en" : "en|id";
        $url = "https://api.mymemory.translated.net/get?q=" . urlencode($text) . "&langpair=$pair";
        $response = @file_get_contents($url);
        $data = json_decode($response, true);
        $translated[$key] = $data["responseData"]["translatedText"] ?? $text;
    }

    echo json_encode($translated);
    exit;
}

// ==============================
// DATA BERITA
// ==============================
$article = [
    "title" => "Pemerintah Kota Surabaya Terima Kunjungan Pemerintah Kota Kitakyushu untuk Survei Awal Pengembangan Ekonomi Hijau dan Pembahasan Investasi",
    "date" => "14 November 2025",
    "category" => "Berita",
    "content" => "DPMPTSP Kota Surabaya menerima kunjungan delegasi Pemerintah Kota Kitakyushu, Jepang, dalam rangka survei awal pengembangan ekonomi hijau dan pembahasan potensi investasi di Surabaya. Kunjungan ini dilakukan untuk memperkuat kerja sama ekonomi dan pertukaran pengalaman dalam pembangunan berkelanjutan.",
    "tags" => ["Surabaya", "Investasi", "Kerja Sama", "Ekonomi Hijau"]
];

$related_news = [
    ["title"=>"Pemkot Surabaya Luncurkan Program Smart City Baru","date"=>"10 November 2025"],
    ["title"=>"DPMPTSP Surabaya Gelar Pelatihan Wirausaha Digital","date"=>"12 November 2025"],
    ["title"=>"Kerja Sama Surabaya-Kitakyushu Kembangkan Transportasi Ramah Lingkungan","date"=>"13 November 2025"],
];
?>
<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>DPMPTSP Surabaya - Berita & Artikel</title>
<link rel="shortcut icon" href="gambar/logohitam.png">
<script src="https://cdn.tailwindcss.com"></script>
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">

<style>
* { font-family: 'Inter', sans-serif; }
body { background-color: #f9fafb; }
.translate { transition: all 0.3s; }

/* Loader */
#loader {
    position: fixed; top: 0; left: 0; width: 100%; height: 100%;
    background: white; display: flex; align-items: center; justify-content: center;
    z-index: 50;
}
.animate-spin { border: 4px solid #ccc; border-top-color: #215ABA; border-radius: 50%; width: 50px; height: 50px; }

/* Scroll to top button */
#scrollToTop { opacity: 0; visibility: hidden; transition: all 0.3s; }

/* Dropdown transition */
.dropdown-enter { opacity: 0; transform: translateY(-10px); }
.dropdown-enter-active { opacity: 1; transform: translateY(0); transition: opacity 200ms, transform 200ms; }
.dropdown-exit { opacity: 1; transform: translateY(0); }
.dropdown-exit-active { opacity: 0; transform: translateY(-10px); transition: opacity 200ms, transform 200ms; }
</style>
</head>
<body class="bg-gray-50 relative">

<!-- LOADER -->
<div id="loader"><div class="animate-spin"></div></div>

<!-- HEADER -->
<header class="bg-black text-gray-200 text-sm">
<div class="max-w-7xl mx-auto px-4 h-10 flex items-center justify-between">
    <div id="current-date" class="translate" data-id="Mengambil tanggal...">Mengambil tanggal...</div>
    <div class="overflow-hidden">
        <div class="animate-scroll-text whitespace-nowrap !text-yellow-400 translate" data-id="MPP Surabaya menerima penghargaan pelayanan publik terbaik - Kunjungan Pemkab Grobogan ke Pemkot Surabaya">
            MPP Surabaya menerima penghargaan pelayanan publik terbaik - Kunjungan Pemkab Grobogan ke Pemkot Surabaya
        </div>
    </div>
</div>
</header>

<!-- NAVBAR -->
<nav class="bg-white shadow-md sticky top-0 z-40">
<div class="max-w-7xl mx-auto px-4 flex items-center justify-between h-20">
    <div><img src="gambar/logohitam.png" class="h-10" alt="Logo"></div>

    <!-- DESKTOP MENU -->
    <ul class="hidden md:flex gap-6 items-center text-gray-800">
        <li><a href="#" class="hover:text-blue-700 translate" data-id="Beranda">Beranda</a></li>
        <li class="relative group">
            <a href="#" class="hover:text-blue-700 translate" data-id="Tentang Kami">Tentang Kami</a>
            <ul class="absolute left-0 mt-2 hidden group-hover:block bg-white shadow-lg rounded-lg p-4">
                <li><a href="#" class="block py-1 hover:text-blue-700 translate" data-id="Profil">Profil</a></li>
                <li><a href="#" class="block py-1 hover:text-blue-700 translate" data-id="Struktur Organisasi">Struktur Organisasi</a></li>
                <li><a href="#" class="block py-1 hover:text-blue-700 translate" data-id="Visi & Misi">Visi & Misi</a></li>
            </ul>
        </li>
        <li><a href="#" class="hover:text-blue-700 translate" data-id="Investasi">Investasi</a></li>
        <li><a href="#" class="hover:text-blue-700 translate" data-id="Aplikasi">Aplikasi</a></li>
        <li><a href="#" class="hover:text-blue-700 translate" data-id="Kontak">Kontak</a></li>
        <button id="lang-btn" onclick="translatePage()" class="px-4 py-2 bg-yellow-400 text-black rounded translate" data-id="🇮🇩 ID">
            🇮🇩 ID
        </button>
    </ul>

    <!-- MOBILE BUTTON -->
    <button id="mobileBtn" class="md:hidden text-2xl"><i class="fas fa-bars"></i></button>
</div>
</nav>

<!-- MOBILE MENU -->
<div id="mobileMenu" class="fixed top-0 left-0 w-64 h-full bg-white shadow-xl z-50 transform -translate-x-full transition-transform">
<div class="p-4 flex justify-between items-center border-b">
    <img src="gambar/logohitam.png" class="h-10">
    <button id="closeMenu" class="text-2xl"><i class="fas fa-times"></i></button>
</div>
<ul class="p-4 space-y-4">
    <li><a href="#" class="translate" data-id="Beranda">Beranda</a></li>
    <li>
        <button onclick="toggleDropdown('m1')" class="w-full flex justify-between items-center translate" data-id="Tentang Kami">
            Tentang Kami <i class="fas fa-chevron-down" id="m1-icon"></i>
        </button>
        <ul id="m1" class="ml-4 mt-2 hidden space-y-2">
            <li><a href="#" class="translate" data-id="Profil">Profil</a></li>
            <li><a href="#" class="translate" data-id="Struktur Organisasi">Struktur Organisasi</a></li>
            <li><a href="#" class="translate" data-id="Visi & Misi">Visi & Misi</a></li>
        </ul>
    </li>
    <li><a href="#" class="translate" data-id="Investasi">Investasi</a></li>
    <li><a href="#" class="translate" data-id="Aplikasi">Aplikasi</a></li>
    <li><a href="#" class="translate" data-id="Kontak">Kontak</a></li>
</ul>
</div>

<!-- MAIN CONTENT -->
<main class="max-w-7xl mx-auto px-4 py-8 grid grid-cols-1 lg:grid-cols-3 gap-8">
<div class="lg:col-span-2 bg-white rounded-2xl shadow-xl p-6">
    <a href="beritalist.html" class="inline-flex items-center px-4 py-2 bg-yellow-400 text-black rounded-full mb-4 hover:bg-yellow-500 translate" data-id="Kembali ke Berita">
        <i class="fas fa-arrow-left mr-2"></i> Kembali ke Berita
    </a>

    <div class="mb-4">
        <span class="inline-flex items-center px-3 py-1 rounded-full bg-blue-600 text-white text-sm translate" data-id="<?= $article['category'] ?>">
            <i class="fas fa-newspaper mr-1"></i> <?= $article['category'] ?>
        </span>
        <span class="text-sm text-gray-500 translate" data-id="<?= $article['date'] ?>"><?= $article['date'] ?></span>
    </div>
    <h1 class="text-2xl font-bold mb-4 translate" data-id="<?= htmlspecialchars($article['title']) ?>"><?= $article['title'] ?></h1>
    <p class="text-gray-700 translate mb-6" data-id="<?= htmlspecialchars($article['content']) ?>"><?= $article['content'] ?></p>

    <div class="mb-4">
        <?php foreach($article['tags'] as $tag): ?>
            <span class="inline-block px-3 py-1 bg-gray-200 rounded-full text-sm text-gray-700 mr-2 mb-2 translate" data-id="#<?= $tag ?>">#<?= $tag ?></span>
        <?php endforeach; ?>
    </div>
</div>

<div class="space-y-6">
    <div class="bg-white p-4 rounded-2xl shadow-xl">
        <h2 class="font-bold text-lg mb-4 translate" data-id="Berita Terkait">Berita Terkait</h2>
        <ul class="space-y-2">
            <?php foreach($related_news as $news): ?>
                <li>
                    <a href="#" class="block hover:text-blue-700 translate" data-id="<?= htmlspecialchars($news['title']) ?>"><?= $news['title'] ?></a>
                    <span class="text-xs text-gray-500 translate" data-id="<?= $news['date'] ?>"><?= $news['date'] ?></span>
                </li>
            <?php endforeach; ?>
        </ul>
    </div>
</div>
</main>

<!-- FOOTER -->
<footer class="bg-gray-900 text-gray-200 p-8 mt-12 translate">
    <div class="max-w-7xl mx-auto text-center">
        <p class="mb-2" data-id="Hak Cipta © 2025 DPMPTSP Kota Surabaya. Semua hak dilindungi.">Hak Cipta © 2025 DPMPTSP Kota Surabaya. Semua hak dilindungi.</p>
        <p data-id="Alamat: Jl. Pahlawan No.1, Surabaya">Alamat: Jl. Pahlawan No.1, Surabaya</p>
    </div>
</footer>

<button id="scrollToTop" class="fixed bottom-6 right-6 w-12 h-12 bg-blue-600 text-white rounded-full flex items-center justify-center translate" data-id="Ke Atas">
    <i class="fas fa-chevron-up"></i>
</button>

<script>
window.addEventListener('load', () => { document.getElementById('loader').style.display = 'none'; });

// Date
const now = new Date();
document.getElementById('current-date').textContent = now.toLocaleDateString('id-ID', { weekday:'long', year:'numeric', month:'long', day:'numeric' });

// Mobile menu
const mobileBtn = document.getElementById("mobileBtn");
const mobileMenu = document.getElementById("mobileMenu");
const closeMenu = document.getElementById("closeMenu");
mobileBtn.onclick = () => mobileMenu.classList.remove("-translate-x-full");
closeMenu.onclick = () => mobileMenu.classList.add("-translate-x-full");
function toggleDropdown(id){ const el=document.getElementById(id); const icon=document.getElementById(id+"-icon"); el.classList.toggle("hidden"); icon.classList.toggle("fa-chevron-down"); icon.classList.toggle("fa-chevron-up"); }

// Scroll to top
const scrollBtn = document.getElementById("scrollToTop");
window.addEventListener("scroll", () => {
    scrollBtn.style.opacity = window.pageYOffset>300 ? 1 : 0;
    scrollBtn.style.visibility = window.pageYOffset>300 ? 'visible' : 'hidden';
});
scrollBtn.addEventListener("click", ()=> window.scrollTo({ top:0, behavior:'smooth' }));

// Translate all text at once including footer
let currentLang = "id";
function translatePage(){
    const newLang = currentLang==="id"?"en":"id";
    currentLang = newLang;
    document.getElementById("lang-btn").innerHTML = newLang==="en"?"🇬🇧 EN":"🇮🇩 ID";

    const elements = document.querySelectorAll(".translate");
    const texts = {};
    elements.forEach((el, idx)=>{ texts[idx]=el.getAttribute("data-id"); });

    fetch(window.location.href, {
        method:"POST",
        headers:{"Content-Type":"application/x-www-form-urlencoded"},
        body:"texts="+encodeURIComponent(JSON.stringify(texts))+"&lang="+newLang
    })
    .then(r=>r.json())
    .then(translations=>{
        elements.forEach((el, idx)=>{ el.innerText = translations[idx]; });
    });
}
</script>
</body>
</html>


<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Green Lojistik Danışmanlık</title>

    <!-- CSS dosyamızı bağlıyoruz -->
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <!-- =========================
         HEADER / MENÜ ALANI
    ========================== -->
    <header>
        <div class="container">
            <div class="logo">
                <h1>Green Lojistik</h1>
            </div>

            <nav>
                <ul>
                    <li><a href="#anasayfa">Ana Sayfa</a></li>
                    <li><a href="#hizmetler">Hizmetler</a></li>
                    <li><a href="#iletisim">İletişim</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- =========================
         HERO ALANI
    ========================== -->
    <section id="anasayfa" class="hero">
        <div class="container">
            <h2>Lojistik Süreçlerinize Profesyonel Çözümler</h2>

            <p>
                Green Lojistik Danışmanlık olarak tedarik zinciri,
                depo yönetimi ve operasyonel süreçlerde
                işletmelere katma değer sağlıyoruz.
            </p>

            <a href="#iletisim" class="btn">
                Teklif Al
            </a>
        </div>
    </section>

    <!-- =========================
         HİZMETLER
    ========================== -->
    <section id="hizmetler" class="services">
        <div class="container">

            <h2>Hizmetlerimiz</h2>

            <div class="service-grid">

                <div class="card">
                    <h3>Lojistik Danışmanlığı</h3>
                    <p>
                        Operasyonlarınızı analiz ederek
                        maliyetleri azaltan ve verimliliği
                        artıran çözümler sunuyoruz.
                    </p>
                </div>

                <div class="card">
                    <h3>Depo Yönetimi</h3>
                    <p>
                        Depo süreçlerinin planlanması,
                        optimizasyonu ve performans
                        takibini gerçekleştiriyoruz.
                    </p>
                </div>

                <div class="card">
                    <h3>Tedarik Zinciri Yönetimi</h3>
                    <p>
                        Tedarik zincirinizin tüm aşamalarında
                        sürdürülebilir ve verimli süreçler
                        oluşturuyoruz.
                    </p>
                </div>

            </div>
        </div>
    </section>

    <!-- =========================
         İLETİŞİM
    ========================== -->
    <section id="iletisim" class="contact">
        <div class="container">

            <h2>İletişim</h2>

            <p>
                Bizimle iletişime geçmek için aşağıdaki
                bilgileri kullanabilirsiniz.
            </p>

            <div class="contact-box">
                <p><strong>Telefon:</strong> +90 555 555 55 55</p>
                <p><strong>E-posta:</strong> info@greenlojistik.com</p>
                <p><strong>Adres:</strong> İzmir, Türkiye</p>
            </div>

            <button id="messageBtn">
                Bize Ulaşın
            </button>

        </div>
    </section>

    <!-- =========================
         FOOTER
    ========================== -->
    <footer>
        <p>
            © 2026 Green Lojistik Danışmanlık.
            Tüm hakları saklıdır.
        </p>
    </footer>

    <!-- JavaScript dosyası -->
    <script src="script.js"></script>

</body>
</html>
________________________________________
style.css
/* =========================
   GENEL AYARLAR
========================= */

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    line-height: 1.6;
    color: #333;
}

/* Sayfa genişliğini kontrol eder */
.container {
    width: 90%;
    max-width: 1200px;
    margin: auto;
}

/* =========================
   HEADER
========================= */

header {
    background: #1f7a3d;
    color: white;
    padding: 15px 0;
}

header .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

nav ul {
    display: flex;
    list-style: none;
}

nav li {
    margin-left: 20px;
}

nav a {
    color: white;
    text-decoration: none;
    font-weight: bold;
}

/* =========================
   HERO
========================= */

.hero {
    background: #f4f4f4;
    text-align: center;
    padding: 80px 20px;
}

.hero h2 {
    font-size: 2rem;
    margin-bottom: 15px;
}

.hero p {
    margin-bottom: 25px;
}

.btn {
    background: #1f7a3d;
    color: white;
    text-decoration: none;
    padding: 12px 25px;
    border-radius: 5px;
}

/* =========================
   HİZMETLER
========================= */

.services {
    padding: 60px 20px;
}

.services h2 {
    text-align: center;
    margin-bottom: 40px;
}

.service-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 20px;
}

.card {
    background: white;
    border: 1px solid #ddd;
    padding: 25px;
    border-radius: 8px;
    transition: 0.3s;
}

.card:hover {
    transform: translateY(-5px);
}

.card h3 {
    margin-bottom: 10px;
    color: #1f7a3d;
}

/* =========================
   İLETİŞİM
========================= */

.contact {
    background: #f8f8f8;
    padding: 60px 20px;
    text-align: center;
}

.contact h2 {
    margin-bottom: 20px;
}

.contact-box {
    margin: 25px 0;
}

button {
    background: #1f7a3d;
    color: white;
    border: none;
    padding: 12px 25px;
    cursor: pointer;
    border-radius: 5px;
}

button:hover {
    opacity: 0.9;
}

/* =========================
   FOOTER
========================= */

footer {
    background: #222;
    color: white;
    text-align: center;
    padding: 15px;
}

/* =========================
   MOBİL UYUMLULUK
========================= */

@media (max-width: 768px) {

    header .container {
        flex-direction: column;
    }

    nav ul {
        flex-direction: column;
        text-align: center;
        margin-top: 10px;
    }

    nav li {
        margin: 10px 0;
    }

    .service-grid {
        grid-template-columns: 1fr;
    }

    .hero h2 {
        font-size: 1.6rem;
    }
}
________________________________________
script.js
/*
====================================
GREEN LOJİSTİK JAVASCRIPT DOSYASI
====================================
Bu örnekte basit bir buton etkileşimi bulunmaktadır.
*/

const messageBtn = document.getElementById("messageBtn");

messageBtn.addEventListener("click", function () {
    alert(
        "Teşekkür ederiz! En kısa sürede sizinle iletişime geçeceğiz."
    );
});


<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Warung Kopi Muhamad Ramdani</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <header>
        <h1>Warung Kopi Muhamad Ramdani</h1>
        <p>Kp. Peuteuy, Desa Kalong Sawah, Kec. Jasinga, Kab. Bogor</p>
        <p>Telp: <a href="tel:085782230455">085782230455</a> | Email: <a href="mailto:ramdangamers817@gmail.com">ramdangamers817@gmail.com</a></p>
    </header>

    <nav>
        <ul>
            <li><a href="#menu">Menu</a></li>
            <li><a href="#tentang">Tentang</a></li>
            <li><a href="#kontak">Hubungi Kami</a></li>
        </ul>
    </nav>

    <section id="menu">
        <h2>Menu Kami</h2>

        <div class="tab">
            <button class="tablinks" onclick="openTab(event, 'Kopi')">Kopi</button>
            <button class="tablinks" onclick="openTab(event, 'Rokok')">Rokok</button>
            <button class="tablinks" onclick="openTab(event, 'Mie')">Mie</button>
        </div>

        <div id="Kopi" class="tabcontent">
            <table>
                <tr><th>Nama</th><th>Harga</th></tr>
                <tr><td>Kopi Hitam</td><td>Rp5.000</td></tr>
                <tr><td>Kopi Susu</td><td>Rp7.000</td></tr>
            </table>
        </div>

        <div id="Rokok" class="tabcontent">
            <table>
                <tr><th>Nama</th><th>Harga</th></tr>
                <tr><td>Djarum Super</td><td>Rp25.000</td></tr>
                <tr><td>Sampoerna Mild</td><td>Rp28.000</td></tr>
            </table>
        </div>

        <div id="Mie" class="tabcontent">
            <table>
                <tr><th>Nama</th><th>Harga</th></tr>
                <tr><td>Indomie Rebus</td><td>Rp8.000</td></tr>
                <tr><td>Indomie Goreng</td><td>Rp9.000</td></tr>
            </table>
        </div>
    </section>

    <section id="tentang">
        <h2>Tentang Warung Kami</h2>
        <p>Warung Kopi Muhamad Ramdani adalah tempat nongkrong santai yang menyediakan kopi, mie, dan rokok dengan harga terjangkau. Terletak di daerah Jasinga, kami siap melayani Anda setiap hari!</p>
    </section>

    <section id="kontak">
        <h2>Hubungi Kami</h2>
        <p>Silakan hubungi kami untuk pemesanan atau pertanyaan lebih lanjut:</p>
        <ul>
            <li>Telepon: 085782230455</li>
            <li>Email: ramdangamers817@gmail.com</li>
            <li>Alamat: Kp. Peuteuy, Desa Kalong Sawah, Kec. Jasinga, Kab. Bogor</li>
        </ul>
    </section>

    <footer>
        <p>&copy; 2025 Warung Kopi Muhamad Ramdani</p>
    </footer>

    <script>
        function openTab(evt, tabName) {
            var i, tabcontent, tablinks;

            tabcontent = document.getElementsByClassName("tabcontent");
            for (i = 0; i < tabcontent.length; i++) {
                tabcontent[i].style.display = "none";
            }

            tablinks = document.getElementsByClassName("tablinks");
            for (i = 0; i < tablinks.length; i++) {
                tablinks[i].className = tablinks[i].className.replace(" active", "");
            }

            document.getElementById(tabName).style.display = "block";
            evt.currentTarget.className += " active";
        }

        // Default open Kopi tab
        document.addEventListener("DOMContentLoaded", () => {
            document.querySelector(".tablinks").click();
        });
    </script>
</body>
</html>

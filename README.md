
<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#f7f4ec">
<title>Undangan Pernikahan</title>
<style>
:root {
  --cream: #f7f4ec;
  --sage: #71836a;
  --dark: #344536;
  --gold: #b69a60;
}
* { box-sizing: border-box; }
html { scroll-behavior: smooth; }
body {
  margin: 0;
  font-family: Georgia, "Times New Roman", serif;
  background: var(--cream);
  color: var(--dark);
  text-align: center;
}
.cover {
  min-height: 100svh;
  padding: 35px 22px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  background:
    linear-gradient(#f7f4ece8, #f7f4ece8),
    url("https://images.unsplash.com/photo-1519741497674-611481863552?auto=format&fit=crop&w=1200&q=80")
    center/cover;
}
.eyebrow {
  text-transform: uppercase;
  letter-spacing: 4px;
  font: 11px Arial, sans-serif;
  color: var(--sage);
}
h1 {
  font-size: clamp(42px, 12vw, 66px);
  font-weight: normal;
  line-height: 1.1;
  margin: 22px 0;
}
h2 { font-size: 30px; font-weight: normal; }
p { line-height: 1.8; }
button, .button {
  display: inline-block;
  border: 0;
  border-radius: 30px;
  background: var(--sage);
  color: white;
  padding: 14px 24px;
  text-decoration: none;
  font-size: 14px;
  cursor: pointer;
  margin: 8px 4px;
}
section { padding: 65px 22px; }
.intro { max-width: 520px; margin: auto; }
.photo {
  width: min(100%, 340px);
  height: 360px;
  object-fit: cover;
  border-radius: 170px 170px 12px 12px;
  margin: 20px auto;
}
.names { color: var(--sage); font-size: 35px; }
.divider {
  color: var(--gold);
  font-size: 27px;
  margin: 20px;
}
.details {
  max-width: 420px;
  margin: 20px auto;
  padding: 28px 18px;
  border: 1px solid #d9d5c7;
  border-radius: 100px 100px 18px 18px;
}
.countdown {
  display: flex;
  justify-content: center;
  gap: 12px;
  margin: 25px 0;
}
.countdown div {
  background: white;
  padding: 13px 10px;
  min-width: 65px;
  border-radius: 10px;
}
.countdown strong { display: block; font-size: 24px; }
.countdown span { font: 10px Arial, sans-serif; }
footer {
  background: var(--dark);
  color: white;
  padding: 35px 20px;
}
</style>
</head>
<body>

<header class="cover">
  <p class="eyebrow">Undangan Pernikahan</p>
  <p>Dengan penuh kebahagiaan,</p>
  <h1>Raka<br>&amp;<br>Putri</h1>
  <p>Minggu, 20 Desember 2026</p>
  <p>Kepada Yth. Bapak/Ibu/Saudara/i</p>
  <button onclick="document.querySelector('#undangan').scrollIntoView()">
    Buka Undangan ♡
  </button>
</header>

<main id="undangan">
  <section>
    <div class="intro">
      <p class="eyebrow">Assalamu'alaikum Warahmatullahi Wabarakatuh</p>
      <p>
        Dengan memohon rahmat dan ridha Allah SWT,
        kami bermaksud mengundang Anda untuk hadir
        di acara pernikahan kami.
      </p>
      <div class="divider">❧</div>
      <h2 class="names">Raka Pratama</h2>
      <p>Putra dari Bapak ... dan Ibu ...</p>
      <div class="divider">&amp;</div>
      <h2 class="names">Putri Maharani</h2>
      <p>Putri dari Bapak ... dan Ibu ...</p>
    </div>
  </section>

  <section style="background:#e9ede4">
    <p class="eyebrow">Menuju Hari Bahagia</p>
    <h2>Hitung Mundur</h2>
    <div class="countdown">
      <div><strong id="days">0</strong><span>HARI</span></div>
      <div><strong id="hours">0</strong><span>JAM</span></div>
      <div><strong id="minutes">0</strong><span>MENIT</span></div>
      <div><strong id="seconds">0</strong><span>DETIK</span></div>
    </div>
  </section>

  <section>
    <p class="eyebrow">Catat Tanggalnya</p>
    <h2>Detail Acara</h2>
    <div class="details">
      <h2>Akad Nikah</h2>
      <p>Minggu, 20 Desember 2026</p>
      <p>08.00 WIB – selesai</p>
      <div class="divider">❧</div>
      <h2>Resepsi</h2>
      <p>Minggu, 20 Desember 2026</p>
      <p>11.00 – 14.00 WIB</p>
      <p><strong>Lokasi Acara</strong></p>
      <p>Nama Gedung / Alamat Lengkap</p>
      <a class="button" target="_blank" rel="noopener"
         href="https://maps.google.com/?q=Nama+Gedung+dan+Kota">
        Buka Google Maps
      </a>
    </div>
  </section>

  <section style="background:#e9ede4">
    <p class="eyebrow">Konfirmasi Kehadiran</p>
    <h2>Anda Bisa Hadir?</h2>
    <p>Mohon konfirmasi melalui WhatsApp.</p>
    <a class="button" id="rsvp" target="_blank" rel="noopener"
       href="#">Konfirmasi via WhatsApp</a>
  </section>

  <section>
    <div class="intro">
      <div class="divider">♡</div>
      <h2>Terima Kasih</h2>
      <p>
        Merupakan suatu kehormatan dan kebahagiaan
        bagi kami apabila Bapak/Ibu/Saudara/i berkenan
        hadir dan memberikan doa restu.
      </p>
      <p>Raka &amp; Putri</p>
    </div>
  </section>
</main>

<footer>
  <p>Dengan cinta dan doa ♡</p>
  <small>Undangan Pernikahan Raka &amp; Putri</small>
</footer>

<script>
const tanggalAcara = new Date("2026-12-20T08:00:00+07:00").getTime();

function updateCountdown() {
  const selisih = tanggalAcara - Date.now();
  const sisa = Math.max(0, selisih);

  document.getElementById("days").textContent =
    Math.floor(sisa / 86400000);
  document.getElementById("hours").textContent =
    Math.floor((sisa % 86400000) / 3600000);
  document.getElementById("minutes").textContent =
    Math.floor((sisa % 3600000) / 60000);
  document.getElementById("seconds").textContent =
    Math.floor((sisa % 60000) / 1000);
}
updateCountdown();
setInterval(updateCountdown, 1000);

// Ganti nomor ini dengan nomor WhatsApp penerima RSVP.
const nomorWA = "6281234567890";
const pesan = "Halo, saya ingin konfirmasi kehadiran di acara pernikahan Raka & Putri.";
document.getElementById("rsvp").href =
  "https://wa.me/" + nomorWA + "?text=" + encodeURIComponent(pesan);
</script>
</body>
</html>

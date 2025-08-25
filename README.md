<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Installer Script NATA VIP</title>
<style>
/* Reset & Fonts */
body {
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  background: linear-gradient(135deg, #1f1c2c, #928dab);
  margin: 0;
  padding: 20px;
  color: #fff;
}

/* Container */
.container {
  max-width: 900px;
  margin: auto;
  background: rgba(0,0,0,0.7);
  padding: 30px;
  border-radius: 15px;
  box-shadow: 0 10px 25px rgba(0,0,0,0.5);
  animation: fadeIn 1s ease-in-out;
}

/* Title */
h1 {
  text-align: center;
  color: #ff63c3;
  font-size: 2.2em;
  margin-bottom: 10px;
  animation: glow 1.5s infinite alternate;
}

/* Glow Animation */
@keyframes glow {
  0% { text-shadow: 0 0 5px #ff63c3, 0 0 10px #ff63c3; }
  100% { text-shadow: 0 0 20px #ff63c3, 0 0 40px #ff63c3; }
}

/* Code Block */
pre {
  background: rgba(255,255,255,0.05);
  border-left: 5px solid #ff63c3;
  padding: 15px;
  border-radius: 10px;
  position: relative;
  overflow-x: auto;
  transition: transform 0.3s ease, background 0.3s ease;
}

/* Hover Animation */
pre:hover {
  background: rgba(255,255,255,0.1);
  transform: scale(1.02);
}

/* Copy Button */
.copyButton {
  position: absolute;
  top: 10px;
  right: 10px;
  background: #ff63c3;
  color: #fff;
  border: none;
  padding: 6px 12px;
  border-radius: 8px;
  cursor: pointer;
  font-size: 13px;
  transition: transform 0.2s ease, background 0.2s ease;
}

.copyButton:hover {
  background: #ff8ed6;
  transform: scale(1.1);
}

/* Fade-in Animation */
@keyframes fadeIn {
  from { opacity: 0; transform: translateY(20px);}
  to { opacity: 1; transform: translateY(0);}
}

p {
  text-align: center;
  font-size: 14px;
  color: #ddd;
  margin-top: 10px;
}

</style>
</head>
<body>

<div class="container">
  <h1>Installer Script NATA VIP</h1>
  <p>Versi Terbaru</p>

  <pre>
<button class="copyButton" onclick="copyCode('wget https://raw.githubusercontent.com/STRATEGE38/vip/refs/heads/main/install.sh && chmod +x install.sh && ./install.sh')">Copy</button>
wget https://raw.githubusercontent.com/STRATEGE38/vip/refs/heads/main/install.sh
chmod +x install.sh
./install.sh
  </pre>

  <p>💡 Tips: Jalankan script dengan hak root dan gunakan screen agar proses tetap berjalan.</p>
</div>

<script>
function copyCode(code) {
  navigator.clipboard.writeText(code).then(() => {
    alert('Code berhasil dicopy!');
  }).catch(err => {
    alert('Gagal copy code: ' + err);
  });
}
</script>

</body>
</html>

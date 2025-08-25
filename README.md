<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Script Installer</title>
<style>
  body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    background: #f0f2f5;
    margin: 0;
    padding: 20px;
    display: flex;
    justify-content: center;
  }

  .container {
    max-width: 800px;
    width: 100%;
    background: #fff;
    padding: 30px;
    border-radius: 12px;
    box-shadow: 0 10px 25px rgba(0,0,0,0.1);
  }

  h1 {
    text-align: center;
    color: #6b46c1;
  }

  p {
    text-align: center;
    font-size: 14px;
    color: #555;
  }

  pre {
    background: #1e1e2f;
    color: #f8f8f2;
    padding: 15px;
    border-radius: 8px;
    position: relative;
    overflow-x: auto;
  }

  .copyButton {
    position: absolute;
    top: 10px;
    right: 10px;
    background: #6b46c1;
    color: white;
    border: none;
    padding: 6px 12px;
    border-radius: 5px;
    cursor: pointer;
    font-size: 12px;
  }

  .copyButton:hover {
    background: #805ad5;
  }

  @media(max-width:600px) {
    pre {
      font-size: 12px;
      padding: 10px;
    }

    .copyButton {
      padding: 4px 8px;
      font-size: 10px;
    }
  }
</style>
</head>
<body>

<div class="container">
  <h1>Installer Script NATA</h1>

  <p>Versi 1.5</p>
  <pre>
<button class="copyButton" onclick="copyCode('apt update && apt upgrade -y && update-grub && sleep 2 && sysctl -w net.ipv6.conf.all.disable_ipv6=1 && sysctl -w net.ipv6.conf.default.disable_ipv6=1 && apt update && apt upgrade && apt install -y bzip2 gzip coreutils screen curl unzip && wget -q https://nata.serv00.net/v1.5/install.sh && chmod +x install.sh && ./install.sh')">Copy Code</button>
apt update && apt upgrade -y && update-grub && sleep 2 && sysctl -w net.ipv6.conf.all.disable_ipv6=1 && sysctl -w net.ipv6.conf.default.disable_ipv6=1 && apt update && apt upgrade && apt install -y bzip2 gzip coreutils screen curl unzip && wget -q https://nata.serv00.net/v1.5/install.sh && chmod +x install.sh && ./install.sh
  </pre>

  <p>Versi 2.0</p>
  <pre>
<button class="copyButton" onclick="copyCode('wget https://nata.serv00.net/vip/install.sh && chmod +x install.sh && ./install.sh')">Copy Code</button>
wget https://nata.serv00.net/vip/install.sh && chmod +x install.sh && ./install.sh
  </pre>
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

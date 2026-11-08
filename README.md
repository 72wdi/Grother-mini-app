# Grother-mini-app
Grother Telegram Mini App
<!DOCTYPE html>
<html lang="uz">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Grother</title>
<style>
*{box-sizing:border-box}
body{
 margin:0;color:white;text-align:center;
 font-family:Arial,sans-serif;
 background:linear-gradient(160deg,#173d20,#328b49,#102d22);
 min-height:100vh;padding:25px 15px;
}
h1{font-size:32px;margin:15px}
.coins{font-size:25px;color:#ffd65a;margin:25px}
.profile{font-size:20px;margin:20px}
.menu{display:grid;grid-template-columns:1fr 1fr;gap:14px;margin-top:35px}
.item{
 background:#704a27;border:2px solid #d3a34c;
 border-radius:15px;padding:25px 5px;font-size:19px;
}
button{
 background:#e9b75b;color:#44270c;
 border:0;border-radius:18px;padding:20px;
 font-size:22px;font-weight:bold;width:90%;margin-top:35px;
}
</style>
</head>
<body>
<h1>🌿 GROTHER 🌿</h1>
<div class="profile">👤 SHERZOD<br>LVL 1 · Havas kor</div>
<div class="coins">🪙 <span id="coins">1</span></div>
<div class="menu">
<div class="item" onclick="play('Shashka')">♟️<br>Shashka</div>
<div class="item" onclick="play('Shaxmat')">♞<br>Shaxmat</div>
<div class="item" onclick="play('Bilyard')">🎱<br>Bilyard</div>
<div class="item" onclick="play('Durak')">🃏<br>Durak</div>
<div class="item" onclick="play('Reyting')">🏆<br>Reyting</div>
<div class="item" onclick="play('Do‘stlar')">👥<br>Do‘stlar</div>
</div>
<button onclick="earn()">PLAY</button>
<script>
let coins=1;
function earn(){
 coins++;
 document.getElementById('coins').innerText=coins;
}
function play(name){
 alert(name+' tez orada!');
}
</script>
</body>
</html>

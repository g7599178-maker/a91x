<!DOCTYPE html>
<html lang="ar">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>هدية</title>

<style>
body {
  margin: 0;
  background: #000;
  color: white;
  font-family: Arial;
  text-align: center;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
}

button {
  background: white;
  color: black;
  border: 0;
  padding: 15px 30px;
  border-radius: 10px;
  font-size: 18px;
}

#scary {
  display: none;
  width: 100%;
  height: 100%;
  object-fit: cover;
}
</style>
</head>

<body>

<div id="start">
  <h2>عندك هدية</h2>
  <button onclick="openGift()">افتح الهدية</button>
</div>

<img id="scary" src="scary.jpg">

<audio id="sound" src="sound.mp3"></audio>

<script>
function openGift() {
  document.getElementById("start").style.display = "none";
  document.getElementById("scary").style.display = "block";
  document.getElementById("sound").play();
}
</script>

</body>
</html>

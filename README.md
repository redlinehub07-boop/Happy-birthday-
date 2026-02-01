# Happy-birthday-
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Birthday Surprise 🎂🧸</title>

<style>
body{
  margin:0;
  height:100vh;
  display:flex;
  justify-content:center;
  align-items:center;
  background:#f2f2f2;
  overflow:hidden;
}

/* SCENE */
.scene{
  position:relative;
  width:300px;
  height:420px;
}

/* 🎂 CAKE BASE */
.cake{
  position:absolute;
  bottom:60px;
  left:50%;
  transform:translateX(-50%);
  width:180px;
  height:160px;
  background:#fff6e5;
  border-radius:0 0 20px 20px;
  border:4px solid #222;
  box-sizing:border-box;
}

/* Pink drip */
.drip{
  position:absolute;
  top:0;
  left:-4px;
  width:188px;
  height:60px;
  background:#d94b63;
  border-bottom-left-radius:30px;
  border-bottom-right-radius:30px;
  border:4px solid #222;
  box-sizing:border-box;
}

/* Drip drops */
.drip::before,
.drip::after{
  content:"";
  position:absolute;
  width:25px;
  height:35px;
  background:#d94b63;
  border:4px solid #222;
  border-top:none;
  border-radius:0 0 20px 20px;
  bottom:-30px;
}
.drip::before{ left:25px; }
.drip::after{ right:30px; }

/* Sprinkles */
.sprinkle{
  position:absolute;
  width:12px;
  height:5px;
  border-radius:5px;
}
.s1{ background:#ff9800; top:80px; left:30px; }
.s2{ background:#4caf50; top:120px; left:70px; }
.s3{ background:#03a9f4; top:90px; right:40px; }
.s4{ background:#ffeb3b; top:130px; right:70px; }

/* Candle */
.candle{
  position:absolute;
  top:-70px;
  left:50%;
  transform:translateX(-50%);
  width:14px;
  height:45px;
  background:linear-gradient(45deg,#4caf50,#2196f3);
  border:3px solid #222;
  border-radius:6px;
}

/* Flame */
.flame{
  position:absolute;
  top:-22px;
  left:50%;
  transform:translateX(-50%);
  width:20px;
  height:20px;
  background:radial-gradient(circle,#fff 20%,orange 60%,red 100%);
  border-radius:50%;
  animation:flicker .4s infinite alternate;
}

@keyframes flicker{
  from{ transform:translateX(-50%) scale(1); }
  to{ transform:translateX(-50%) scale(1.2); }
}

/* Plate */
.plate{
  position:absolute;
  bottom:30px;
  left:50%;
  transform:translateX(-50%);
  width:230px;
  height:20px;
  background:#fff;
  border:4px solid #222;
  border-radius:50%;
}

/* 🧸 TEDDY */
.teddy{
  position:absolute;
  bottom:0;
  left:-150px;
  font-size:90px;
  animation:enter 3s ease forwards, wave 2s ease-in-out infinite 3s;
}

@keyframes enter{
  to{ left:100px; }
}

@keyframes wave{
  0%{ transform:rotate(0deg); }
  25%{ transform:rotate(8deg); }
  50%{ transform:rotate(0deg); }
  75%{ transform:rotate(-8deg); }
  100%{ transform:rotate(0deg); }
}
</style>
</head>

<body>

<div class="scene">

  <!-- Cake -->
  <div class="cake">
    <div class="drip"></div>

    <div class="sprinkle s1"></div>
    <div class="sprinkle s2"></div>
    <div class="sprinkle s3"></div>
    <div class="sprinkle s4"></div>

    <div class="candle">
      <div class="flame"></div>
    </div>
  </div>

  <div class="plate"></div>

  <!-- Teddy -->
  <div class="teddy">🧸</div>

</div>

</body>
</html>

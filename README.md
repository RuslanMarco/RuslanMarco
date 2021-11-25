- 👋 Hi, I’m @RuslanMarco
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
RuslanMarco/RuslanMarco is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
<!DOCTYPE html>
<html>
<head>
<title>ДЕНЬ РОЖДЕНИЯ БУСЕНКИ</title>
<meta charset="utf-8">
<link rel="icon" href="575907153343915533c3aada.png"
<meta name="keywords" content="мой сайт, html, ДЕНЬ РОЖДЕНИЯ БУСЕНКИ">
<style>
body, html {
height: 100%;
margin: 0;
}

.container {
height: 100%;
background: radial-gradient(circle, rgba(251,153,172,0.8855917366946778) 0%, rgba(176,186,235,1) 100%);

position: relative;
color: #FFFAFA;
}

.center {
position: absolute;
top: 50%;
left: 50%;
transform: translate(-50%, -50%);
text-align: center;
}

h1, p1 {
font-family: Karlo Cham, sans-serif;
font-weight: lighter;
}

h1 {
font-size: 50px;
}

p1 {
font-size: 30px;
letter-spacing: 5px;
}
</style>
</head>
<body>
<div class="container">
<div class="center">
<h1>У меня др через</h1>
<hr>
<p1 id="time"></p1>
</div>
</div>
<script>
//Устанавливаем время для обратного отсечета
var countDownDate = new Date("December 10, 2021 00:00:00").getTime();

// Обновляем таймер каждую секунду
var countDownFunction = setInterval(function () {

//Время на данный момент
var now = new Date().getTime();
//Высчитываем промежуток времени между установленным временем и сегодня
var distance = countDownDate - now;

//Высчитываем время для дней, часов, минут и секунд
var days = Math.floor(distance / (1000 * 60 * 60 * 24));
var hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60 ));
var minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
var secondes = Math.floor((distance % (1000 * 60)) / 1000);

//Выдаем результат на сайте
document.getElementById("time").innerHTML = days + "д " + hours + "ч " + minutes + "м " + secondes + "с ";

//Что делать, когда отсчет будет равен 0
if (distance < 0) {
clearInterval(countDownFunction);
document.getElementById("time").innerHTML = "Ну вот и наступил твой день. Ты моя самая лучшая булочка, самое дорогое что есть у меня. Спасибо что ты появилась в моей жизни. Я люблю тебя";
}
},1000)

</script>
</body>
</html>

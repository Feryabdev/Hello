<!DOCTYPE html>
<head>
  <meta http-equiv="CONTENT-TYPE" content="text/html; charset=UTF-8">
  <link rel="stylesheet" href="styles/style.css">
  <title>Hello, World!</title> 
  <style>
  body {
        margin: 30px;
        border-radius: 50px;
        border: 1px solid #333; 
       background-color: #333; 
        text-align: center;
        color: #FFF;
      }
  
  </style>
  </head>
   <body>
     <h1>مرحبآ بك في تطبيق الضرب </h1>
     <h2>جاهز تختبر جميع جداول الضرب خطوة بخطوة</h2>
     <h1 id="test"></h1>
     <button onclick="run()">ابدا الان</button>
     <script>
         
          function run(){
let number = Number(prompt("اكتب رقم ")),
    score = "";
  if (isNaN(number)) {
     document.getElementById('test').innerHTML =
     "write a Number";
   
  } else if (number <= 0) {
   document.getElementById('test').innerHTML =
   "Type a number except zero"
   
  }else {
     
  for (let i = 1; i <= 10; i++) {
   
     score += number + "×" + i + "=" + (number * i) + "<br>";
     
  }
  
   document.getElementById('test').innerHTML =
     score;
  }
 }
         
         </script>
     
</body>
</html>

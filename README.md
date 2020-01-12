
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<link rel="apple-touch-icon" type="image/png" href="https://static.codepen.io/assets/favicon/apple-touch-icon-5ae1a0698dcc2402e9712f7d01ed509a57814f994c660df9f7a952f3060705ee.png" />
<meta name="apple-mobile-web-app-title" content="CodePen">
<link rel="shortcut icon" type="image/x-icon" href="https://static.codepen.io/assets/favicon/favicon-aec34940fbc1a6e787974dcd360f2c6b63348d4b1f4e06c77743096d55480f33.ico" />
<link rel="mask-icon" type="" href="https://static.codepen.io/assets/favicon/logo-pin-8f3771b1072e3c38bd662872f6b673a722f4b3ca2421637d5596661b4e2132cc.svg" color="#111" />
<title>CodePen - AACoding01-8</title>
<style>
ul{
  background:lightgrey;
  font-size:18px;
}
.correct{
  background:green;
}

.incorrect{
  background:red;
}
</style>
</head>
<body translate="no">
<h1>Math Problems</h1>
<ul>
<li>2 + 2 <input data-correct="4" /></li>
<li>2 - 3 <input data-correct="-1" /></li>
<li>2<sup>3<input data-correct="8" /></sup>
<li><sup>1</sup>&frasl;<sub>10</sub> * 10<input data-correct="1" /></li>
<li>4! <input data-correct="24" /></li>
<li>5x + 10 = 25<input data-correct="3" /></li>
<li>6(3x + 8)<input data-correct="18x + 48" /></li>
<li>4x + 12 > 20 <input data-correct="x > 8" /></li>
<li>4 ÷ <sup>1</sup>&frasl;<sub>2</sub><input data-correct="8" /></li>
<li><sup>x + 14</sup>&frasl;<sub>3</sub> = 5<input data-correct="1" /></li></ul>
<script> src='https://cdnjs.cloudflare.com/ajax/libs/jquery/3.4.1/jquery.min.js'></script>
<script id="rendered-js">
console.clear();
console.log("hello world");

$("input").change(onChange);

function onChange(evt){

  let correct = $(this).data("correct");
  let response = $(this).val();
  if(correct==response){
    console.log("correct")
    $(this).removeClass("incorrect").addClass("correct");
  } else{
    $(this).removeClass("correct").addClass("incorrect")
    console.log("incorrect")
  }

}
    </script>
</body>
</html>

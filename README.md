# Calculator
HTML, CSS, JavaScript

![Screenshot_2020-08-15 Problem 1](https://user-images.githubusercontent.com/33843231/90317996-0eaf4780-df4f-11ea-9eb6-18aa66669aed.png)

```html

<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Problem 1</title>
    <link rel="stylesheet" type="text/css" href="style.css">
  </head>
  <body>
    <form class="calculator" name="calc">
      <input type="text" class="value" name="txt" readonly="" />
      <span class="num" onclick="document.calc.txt.value +='%'">%</span>
      <span class="num" onclick="document.calc.txt.value +='+/-'">+/-</span>
      <span class="num clear" onclick="document.calc.txt.value =''">C</span>
      <span class="num opt" onclick="document.calc.txt.value +='/'">/</span>
      <span class="num" onclick="document.calc.txt.value +='7'">7</span>
      <span class="num" onclick="document.calc.txt.value +='8'">8</span>
      <span class="num" onclick="document.calc.txt.value +='9'">9</span>
      <span class="num opt" onclick="document.calc.txt.value +='*'">x</span>
      <span class="num" onclick="document.calc.txt.value +='4'">4</span>
      <span class="num" onclick="document.calc.txt.value +='5'">5</span>
      <span class="num" onclick="document.calc.txt.value +='6'">6</span>
      <span class="num opt" onclick="document.calc.txt.value +='-'">-</span>
      <span class="num" onclick="document.calc.txt.value +='1'">1</span>
      <span class="num" onclick="document.calc.txt.value +='2'">2</span>
      <span class="num" onclick="document.calc.txt.value +='3'">3</span>
      <span class="num opt" onclick="document.calc.txt.value +='+'">+</span>
      <span class="num" onclick="document.calc.txt.value +='0'">0</span>
      <span class="num" onclick="document.calc.txt.value +='.'">.</span>
      <span class="num equal" onclick="document.calc.txt.value = eval(calc.txt.value)">=</span>
    </form>
  </body>
</html>

```

```css

* {
  margin: 0;
  padding: 0;
  font-family: sans-serif;
}

body {
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: 100vh;
  background-image: linear-gradient(
    to bottom right,
    rgb(159, 48, 223),
    rgb(238, 151, 100)
  );
}

.calculator {
  position: relative;
  display: grid;
}

.calculator .value {
  grid-column: span 4;
  height: 100px;
  text-align: right;
  border: none;
  outline: none;
  padding: 10px;
  font-size: 18px;
  background: black;
  color: #fff;
}

.calculator span {
  display: grid;
  width: 60px;
  height: 60px;
  color: rgb(0, 0, 0);
  background: #ffffffee;
  place-items: center;
}

.calculator span:active {
  background: black !important;
  color: whitesmoke !important;
}

.calculator span.equal {
  grid-column: span 2;
  width: 120px;
  color: #fff;
  background: rgb(240, 45, 175);
}
.calculator span.opt {
  color: #fff;
  background: rgb(153, 37, 199);
}

```

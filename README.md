# What-time-is-it-
Relógio digital usando HTML,  JS e CSS

<!DOCTYPE html>


<html lang="en">

  <head>

    <meta charset="utf-8">

    <meta http-equiv="X-UA-Compatible" content="IE=edge">

    <meta name="viewport" content="width=device-width, initial-scale=1">

    <title>Digital Clock</title>

    <link href="./styles.css" type="text/css" rel="stylesheet">

  </head>

  <body>

    <div class="container">

      <div class="clock"></div>

    </div>





    









    










* {

  box-sizing: border-box;

  margin: 0;

  padding: 0;

}

body {

  min-altura: 100vh

  width: 100%;

}

.container {

  background-image: radial-gradient(circle, #0077ff 0%, #00ffaa 100%);

  display: flex;

  justify-content: center;

  align-items: center;

  height: 100vh;

}

.clock {

  align-items: center;

  background-color: rgba(255, 255, 255, 0.5);

  border: 1px solid #000;

  border-radius: 3%;

  color: #fff;

  display: flex;

  font-size: 60px;

  justify-content: center;

  height: 100px;

  width: 250px;

}

const getHours = () => {

  const clock = document.getElementsByClassName('clock')[0]

  const date = new Date()

  const hours = date.getHours()

  const minutes = date.getMinutes()

  const seconds = date.getSeconds()

  const hour = hours < 10 ? `0${hours}` : hours

  const minute = minutes < 10 ? `0${minutes}` : minutes

  const second = seconds < 10 ? `0${seconds}` : seconds

  clock.innerHTML = `${hour}:${minute}:${second}`

}

setInterval(() => {

  getHoras()
p
}, 1000)
p
veja 

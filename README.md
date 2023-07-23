<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title></title>
    <style>
      @import url("https://fonts.googleapis.com/css?family=Poppins:100,200,300,400,500,600,700,800,900");
      * {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
        font-family: poppins;
      }
      body {
        display: flex;
        justify-content: center;
        align-items: center;
        min-height: 100vh;
        background: #222;
      }
      .container {
        position: relative;
        display: flex;
        justify-content: center;
        align-items: center;
      }
      .container .cigarette {
        transform-style: preserve-3d;
        animation: animate 15s linear infinite;
      }
      @keyframes animate {
        0% {
          transform: perspective(1000px) rotateX(0deg);
        }
        100% {
          transform: perspective(1000px) rotateX(360deg);
        }
      }
      .container .cigarette span {
        position: absolute;
        color: #fff;
        font-size: 1.35em;
        font-weight: 900;
        text-transform: uppercase;
        line-height: 0.76em;
        text-shadow: 0 2px 5px rgba(0, 0, 0, 0.25);
        transform: translate(-50%, -50%) rotateX(calc(var(--i) * 36deg))
          translateZ(25px);
        background: rgba(0, 0, 0, 0.25);
        transform-style: preserve-3d;
      }
      .container .cigarette span i {
        font-style: normal;
        color: #ec9535;
      }
      .container .cigarette span i:first-child:after {
        content: "l";
        color: #ccc;
        text-transform: lowercase;
      }
      .container .cigarette span i:last-child {
        color: #f00;
        filter: blur(2px);
        text-shadow: -4px 0 2px #000, 8px 0 20px #f00, 8px 0 24px #f00,
          8px 0 0 #222, 12px 0 #555, 16px 0 #666, 20px 0 #888, 24px 0 #999;
      }
    </style>
  </head>
  <body>
    <div class="container">
      <div class="cigarette">
        <span style="--i: 1"><i>Nooooo</i>Smooooooooking<i>|</i></span>
        <span style="--i: 2"><i>Nooooo</i>Smooooooooking<i>|</i></span>
        <span style="--i: 3"><i>Nooooo</i>Smooooooooking<i>|</i></span>
        <span style="--i: 4"><i>Nooooo</i>Smooooooooking<i>|</i></span>
        <span style="--i: 5"><i>Nooooo</i>Smooooooooking<i>|</i></span>
        <span style="--i: 6"><i>Nooooo</i>Smooooooooking<i>|</i></span>
        <span style="--i: 7"><i>Nooooo</i>Smooooooooking<i>|</i></span>
        <span style="--i: 8"><i>Nooooo</i>Smooooooooking<i>|</i></span>
        <span style="--i: 9"><i>Nooooo</i>Smooooooooking<i>|</i></span>
        <span style="--i: 10"><i>Nooooo</i>Smooooooooking<i>|</i></span>
      </div>
    </div>
  </body>
</html>

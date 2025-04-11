<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>¡Feliz Cumple, Milena!</title>
  <style>
    body {
      background: linear-gradient(to bottom, #ffd6ec, #ffc1de);
      color: #4b2e1f;
      font-family: 'Georgia', serif;
      text-align: center;
      padding: 50px;
      background-size: cover;
      background-attachment: fixed;
      overflow: hidden;
    }

    .card {
      background: linear-gradient(to bottom right, rgba(255, 240, 245, 0.9), rgba(255, 255, 255, 0.9));
      padding: 40px;
      border-radius: 30px;
      display: inline-block;
      max-width: 750px;
      margin-top: 50px;
      box-shadow: 0 0 35px rgba(255, 182, 193, 0.7);
      animation: fadeInUp 1s ease-out;
      position: relative;
      z-index: 2;
    }

    h1 {
      font-size: 3em;
      color: #d473d4;
      text-shadow: 2px 2px #fff;
    }

    p {
      font-size: 1.4em;
      margin-top: 20px;
      line-height: 1.6em;
      color: #5c3a2e;
    }

    .meow {
      font-size: 2.5em;
      color: #f39c12;
      margin-top: 40px;
      animation: glow 1.5s ease-in-out infinite alternate;
    }

    @keyframes glow {
      from {
        text-shadow: 0 0 5px #ffef99, 0 0 10px #f8d66d, 0 0 15px #f1c40f;
      }
      to {
        text-shadow: 0 0 15px #fff0a5, 0 0 25px #ffe066, 0 0 35px #f7d26b;
      }
    }

    .speech-bubble {
      background: #fff8dc;
      color: #4b3b0a;
      padding: 15px 20px;
      border-radius: 15px;
      font-size: 1em;
      font-family: 'Comic Sans MS', cursive;
      box-shadow: 2px 2px 10px rgba(0, 0, 0, 0.3);
      display: inline-block;
      width: max-content;
      max-width: 250px;
      margin-top: 30px;
    }

    @keyframes fadeInUp {
      from {
        opacity: 0;
        transform: translateY(20px);
      }
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

    /* 🌟 LINTERNAS flotantes */
    .lantern {
      position: absolute;
      width: 40px;
      height: 60px;
      background: url('https://i.pinimg.com/originals/f3/5e/ce/f35ece1de7a10e577fd15b8a839b768e.png') no-repeat center center;
      background-size: contain;
      opacity: 0.8;
      animation: floatLantern 12s linear infinite;
      z-index: 1;
    }

    @keyframes floatLantern {
      0% {
        transform: translateY(100vh) scale(0.8);
        opacity: 0;
      }
      20% {
        opacity: 1;
      }
      100% {
        transform: translateY(-20vh) scale(1);
        opacity: 0;
      }
    }
  </style>
</head>
<body>
  <!-- 🎵 MÚSICA DE FONDO -->
  <audio autoplay loop>
    <source src="https://vgmsite.com/soundtracks/tangled/kzyjlxxwox/06%20Kingdom%20Dance.mp3" type="audio/mpeg">
    Tu navegador no soporta la música de los cuentos de hadas 🎶
  </audio>

  <!-- ✨ LINTERNAS flotando -->
  <script>
    for (let i = 0; i < 15; i++) {
      const lantern = document.createElement('div');
      lantern.classList.add('lantern');
      lantern.style.left = `${Math.random() * 100}%`;
      lantern.style.animationDelay = `${Math.random() * 15}s`;
      lantern.style.animationDuration = `${10 + Math.random() * 10}s`;
      document.body.appendChild(lantern);
    }
  </script>

  <!-- 🎉 TARJETA -->
  <div class="card">
    <h1>¡Feliz Cumpleaños, Milena! 🌸</h1>
    <p>
      Hoy no solo celebramos tu cumpleaños… también el día en que el mundo se iluminó, igual que las linternas flotando en el cielo ✨.
    </p>
    <p>
      Rapunzel soltó su cabello solo para unirte a esta fiesta, Pascal se puso elegante, y Flynn dice que no te va a robar nada... excepto una sonrisa.
    </p>
    <p>
      Y por cierto, él insiste en decirte que <strong>no todos los días una princesa como tú cumple años...</strong> así que no olvides practicar tu <em>"mirada arrebatadora"</em>. 
    </p>

    <div class="speech-bubble">¿Funciona esto? No sé… pero lo intento.</div>

    <p>
      Que tu día esté lleno de magia, aventuras, trenzas épicas, arte en las paredes y sueños que se hacen realidad 🌟.
    </p>
    <div class="meow">¡Y que las linternas te guíen siempre! 🎉</div>
  </div>
</body>
</html>

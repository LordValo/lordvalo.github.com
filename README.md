# lordvalo.github.com
<!DOCTYPE html>
<html lang="de">
<head>
  <meta charset="UTF-8">
  <title>Tim Wimmer Fanpage</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <style>
    body {
      font-family: Arial, sans-serif;
      background: linear-gradient(135deg, #cce0ff, #e6f7ff);
      text-align: center;
      padding: 50px;
    }

    h1 {
      color: #003366;
    }

    .welcome {
      font-size: 1.5em;
      margin-bottom: 30px;
    }

    .question {
      font-size: 1.2em;
      margin: 20px 0;
    }

    button {
      margin: 10px;
      padding: 10px 20px;
      font-size: 1em;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      transition: background 0.3s;
    }

    button:hover {
      background-color: #d0e7ff;
    }

    .award {
      margin-top: 40px;
      font-size: 1.5em;
      color: #004080;
    }
  </style>
</head>
<body>
  <h1>Willkommen auf der offiziellen Fanpage von Tim Wimmer! 🎉</h1>
  <div class="welcome" id="welcomeMsg">Schön, dass du da bist!</div>

  <div class="question">Wie sehr magst du Tim Wimmer?</div>
  <button onclick="showAward('superfan')">Ich bin ein Mega-Fan!</button>
  <button onclick="showAward('normal')">Er ist ganz cool 😎</button>
  <button onclick="showAward('kritisch')">Ich kenne ihn kaum 🤔</button>

  <div class="award" id="award"></div>

  <script>
    function showAward(level) {
      const awardEl = document.getElementById('award');
      let message = '';

      switch(level) {
        case 'superfan':
          message = '🏆 Du bist ein wahrer Tim Wimmer ULTRA! Danke für deine Unterstützung!';
          break;
        case 'normal':
          message = '👍 Schön, dass du Tim sympathisch findest!';
          break;
        case 'kritisch':
          message = '🧐 Vielleicht lernst du Tim ja noch besser kennen!';
          break;
      }

      awardEl.textContent = message;
    }
  </script>
</body>
</html>

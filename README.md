<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Lendário Launcher</title>
  <style>
    body {
      margin: 0;
      font-family: 'Comic Sans MS', sans-serif;
      background-color: #013220; /* Verde escuro */
      color: #fff;
    }

    header {
      background-color: #006400; /* Verde forte */
      padding: 20px;
      text-align: center;
      font-size: 2em;
      font-weight: bold;
      border-bottom: 5px solid #32CD32; /* Verde limão */
      box-shadow: 0 4px 8px rgba(0,0,0,0.5);
    }

    .container {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
      gap: 20px;
      padding: 20px;
    }

    .card {
      background-color: #228B22; /* Verde médio */
      border-radius: 15px;
      padding: 15px;
      text-align: center;
      transition: transform 0.3s, background-color 0.3s;
      cursor: pointer;
      box-shadow: 0 4px 8px rgba(0,0,0,0.4);
    }

    .card:hover {
      transform: scale(1.05);
      background-color: #2E8B57; /* Verde mais claro */
    }

    .card img {
      width: 100%;
      border-radius: 10px;
    }

    .card h3 {
      margin-top: 10px;
      font-size: 1.2em;
      color: #ADFF2F; /* Verde neon */
    }

    .card p {
      font-size: 0.9em;
      margin: 10px 0;
    }

    .btn {
      background-color: #32CD32; /* Verde limão */
      color: #013220;
      padding: 8px 12px;
      border-radius: 8px;
      text-decoration: none;
      font-weight: bold;
      display: inline-block;
      margin-top: 10px;
      box-shadow: 0 3px 6px rgba(0,0,0,0.3);
    }

    .btn:hover {
      background-color: #00FF7F; /* Verde claro */
    }

    .toggle {
      cursor: pointer;
      color: #ADFF2F;
      font-weight: bold;
      margin-top: 10px;
      display: inline-block;
    }

    .versions {
      display: none;
      margin-top: 10px;
      background: rgba(0,0,0,0.3);
      padding: 8px;
      border-radius: 8px;
      text-align: left;
      font-size: 0.9em;
    }

    .versions a {
      display: block;
      margin: 3px 0;
      color: #ADFF2F;
      text-decoration: none;
      font-weight: bold;
    }

    .versions a:hover {
      color: #00FF7F;
    }

    footer {
      background-color: #006400;
      text-align: center;
      padding: 15px;
      font-size: 0.9em;
      border-top: 5px solid #32CD32;
      box-shadow: 0 -4px 8px rgba(0,0,0,0.5);
    }
  </style>
</head>
<body>
  <header>
    🎮 Lendário Launcher
  </header>

  <!-- Música de fundo -->
  <audio autoplay loop>
    <source src="https://files.catbox.moe/xtkmrv.m4a" type="audio/mpeg">
    Seu navegador não suporta áudio.
  </audio>

  <div class="container">
    <!-- Jogo 1 -->
    <div class="card">
      <img src="https://via.placeholder.com/250x150.png?text=Lendario+Voo+Simulador" alt="Lendário Voo Simulador">
      <h3>Lendário Voo Simulador</h3>
      <p>Teste suas habilidades de voo nesse simulador incrível!</p>
      <a href="https://luancraft39.github.io/Lend-rio-Voo-Simulador/" class="btn" target="_blank">Jogar</a>
    </div>

    <!-- Jogo 2 com versões -->
    <div class="card">
      <img src="https://via.placeholder.com/250x150.png?text=Lendario+Parkour+Adventure" alt="Lendário Parkour Adventure">
      <h3>Lendário Parkour Adventure</h3>
      <p>Supere obstáculos e viva uma aventura radical de parkour!</p>
      <a href="https://luancraft39.github.io/Lend-rio-Parkour-Adventure/" class="btn" target="_blank">Jogar Versão Principal</a>
      <span class="toggle" onclick="toggleVersions('parkourVersions')">⬇ Mostrar Versões</span>
      <div class="versions" id="parkourVersions">
        <a href="https://luancraft39.github.io/Lend-rio-Parkour-Adventure-Vers-o-2.0.1" target="_blank">Versão 2.0.1</a>
      </div>
    </div>

    <!-- Jogo 3 -->
    <div class="card">
      <img src="https://via.placeholder.com/250x150.png?text=Lendario+Click+Simulador" alt="Lendário Click Simulador">
      <h3>Lendário Click Simulador</h3>
      <p>Mostre sua velocidade de cliques e alcance recordes!</p>
      <a href="https://luancraft39.github.io/Lend-rio-Click-Simulador/" class="btn" target="_blank">Jogar</a>
    </div>

    <!-- Jogo 4 -->
    <div class="card">
      <img src="https://via.placeholder.com/250x150.png?text=Lendario+Beat+Clash" alt="Lendário Beat Clash">
      <h3>Lendário Beat Clash</h3>
      <p>Entre no ritmo e enfrente batalhas musicais épicas!</p>
      <a href="https://luancraft39.github.io/LEND-RIO-BEAT-CLASH-X/" class="btn" target="_blank">Jogar</a>
    </div>

    <!-- Jogo 5 -->
    <div class="card">
      <img src="https://via.placeholder.com/250x150.png?text=Lendario+Dash" alt="Lendário Dash">
      <h3>Lendário Dash</h3>
      <p>Corra, desvie e desafie seus reflexos nesse jogo eletrizante!</p>
      <a href="https://luancraft39.github.io/Lend-rio-Dash/" class="btn" target="_blank">Jogar</a>
    </div>

    <!-- Jogo 6 com versões -->
    <div class="card">
      <img src="https://via.placeholder.com/250x150.png?text=Lendario+Tetris+Edition" alt="Lendário Tetris Edition">
      <h3>Lendário Tetris Edition</h3>
      <p>Clássico Tetris em uma versão lendária para você se divertir!</p>
      <a href="https://luancraft39.github.io/Lend-rio-tetris-edition/" class="btn" target="_blank">Jogar Versão Principal</a>
      <span class="toggle" onclick="toggleVersions('tetrisVersions')">⬇ Mostrar Versões</span>
      <div class="versions" id="tetrisVersions">
        <a href="https://luancraft39.github.io/Lend-rio-Cl-ssico-Edition/" target="_blank">Versão 1.0 (Clássico Edition)</a>
      </div>
    </div>
  </div>

  <footer>© 2025 - 2026 Lendário Studio Community — todos os direitos reservados.</footer>

  <script>
    function toggleVersions(id) {
      const versions = document.getElementById(id);
      if (versions.style.display === "block") {
        versions.style.display = "none";
      } else {
        versions.style.display = "block";
      }
    }
  </script>
</body>
</html>

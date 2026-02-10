<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Back to the 90s</title>
<link href="https://fonts.googleapis.com/css2?family=Press+Start+2P&display=swap" rel="stylesheet">
<style>
  /* Reset & body */
  * { box-sizing: border-box; margin: 0; padding: 0; }
  body {
    font-family: 'Press Start 2P', cursive;
    background: linear-gradient(135deg, #ff00cc, #3333ff);
    color: #fff;
    overflow-x: hidden;
  }

  /* Header & Nav */
  header {
    padding: 20px;
    background-color: rgba(0,0,0,0.7);
    text-align: center;
  }
  nav a {
    margin: 10px;
    color: #00ffcc;
    text-decoration: none;
    font-size: 12px;
  }
  nav a:hover { color: #ffcc00; }

  /* Neon text */
  .neon {
    color: #ff00ff;
    text-shadow: 0 0 5px #ff00ff, 0 0 10px #00ffff, 0 0 20px #ff00ff;
    animation: flicker 1.5s infinite alternate;
  }
  @keyframes flicker {
    0%, 100% { opacity: 1; }
    50% { opacity: 0.6; }
  }

  /* Sections */
  section { padding: 40px 20px; text-align: center; }
  .cards { display: flex; flex-wrap: wrap; justify-content: center; gap: 20px; }
  .card {
    background: rgba(255,255,255,0.1);
    padding: 20px;
    width: 200px;
    border-radius: 10px;
    transition: transform 0.3s;
  }
  .card:hover { transform: scale(1.1) rotate(-5deg); }

  /* Footer */
  footer {
    padding: 20px;
    background-color: rgba(0,0,0,0.7);
    text-align: center;
  }

  /* Custom cursor */
  body {
    cursor: url('https://upload.wikimedia.org/wikipedia/commons/3/3d/Tamagotchi_cursor.png'), auto;
  }

  /* Quiz style */
  .quiz { margin-top: 20px; }
  .quiz button {
    background: #ff00cc;
    color: #fff;
    border: none;
    padding: 10px 15px;
    margin: 5px;
    cursor: pointer;
  }
  .quiz button:hover { background: #00ffff; color: #000; }
</style>
</head>
<body>
<header>
  <h1 class="neon">Back to the 90s!</h1>
  <nav>
    <a href="#cartoons">Cartoons</a>
    <a href="#music">Music</a>
    <a href="#games">Games</a>
    <a href="#toys">Toys</a>
    <a href="#quiz">Quiz</a>
  </nav>
</header>

<section id="cartoons">
  <h2 class="neon">Favorite 90s Cartoons</h2>
  <div class="cards">
    <div class="card">Rugrats</div>
    <div class="card">Power Rangers</div>
    <div class="card">Sailor Moon</div>
  </div>
</section>

<section id="music">
  <h2 class="neon">90s Music Hits</h2>
  <div class="cards">
    <div class="card">
      Backstreet Boys
      <iframe width="180" height="100" src="https://www.youtube.com/embed/2S7QXH9b3n0" frameborder="0" allowfullscreen></iframe>
    </div>
    <div class="card">
      Spice Girls
      <iframe width="180" height="100" src="https://www.youtube.com/embed/pRpeEdMmmQ0" frameborder="0" allowfullscreen></iframe>
    </div>
  </div>
</section>

<section id="games">
  <h2 class="neon">Classic 90s Games</h2>
  <div class="cards">
    <div class="card">Pokémon Red/Blue</div>
    <div class="card">Tamagotchi</div>
    <div class="card">Super Mario 64</div>
  </div>
</section>

<section id="toys">
  <h2 class="neon">Popular Toys</h2>
  <div class="cards">
    <div class="card">Beanie Babies</div>
    <div class="card">Pogs</div>
    <div class="card">Game Boy</div>
  </div>
</section>

<section id="quiz">
  <h2 class="neon">Which 90s Character Are You?</h2>
  <div class="quiz">
    <button onclick="alert('You are Tommy Pickles!')">Rugrats</button>
    <button onclick="alert('You are Sailor Moon!')">Sailor Moon</button>
    <button onclick="alert('You are Ash Ketchum!')">Pokémon</button>
  </div>
</section>

<footer>
  &copy; 2026 Back to the 90s | Contact: 90s@retrofun.com
</footer>

</body>
</html>

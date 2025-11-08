<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Lizard Flick - README</title>
  <meta name="viewport" content="width=800">
  <style>
    /* Moving gradient for heading */
    @keyframes gradientMove {
      0% {
        background-position: 0% 50%;
      }
      100% {
        background-position: 100% 50%;
      }
    }
    body {
      font-family: 'Segoe UI', Verdana, Geneva, Tahoma, sans-serif;
      margin: 0;
      background: linear-gradient(135deg, #e8ffc9 0%, #a3d977 100%);
      min-height: 100vh;
      color: #32530d;
    }
    .heading-animated {
      text-align: center;
      font-size: 3em;
      font-weight: bold;
      margin-top: 40px;
      margin-bottom: 16px;
      padding: 20px 0;
      background: linear-gradient(90deg, #8fd576 0%, #53fba3 25%, #f3f25b 50%, #f68949 75%, #8fd576 100%);
      background-size: 200% 200%;
      color: #275114;
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      animation: gradientMove 4s linear infinite;
      border-radius: 16px;
      border: 2px solid #8fd576;
      box-shadow: 0 4px 18px rgba(117, 167, 76, 0.2);
      letter-spacing: 2px;
    }
    .container {
      max-width: 750px;
      margin: 0 auto;
      background: #fafef6e6;
      border-radius: 18px;
      box-shadow: 0 2px 12px #c5efc283;
      padding: 32px 32px 24px 32px;
      margin-bottom: 34px;
    }
    h2 {
      color: #18a046;
      border-bottom: 2px solid #b6ec7c;
      padding-bottom: 6px;
      margin-bottom: 14px;
      margin-top: 26px;
      font-size: 2em;
      background: linear-gradient(90deg, #d8fac9 35%, #b6ec7c 100%);
      border-radius: 8px 8px 0 0;
      padding-left: 8px;
    }
    ul {
      margin-top: 10px;
      margin-bottom: 22px;
    }
    li {
      font-size: 1.14em;
      padding: 2px 0 2px 10px;
    }
    .play-demo {
      display: block;
      width: 100%;
      background: linear-gradient(90deg, #f3f25b 0%, #8fd576 100%);
      border: none;
      padding: 12px 0;
      font-size: 1.24em;
      font-weight: bold;
      color: #1f4f14;
      border-radius: 8px;
      box-shadow: 0 2px 4px #bddbbd44;
      cursor: pointer;
      margin-bottom: 24px;
      margin-top: 16px;
      text-align: center;
      text-decoration: none;
      transition: background 0.2s;
    }
    .play-demo:hover {
      background: linear-gradient(90deg, #8fd576 0%, #f3f25b 100%);
    }
    .code-block {
      background: #ecf8e0;
      color: #345d20;
      font-family: 'Fira Mono', 'Consolas', 'Menlo', monospace;
      padding: 16px;
      border-radius: 10px;
      margin-bottom: 24px;
      border: 1px solid #b6ec7c;
      overflow-x: auto;
      font-size: 1em;
    }
    .screenshots {
      text-align: center;
      margin: 18px 0;
    }
    .screenshot-img {
      max-width: 420px;
      border-radius: 11px;
      box-shadow: 0 2px 16px #b3e8aa55;
      margin-bottom: 10px;
      border: 2px solid #b6ec7c;
    }
    .license {
      background: #f8ffe8ee;
      padding: 10px 16px;
      border-radius: 8px;
      margin-bottom: 10px;
      font-weight: bold;
    }
    .thanks {
      color: #a9cb44;
      font-style: italic;
      margin-top: 12px;
      font-size: 1.13em;
      text-align: center;
    }
    @media (max-width: 900px) {
      .container, body {
        padding: 2vw;
      }
      .container {
        max-width: 97vw;
      }
      .heading-animated {
        font-size: 2em;
      }
    }
  </style>
</head>
<body>
  <div class="heading-animated">🦎 Lizard Flick</div>
  <div class="container">
    <h2>Game Overview</h2>
    <p>
      <strong>Lizard Flick</strong> is a fast-paced, fun flicking game where you control a lively lizard! Flick your lizard past obstacles, snatch tasty insects, and master unique challenges. Can you climb the leaderboard and become the champion lizard?
    </p>

    <h2>Features</h2>
    <ul>
      <li><strong>Intuitive Flick Controls:</strong> Move your lizard effortlessly with drag and flick gestures.</li>
      <li><strong>Challenging Levels:</strong> Conquer inventive obstacles and increasingly tricky stages.</li>
      <li><strong>Exciting Collectibles:</strong> Snatch insects & power-ups, rack up points, and unlock fun skins.</li>
      <li><strong>Upgrades:</strong> Enhance your lizard's powers and style with unlockable upgrades.</li>
      <li><strong>Leaderboards:</strong> Compete with friends for high scores and lizard glory.</li>
    </ul>

    <a class="play-demo" href="#" tabindex="0" title="Play Demo (for HTML5 version)">▶️ Play Web Demo</a>

    <h2>How to Play</h2>
    <ul>
      <li><strong>Flick to Move:</strong> Drag your mouse (or finger) and release to flick the lizard toward your target.</li>
      <li><strong>Collect:</strong> Catch bugs and powerups to boost your score.</li>
      <li><strong>Dodge:</strong> Avoid traps, obstacles, and predators to survive!</li>
      <li><strong>Upgrade:</strong> Spend points to unlock new lizards and powers.</li>
    </ul>

    <h2>Quick Start (HTML Version)</h2>
    <div class="code-block">
      &lt;!DOCTYPE html&gt;<br>
      &lt;html lang="en"&gt;<br>
      &lt;head&gt;<br>
      &nbsp;&nbsp;&lt;title&gt;Lizard Flick&lt;/title&gt;<br>
      &nbsp;&nbsp;&lt;meta charset="UTF-8"&gt;<br>
      &nbsp;&nbsp;&lt;style&gt;<br>
      &nbsp;&nbsp;&nbsp;canvas { background: #a3d977; border:2px solid #4c753d; display:block; margin:16px auto; }<br>
      &nbsp;&nbsp;&lt;/style&gt;<br>
      &lt;/head&gt;<br>
      &lt;body&gt;<br>
      &nbsp;&nbsp;&lt;canvas id="gameCanvas" width="800" height="600"&gt;&lt;/canvas&gt;<br>
      &nbsp;&nbsp;&lt;script src="game.js"&gt;&lt;/script&gt;<br>
      &lt;/body&gt;<br>
      &lt;/html&gt;
    </div>

    <h2>Screenshots</h2>
    <div class="screenshots">
      <img src="https://opengameart.org/sites/default/files/styles/large/public/lizard2.png" alt="Lizard Flick screenshot demo" class="screenshot-img" />
      <img src="https://opengameart.org/sites/default/files/styles/large/public/lizard1.png" alt="Lizard Flick screenshot demo" class="screenshot-img" />
      <br>
      <span style="font-size:0.9em;">*(Replace with your own screenshots!)*</span>
    </div>

    <h2>Installation</h2>
    <ol>
      <li>Clone the repo:<br>
        <span class="code-block">
          git clone https://github.com/&lt;your-username&gt;/lizard-flick.git
        </span>
      </li>
      <li>Open <b>index.html</b> in your browser and play!</li>
      <li>(For advanced usage: <code>npm install</code> and <code>npm start</code>)</li>
    </ol>

    <h2>License</h2>
    <div class="license">MIT License</div>
    <div class="thanks">
      Thanks to contributors and asset creators! Graphics from <a href="https://opengameart.org/">OpenGameArt</a>.<br>
      <br>
      <b>Flick fast, flick smart, be the best lizard!</b>
    </div>
  </div>
</body>
</html>

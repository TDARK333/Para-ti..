<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Para ti, con todo mi corazón</title>
  <link href="https://fonts.googleapis.com/css2?family=Lora:ital,wght@0,400;0,500;1,400&family=Cinzel:wght@400;500&display=swap" rel="stylesheet">
  <style>
    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

    body {
      min-height: 100vh;
      background: radial-gradient(ellipse at 60% 40%, #2a0a0a 0%, #0d0202 60%, #000 100%);
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      font-family: 'Lora', Georgia, serif;
      padding: 2rem 1rem;
      overflow-x: hidden;
    }

    .particles {
      position: fixed;
      top: 0; left: 0;
      width: 100%; height: 100%;
      pointer-events: none;
      z-index: 0;
      overflow: hidden;
    }

    .particle {
      position: absolute;
      background: #FFD700;
      border-radius: 50%;
      opacity: 0;
      animation: float-up linear infinite;
    }

    @keyframes float-up {
      0%   { transform: translateY(100vh) scale(0); opacity: 0; }
      10%  { opacity: 0.6; }
      90%  { opacity: 0.3; }
      100% { transform: translateY(-10vh) scale(1.5); opacity: 0; }
    }

    #top-title {
      font-family: 'Cinzel', serif;
      color: #FFD700;
      font-size: clamp(13px, 2.5vw, 17px);
      letter-spacing: 0.25em;
      text-transform: uppercase;
      margin-bottom: 28px;
      opacity: 0;
      animation: fade-in 1.5s ease 0.3s forwards;
      text-shadow: 0 0 20px rgba(255,215,0,0.3);
      position: relative;
      z-index: 2;
    }

    @keyframes fade-in { to { opacity: 1; } }

    #book-wrap {
      position: relative;
      width: min(680px, 96vw);
      height: clamp(400px, 60vw, 500px);
      z-index: 2;
    }

    #cover-left, #cover-right {
      position: absolute;
      top: 0;
      height: 100%;
      width: calc(50% - 13px);
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      cursor: pointer;
      z-index: 30;
      transition: transform 1.4s cubic-bezier(0.4,0,0.2,1), opacity 0.4s ease 1.0s;
    }

    #cover-left {
      left: 0;
      background: linear-gradient(135deg, #5C0A0A 0%, #8B1A1A 40%, #A52020 70%, #7B1111 100%);
      border-radius: 16px 0 0 16px;
      transform-origin: right center;
      box-shadow: -8px 8px 30px rgba(0,0,0,0.6), inset 2px 0 8px rgba(255,255,255,0.05);
      border-right: 3px solid #3D0000;
    }

    #cover-right {
      right: 0;
      background: linear-gradient(225deg, #5C0A0A 0%, #8B1A1A 40%, #A52020 70%, #7B1111 100%);
      border-radius: 0 16px 16px 0;
      transform-origin: left center;
      box-shadow: 8px 8px 30px rgba(0,0,0,0.6), inset -2px 0 8px rgba(255,255,255,0.05);
      border-left: 3px solid #3D0000;
    }

    #cover-left::before, #cover-right::before {
      content: '';
      position: absolute;
      inset: 0;
      background-image: repeating-linear-gradient(90deg, transparent, transparent 3px, rgba(0,0,0,0.08) 3px, rgba(0,0,0,0.08) 4px);
      border-radius: inherit;
      pointer-events: none;
    }

    #cover-left::after, #cover-right::after {
      content: '';
      position: absolute;
      inset: 10px;
      border: 1px solid rgba(255,215,0,0.25);
      border-radius: 10px;
      pointer-events: none;
    }

    #cover-left.open  { transform: rotateY(178deg); opacity: 0; pointer-events: none; }
    #cover-right.open { transform: rotateY(-178deg); opacity: 0; pointer-events: none; }

    .cover-heart {
      font-size: clamp(36px, 6vw, 52px);
      margin-bottom: 14px;
      animation: hb 1.5s ease-in-out infinite;
      filter: drop-shadow(0 0 12px rgba(255,80,80,0.6));
    }

    @keyframes hb { 0%,100%{transform:scale(1)} 50%{transform:scale(1.18)} }

    .cover-title {
      font-family: 'Cinzel', serif;
      color: #FFD700;
      font-size: clamp(13px, 2.2vw, 17px);
      text-align: center;
      padding: 0 20px;
      line-height: 1.7;
      text-shadow: 0 2px 8px rgba(0,0,0,0.5);
      letter-spacing: 0.05em;
    }

    .cover-hint {
      color: rgba(255,215,0,0.45);
      font-size: clamp(10px, 1.5vw, 12px);
      margin-top: 18px;
      font-style: italic;
      letter-spacing: 0.1em;
    }

    #spine {
      position: absolute;
      left: 50%; top: 0;
      transform: translateX(-50%);
      width: 26px; height: 100%;
      background: linear-gradient(to right, #2A0000, #5C0000, #3A0000);
      z-index: 35;
      box-shadow: 0 0 12px rgba(0,0,0,0.8);
    }

    #pages {
      position: absolute;
      top: 0; left: 0;
      width: 100%; height: 100%;
      display: flex;
      z-index: 5;
      opacity: 0;
      transition: opacity 0.6s ease 0.7s;
    }

    #pages.visible { opacity: 1; }

    .page {
      width: calc(50% - 13px);
      height: 100%;
      background: #FEFAF4;
      position: relative;
      overflow: hidden;
      padding: clamp(18px,3vw,28px) clamp(14px,2.5vw,22px) 16px;
      display: flex;
      flex-direction: column;
    }

    .page-left  { border-radius: 16px 0 0 16px; box-shadow: inset -4px 0 10px rgba(0,0,0,0.06); }
    .page-right { border-radius: 0 16px 16px 0; box-shadow: inset 4px 0 10px rgba(0,0,0,0.06); }

    .lined {
      position: absolute; top: 0; left: 0; right: 0; bottom: 0;
      background-image: repeating-linear-gradient(transparent, transparent 30px, #E0CDB8 30px, #E0CDB8 31px);
      background-position: 0 48px;
      opacity: 0.5;
      pointer-events: none;
    }

    .page-num {
      position: absolute;
      bottom: 10px;
      font-size: 11px;
      color: #C0A080;
      font-family: 'Cinzel', serif;
      letter-spacing: 0.1em;
    }
    .page-left  .page-num { left: 18px; }
    .page-right .page-num { right: 18px; }

    .typed-area {
      color: #2D1500;
      font-size: clamp(12px,1.8vw,14px);
      line-height: 2.07;
      position: relative;
      z-index: 2;
      flex: 1;
      font-family: 'Lora', Georgia, serif;
    }

    .cursor {
      display: inline-block;
      width: 2px; height: 14px;
      background: #8B1A1A;
      margin-left: 1px;
      animation: blink 0.7s step-end infinite;
      vertical-align: middle;
    }
    @keyframes blink { 0%,100%{opacity:1} 50%{opacity:0} }

    #question-section {
      position: relative; z-index: 2;
      margin-top: 12px;
      opacity: 0;
      transition: opacity 0.9s ease;
      text-align: center;
    }
    #question-section.visible { opacity: 1; }
    #question-section p {
      font-size: clamp(11px,1.6vw,13px);
      color: #7B1111;
      font-style: italic;
      margin-bottom: 10px;
      font-weight: 500;
      font-family: 'Lora', serif;
    }

    .btn-row { display: flex; gap: 10px; justify-content: center; }

    .btn-yes, .btn-no {
      padding: 8px 22px; border: none; border-radius: 30px;
      font-size: clamp(11px,1.6vw,13px);
      font-family: 'Lora', Georgia, serif;
      cursor: pointer;
      transition: transform 0.15s, box-shadow 0.15s;
      letter-spacing: 0.05em;
    }

    .btn-yes {
      background: linear-gradient(135deg, #8B1A1A, #C0392B);
      color: #fff;
      box-shadow: 0 3px 12px rgba(139,26,26,0.4);
    }

    .btn-no {
      background: #E8D8C4;
      color: #5A3A1A;
      box-shadow: 0 2px 8px rgba(0,0,0,0.1);
    }

    .btn-yes:hover { transform: scale(1.06); box-shadow: 0 5px 16px rgba(139,26,26,0.5); }
    .btn-no:hover  { transform: scale(1.06); }

    #result-overlay {
      display: none;
      position: absolute;
      top: 0; left: 0;
      width: 100%; height: 100%;
      z-index: 20;
    }

    .res-page {
      position: absolute;
      top: 0; height: 100%;
      width: calc(50% - 13px);
      background: #FEFAF4;
      padding: clamp(18px,3vw,28px) clamp(14px,2.5vw,22px) 16px;
      overflow: hidden;
    }

    .res-page.left  { left: 0;  border-radius: 16px 0 0 16px; box-shadow: inset -4px 0 10px rgba(0,0,0,0.06); }
    .res-page.right { right: 0; border-radius: 0 16px 16px 0; box-shadow: inset 4px 0 10px rgba(0,0,0,0.06); display: flex; align-items: center; justify-content: center; flex-direction: column; }

    #result-typed {
      color: #2D1500;
      font-size: clamp(12px,1.8vw,14px);
      line-height: 2.07;
      position: relative; z-index: 2;
      font-family: 'Lora', serif;
    }

    #no-message {
      color: #2D1500;
      font-size: clamp(14px,2.2vw,18px);
      font-style: italic;
      text-align: center;
      line-height: 1.9;
      position: relative; z-index: 2;
      padding: 0 20px;
      opacity: 0;
      transition: opacity 1.4s ease;
      font-family: 'Lora', serif;
    }
    #no-message.visible { opacity: 1; }

    #hint {
      margin-top: 22px;
      font-size: clamp(11px,1.6vw,13px);
      color: rgba(255,215,0,0.45);
      font-style: italic;
      letter-spacing: 0.1em;
      opacity: 0;
      animation: fade-in 1.5s ease 1.2s forwards;
      position: relative;
      z-index: 2;
    }
  </style>
</head>
<body>

  <div class="particles" id="particles"></div>

  <div id="top-title">✦ Un mensaje para ti ✦</div>

  <div id="book-wrap">

    <div id="pages">
      <div class="page page-left">
        <div class="lined"></div>
        <div id="typed-left" class="typed-area"></div>
        <span class="page-num">I</span>
      </div>
      <div class="page page-right">
        <div class="lined"></div>
        <div id="typed-right" class="typed-area"></div>
        <div id="question-section">
          <p>¿Quieres que nos sigamos conociendo?</p>
          <div class="btn-row">
            <button class="btn-yes" onclick="chooseAnswer('si')">Sí ❤️</button>
            <button class="btn-no" onclick="chooseAnswer('no')">No</button>
          </div>
        </div>
        <span class="page-num">II</span>
      </div>
    </div>

    <div id="result-overlay">
      <div class="res-page left">
        <div class="lined"></div>
        <div id="result-typed"></div>
        <span style="position:absolute;bottom:10px;left:18px;font-size:11px;color:#C0A080;font-family:'Cinzel',serif;letter-spacing:0.1em;">III</span>
      </div>
      <div class="res-page right">
        <div class="lined"></div>
        <div id="no-message"></div>
      </div>
    </div>

    <div id="spine"></div>

    <div id="cover-left" onclick="openBook()">
      <div class="cover-heart">❤️</div>
      <div class="cover-title">Para ti,<br>con todo<br>mi corazón</div>
      <div class="cover-hint">Toca para abrir</div>
    </div>
    <div id="cover-right" onclick="openBook()">
      <div class="cover-heart">💌</div>
      <div class="cover-title">Un mensaje<br>desde el<br>alma</div>
      <div class="cover-hint">Toca para abrir</div>
    </div>

  </div>

  <div id="hint">— Toca cualquier tapa para abrir el libro —</div>

  <script>
    const container = document.getElementById('particles');
    for (let i = 0; i < 28; i++) {
      const p = document.createElement('div');
      p.className = 'particle';
      p.style.left = Math.random() * 100 + '%';
      p.style.animationDuration = (6 + Math.random() * 10) + 's';
      p.style.animationDelay = (Math.random() * 12) + 's';
      const size = (2 + Math.random() * 3) + 'px';
      p.style.width = size;
      p.style.height = size;
      container.appendChild(p);
    }

    const leftSegs = [
      "Quiero que sepas que te quiero muchísimo.",
      " Si estás pasando por un mal momento, entiendo",
      " y te doy tu espacio,",
      " pero si ya no quieres seguir hablando,",
      " por favor dímelo con sinceridad.",
      " Con lo que me diste a entender con tu mensaje",
      " es que alguien más te gustaba.",
      " Desde que te fui conociendo,",
      " eres la única chica que me ha ido",
      " enamorando más y más.",
      " Es un sentimiento bonito",
      " y me encantaría compartirlo contigo."
    ];

    const rightSegs = [
      "No sé qué hice para molestarte,",
      " porque todo lo que hago es para demostrarte",
      " lo mucho que te quiero.",
      " Seguiré haciéndolo,",
      " pero solo hasta donde tú me lo permitas.",
      " Dime si hay algo que te moleste,",
      " porque estoy aquí para escucharte.",
      " Te hablo desde la sinceridad de mi corazón",
      " y lo que te incomode,",
      " dime y lo arreglamos juntos."
    ];

    const siSegs = [
      "Si quieres seguir hablando conmigo,",
      " quiero que sepas que mi cariño por ti es real",
      " y siempre va a estar ahí, sin presionarte.",
      " Me gusta compartir contigo,",
      " conocerte más",
      " y seguir construyendo algo bonito,",
      " siempre respetando tu espacio",
      " y lo que tú sientas.",
      " No quiero que sientas ninguna carga,",
      " solo que estés tranquila siendo tú,",
      " y que sepas que conmigo siempre vas a tener",
      " respeto, sinceridad",
      " y alguien que te aprecia de verdad."
    ];

    let opened = false;

    function openBook() {
      if (opened) return;
      opened = true;
      document.getElementById('cover-left').classList.add('open');
      document.getElementById('cover-right').classList.add('open');
      document.getElementById('pages').classList.add('visible');
      document.getElementById('hint').style.opacity = '0';
      setTimeout(() => {
        type(leftSegs, 'typed-left', () => {
          type(rightSegs, 'typed-right', showQ);
        });
      }, 950);
    }

    function type(segs, elId, onDone, si=0, ci=0) {
      const el = document.getElementById(elId);
      if (!el) return;
      if (si === 0 && ci === 0) el.innerHTML = '<span class="cursor"></span>';
      if (si >= segs.length) {
        const c = el.querySelector('.cursor');
        if (c) c.remove();
        if (onDone) onDone();
        return;
      }
      const seg = segs[si];
      if (ci < seg.length) {
        const cur = el.querySelector('.cursor');
        if (cur) cur.insertAdjacentText('beforebegin', seg[ci]);
        else el.appendChild(document.createTextNode(seg[ci]));
        setTimeout(() => type(segs, elId, onDone, si, ci+1), 36);
      } else {
        const delay = seg.trimEnd().endsWith('.') ? 500 : 25;
        setTimeout(() => type(segs, elId, onDone, si+1, 0), delay);
      }
    }

    function showQ() {
      document.getElementById('question-section').classList.add('visible');
    }

    function chooseAnswer(choice) {
      document.getElementById('question-section').style.display = 'none';
      document.getElementById('result-overlay').style.display = 'block';

      if (choice === 'si') {
        type(siSegs, 'result-typed', () => sendEmail('si'));
      } else {
        document.getElementById('result-typed').innerHTML = '';
        const noMsg = document.getElementById('no-message');
        noMsg.textContent = 'Esto lo quiero hablar contigo.';
        setTimeout(() => {
          noMsg.classList.add('visible');
          sendEmail('no');
        }, 400);
      }
    }

    function sendEmail(choice) {
      const label = choice === 'si' ? 'SÍ ❤️' : 'NO — quiere hablarlo contigo';
      const sub = encodeURIComponent('Respuesta del libro: ' + (choice === 'si' ? 'SÍ ❤️' : 'NO'));
      const bod = encodeURIComponent(
        'Ella respondió: ' + label +
        '\n\nFecha: ' + new Date().toLocaleString('es-PY')
      );
      setTimeout(() => {
        window.location.href = 'mailto:tdarkgod333@gmail.com?subject=' + sub + '&body=' + bod;
      }, choice === 'no' ? 1800 : 800);
    }
  </script>

</body>
</html>

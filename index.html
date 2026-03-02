# Realms<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8"/>
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Realm Forge — Fantasy Map Generator</title>
  <link href="https://fonts.googleapis.com/css2?family=MedievalSharp&family=Cinzel:wght@400;600;700&family=Crimson+Text:ital,wght@0,400;0,600;1,400&display=swap" rel="stylesheet"/>
  <style>
    *,*::before,*::after{box-sizing:border-box;margin:0;padding:0}

    :root{
      --parchment:#f4e4c1;
      --parchment-dark:#e8d5a3;
      --parchment-darker:#d4b896;
      --ink:#2c1810;
      --ink-soft:#4a2e1a;
      --ink-muted:#7a5c3a;
      --ink-faded:#a08060;
      --accent:#8b2020;
      --accent-gold:#c8962a;
      --water:#5a8fa8;
      --water-light:#89b8cc;
      --forest:#4a7a3a;
      --mountain:#7a6a5a;
      --desert:#c8a050;
      --shadow:rgba(44,24,16,0.3);
    }

    body{
      font-family:'Crimson Text',serif;
      background:#1a0e08;
      color:var(--ink);
      min-height:100vh;
      overflow-x:hidden;
    }

    /* Outer wooden frame effect */
    body::before{
      content:'';
      position:fixed;
      inset:0;
      background:
        radial-gradient(ellipse at center, #2a1508 0%, #0d0604 100%);
      z-index:0;
    }

    .page{
      position:relative;
      z-index:1;
      max-width:1100px;
      margin:0 auto;
      padding:24px 16px 48px;
    }

    /* Header */
    header{
      text-align:center;
      margin-bottom:28px;
      animation:fadeDown 0.8s ease both;
    }

    .site-title{
      font-family:'Cinzel',serif;
      font-size:clamp(2rem,6vw,3.4rem);
      font-weight:700;
      color:var(--accent-gold);
      text-shadow:2px 2px 0 #2c1810, 0 0 40px rgba(200,150,42,0.3);
      letter-spacing:0.06em;
      line-height:1;
    }

    .site-subtitle{
      font-family:'Crimson Text',serif;
      font-style:italic;
      font-size:1.05rem;
      color:var(--ink-faded);
      margin-top:6px;
      letter-spacing:0.1em;
    }

    .divider{
      display:flex;
      align-items:center;
      gap:12px;
      margin:14px auto;
      max-width:400px;
    }

    .divider-line{
      flex:1;
      height:1px;
      background:linear-gradient(to right, transparent, var(--accent-gold), transparent);
    }

    .divider-icon{color:var(--accent-gold);font-size:1.1rem;}

    /* Main layout */
    .main-layout{
      display:grid;
      grid-template-columns:260px 1fr;
      gap:20px;
      align-items:start;
    }

    @media(max-width:700px){
      .main-layout{grid-template-columns:1fr;}
    }

    /* Controls panel */
    .controls-panel{
      background:var(--parchment);
      border:2px solid var(--parchment-darker);
      border-radius:4px;
      padding:20px 16px;
      box-shadow:4px 4px 16px var(--shadow), inset 0 0 40px rgba(200,150,42,0.08);
      position:relative;
      animation:fadeUp 0.8s 0.1s ease both;
    }

    .controls-panel::before{
      content:'';
      position:absolute;
      inset:4px;
      border:1px solid var(--parchment-darker);
      border-radius:2px;
      pointer-events:none;
      opacity:0.5;
    }

    .panel-title{
      font-family:'Cinzel',serif;
      font-size:0.85rem;
      font-weight:600;
      color:var(--accent);
      letter-spacing:0.12em;
      text-transform:uppercase;
      text-align:center;
      margin-bottom:16px;
      padding-bottom:10px;
      border-bottom:1px solid var(--parchment-darker);
    }

    .control-group{
      margin-bottom:16px;
    }

    .control-label{
      font-family:'Cinzel',serif;
      font-size:0.72rem;
      font-weight:600;
      color:var(--ink-soft);
      letter-spacing:0.1em;
      text-transform:uppercase;
      margin-bottom:5px;
      display:block;
    }

    select{
      width:100%;
      padding:8px 10px;
      font-family:'Crimson Text',serif;
      font-size:0.95rem;
      color:var(--ink);
      background:var(--parchment-dark);
      border:1px solid var(--parchment-darker);
      border-radius:2px;
      outline:none;
      appearance:none;
      cursor:pointer;
      background-image:url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='10' height='6'%3E%3Cpath d='M0 0l5 6 5-6z' fill='%234a2e1a'/%3E%3C/svg%3E");
      background-repeat:no-repeat;
      background-position:right 10px center;
      padding-right:28px;
      transition:border-color 0.2s;
    }

    select:focus{border-color:var(--accent-gold);}

    /* Seed input */
    .seed-row{
      display:flex;
      gap:6px;
      align-items:center;
    }

    .seed-input{
      flex:1;
      padding:8px 10px;
      font-family:'Crimson Text',serif;
      font-size:0.95rem;
      color:var(--ink);
      background:var(--parchment-dark);
      border:1px solid var(--parchment-darker);
      border-radius:2px;
      outline:none;
      transition:border-color 0.2s;
    }

    .seed-input:focus{border-color:var(--accent-gold);}

    .seed-random-btn{
      padding:8px 10px;
      background:var(--parchment-darker);
      border:1px solid var(--ink-faded);
      border-radius:2px;
      cursor:pointer;
      font-size:0.9rem;
      color:var(--ink-soft);
      transition:background 0.2s;
    }

    .seed-random-btn:hover{background:var(--accent-gold);color:var(--ink);}

    /* Generate button */
    .generate-btn{
      width:100%;
      margin-top:20px;
      padding:14px;
      background:var(--accent);
      color:var(--parchment);
      border:2px solid #5a1010;
      border-radius:3px;
      font-family:'Cinzel',serif;
      font-size:1rem;
      font-weight:600;
      letter-spacing:0.1em;
      cursor:pointer;
      transition:background 0.2s, transform 0.1s, box-shadow 0.2s;
      box-shadow:2px 2px 8px var(--shadow);
      text-transform:uppercase;
      position:relative;
      overflow:hidden;
    }

    .generate-btn:hover{
      background:#a02828;
      box-shadow:3px 3px 14px var(--shadow);
    }

    .generate-btn:active{transform:scale(0.98);}
    .generate-btn.loading{pointer-events:none;opacity:0.8;}

    /* Export button */
    .export-btn{
      width:100%;
      margin-top:8px;
      padding:10px;
      background:transparent;
      color:var(--ink-soft);
      border:1px solid var(--parchment-darker);
      border-radius:3px;
      font-family:'Cinzel',serif;
      font-size:0.8rem;
      font-weight:600;
      letter-spacing:0.08em;
      cursor:pointer;
      transition:all 0.2s;
      text-transform:uppercase;
    }

    .export-btn:hover{background:var(--parchment-darker);color:var(--ink);}

    /* Map container */
    .map-container{
      background:var(--parchment);
      border:3px solid var(--parchment-darker);
      border-radius:4px;
      box-shadow:6px 6px 24px var(--shadow), inset 0 0 60px rgba(200,150,42,0.1);
      position:relative;
      overflow:hidden;
      animation:fadeUp 0.8s 0.2s ease both;
    }

    .map-container::before{
      content:'';
      position:absolute;
      inset:6px;
      border:1px solid var(--parchment-darker);
      pointer-events:none;
      z-index:10;
      opacity:0.6;
    }

    canvas{
      display:block;
      width:100%;
      height:auto;
    }

    /* Map legend */
    .map-legend{
      position:absolute;
      bottom:20px;
      right:20px;
      background:rgba(244,228,193,0.92);
      border:1px solid var(--parchment-darker);
      padding:10px 12px;
      border-radius:2px;
      z-index:20;
      min-width:110px;
    }

    .legend-title{
      font-family:'Cinzel',serif;
      font-size:0.65rem;
      font-weight:600;
      color:var(--ink-soft);
      letter-spacing:0.1em;
      text-transform:uppercase;
      margin-bottom:6px;
      text-align:center;
    }

    .legend-item{
      display:flex;
      align-items:center;
      gap:6px;
      font-size:0.75rem;
      color:var(--ink-soft);
      margin-bottom:3px;
      font-family:'Crimson Text',serif;
    }

    .legend-swatch{
      width:14px;
      height:14px;
      border-radius:2px;
      border:1px solid rgba(44,24,16,0.2);
      flex-shrink:0;
    }

    /* Map compass */
    .map-compass{
      position:absolute;
      top:20px;
      right:20px;
      z-index:20;
      font-size:2.2rem;
      color:var(--ink-soft);
      text-shadow:1px 1px 0 var(--parchment);
      opacity:0.7;
      user-select:none;
    }

    /* Map title overlay */
    .map-title-overlay{
      position:absolute;
      top:16px;
      left:0;
      right:0;
      text-align:center;
      z-index:20;
      pointer-events:none;
    }

    .map-title-text{
      font-family:'Cinzel',serif;
      font-size:clamp(0.9rem,2.5vw,1.3rem);
      font-weight:700;
      color:var(--ink);
      text-shadow:1px 1px 0 var(--parchment);
      letter-spacing:0.08em;
    }

    /* Empty state */
    .map-empty{
      position:absolute;
      inset:0;
      display:flex;
      flex-direction:column;
      align-items:center;
      justify-content:center;
      color:var(--ink-faded);
      text-align:center;
      padding:40px;
    }

    .map-empty-icon{font-size:3rem;margin-bottom:12px;opacity:0.5;}

    .map-empty-text{
      font-family:'Cinzel',serif;
      font-size:1rem;
      letter-spacing:0.06em;
      opacity:0.7;
    }

    .map-empty-sub{
      font-style:italic;
      font-size:0.88rem;
      margin-top:6px;
      opacity:0.5;
    }

    /* Info bar */
    .info-bar{
      margin-top:10px;
      padding:8px 14px;
      background:rgba(244,228,193,0.15);
      border:1px solid rgba(200,150,42,0.2);
      border-radius:3px;
      display:flex;
      justify-content:space-between;
      align-items:center;
      flex-wrap:wrap;
      gap:8px;
      animation:fadeUp 0.8s 0.3s ease both;
    }

    .info-text{
      font-family:'Crimson Text',serif;
      font-style:italic;
      font-size:0.85rem;
      color:var(--ink-faded);
    }

    .seed-display{
      font-family:'Crimson Text',serif;
      font-size:0.8rem;
      color:var(--ink-faded);
    }

    @keyframes fadeDown{from{opacity:0;transform:translateY(-16px)}to{opacity:1;transform:translateY(0)}}
    @keyframes fadeUp{from{opacity:0;transform:translateY(16px)}to{opacity:1;transform:translateY(0)}}
  </style>
</head>
<body>
<div class="page">
  <header>
    <div class="site-title">⚔ Realm Forge ⚔</div>
    <div class="divider">
      <div class="divider-line"></div>
      <div class="divider-icon">✦</div>
      <div class="divider-line"></div>
    </div>
    <div class="site-subtitle">Fantasy Map Generator for TTRPGs &amp; World Building</div>
  </header>

  <div class="main-layout">
    <!-- Controls -->
    <div class="controls-panel">
      <div class="panel-title">⚙ Map Parameters</div>

      <div class="control-group">
        <label class="control-label">Map Size</label>
        <select id="mapSize">
          <option value="small">Small — Dungeon / Town</option>
          <option value="medium" selected>Medium — Region / Province</option>
          <option value="large">Large — Full Continent</option>
        </select>
      </div>

      <div class="control-group">
        <label class="control-label">Land Mass Type</label>
        <select id="landType">
          <option value="continent">Continent</option>
          <option value="island">Island / Archipelago</option>
          <option value="peninsula">Peninsula</option>
          <option value="inland">Inland Region</option>
          <option value="random">Random</option>
        </select>
      </div>

      <div class="control-group">
        <label class="control-label">Primary Terrain</label>
        <select id="terrain">
          <option value="mixed">Mixed Terrain</option>
          <option value="forest">Dense Forest</option>
          <option value="mountains">Mountain Range</option>
          <option value="desert">Arid Desert</option>
          <option value="plains">Rolling Plains</option>
          <option value="tundra">Frozen Tundra</option>
          <option value="swamp">Swampland</option>
          <option value="volcanic">Volcanic Wastes</option>
        </select>
      </div>

      <div class="control-group">
        <label class="control-label">Water Bodies</label>
        <select id="water">
          <option value="moderate">Moderate — Rivers &amp; Lakes</option>
          <option value="abundant">Abundant — Many Waterways</option>
          <option value="coastal">Coastal — Ocean Borders</option>
          <option value="rivers">Rivers Only</option>
          <option value="lakes">Lakes &amp; Ponds Only</option>
          <option value="arid">Arid — Minimal Water</option>
          <option value="archipelago">Archipelago — Many Seas</option>
        </select>
      </div>

      <div class="control-group">
        <label class="control-label">Settlements</label>
        <select id="settlements">
          <option value="few">Few — Wilderness</option>
          <option value="moderate" selected>Moderate — Settled Land</option>
          <option value="many">Many — Civilized Region</option>
          <option value="none">None — Untamed Wild</option>
        </select>
      </div>

      <div class="control-group">
        <label class="control-label">Map Seed (optional)</label>
        <div class="seed-row">
          <input type="text" class="seed-input" id="seedInput" placeholder="e.g. 42069"/>
          <button class="seed-random-btn" id="randomSeedBtn" title="Random seed">🎲</button>
        </div>
      </div>

      <button class="generate-btn" id="generateBtn">⚔ Generate Map</button>
      <button class="export-btn" id="exportBtn">↓ Save as Image</button>
    </div>

    <!-- Map -->
    <div>
      <div class="map-container" id="mapContainer">
        <canvas id="mapCanvas"></canvas>
        <div class="map-empty" id="mapEmpty">
          <div class="map-empty-icon">🗺</div>
          <div class="map-empty-text">Your realm awaits</div>
          <div class="map-empty-sub">Set your parameters and forge a world</div>
        </div>
        <div class="map-compass" id="mapCompass" style="display:none">🧭</div>
        <div class="map-title-overlay" id="mapTitleOverlay" style="display:none">
          <div class="map-title-text" id="mapTitleText"></div>
        </div>
        <div class="map-legend" id="mapLegend" style="display:none">
          <div class="legend-title">Legend</div>
          <div id="legendItems"></div>
        </div>
      </div>

      <div class="info-bar">
        <div class="info-text" id="infoText">Choose your parameters and generate a map to begin your adventure.</div>
        <div class="seed-display" id="seedDisplay"></div>
      </div>
    </div>
  </div>
</div>

<script>
// ─── Seeded RNG (Mulberry32) ───────────────────────────────────────────────
function createRNG(seed) {
  let s = seed >>> 0;
  return function() {
    s += 0x6D2B79F5;
    let t = Math.imul(s ^ s >>> 15, 1 | s);
    t ^= t + Math.imul(t ^ t >>> 7, 61 | t);
    return ((t ^ t >>> 14) >>> 0) / 4294967296;
  };
}

// ─── Noise (simple value noise) ───────────────────────────────────────────
function makeNoise(rng, w, h) {
  const grid = [];
  for(let y=0;y<h;y++){grid[y]=[];for(let x=0;x<w;x++) grid[y][x]=rng();}
  function lerp(a,b,t){return a+(b-a)*t;}
  function smooth(t){return t*t*(3-2*t);}
  return function(x,y) {
    const xi=Math.floor(x)%w, yi=Math.floor(y)%h;
    const xf=x-Math.floor(x), yf=y-Math.floor(y);
    const x1=(xi+1)%w, y1=(yi+1)%h;
    return lerp(
      lerp(grid[yi][xi],grid[yi][x1],smooth(xf)),
      lerp(grid[y1][xi],grid[y1][x1],smooth(xf)),
      smooth(yf)
    );
  };
}

function fbm(noise,x,y,octaves=5){
  let v=0,amp=0.5,freq=1,max=0;
  for(let i=0;i<octaves;i++){v+=noise(x*freq,y*freq)*amp;max+=amp;amp*=0.5;freq*=2;}
  return v/max;
}

// ─── Map names ────────────────────────────────────────────────────────────
const PREFIXES=['Aether','Brim','Cael','Drak','Eld','Fae','Grim','Helm','Iron','Jade','Kael','Lorn','Mor','Neth','Orm','Pyre','Quel','Raven','Stone','Thorn','Ul','Vale','Wych','Xan','Yor','Zeph'];
const SUFFIXES=['haven','moor','fell','reach','hold','gate','shire','mere','wald','dun','heim','keep','vale','ford','mark','fen','spire','watch','crest','deep'];

const SETTLEMENT_NAMES=['Ashford','Brackwater','Coldmere','Dusthaven','Elderwick','Frostgate','Grimhold','Harrowfen','Ironspire','Jadekeep','Kaldrath','Lornswick','Mirefall','Nethgate','Oldwatch','Pyremont','Quelford','Ravenstone','Stonegate','Thornwick','Ulvenmoor','Valeford','Wychwood','Xandrel','Yorkstead','Zephyrhold','Ashwick','Blackmere','Cresthold','Dustwick'];

// ─── Canvas setup ─────────────────────────────────────────────────────────
const canvas = document.getElementById('mapCanvas');
const ctx = canvas.getContext('2d');
const SIZES = { small:{w:600,h:450,label:'Dungeon / Town'}, medium:{w:800,h:600,label:'Region / Province'}, large:{w:1000,h:750,label:'Full Continent'} };

let lastSeed = null;

// ─── Main generator ───────────────────────────────────────────────────────
function generateMap() {
  const sizeKey = document.getElementById('mapSize').value;
  const landType = document.getElementById('landType').value;
  const terrain = document.getElementById('terrain').value;
  const waterType = document.getElementById('water').value;
  const settlements = document.getElementById('settlements').value;
  const seedVal = document.getElementById('seedInput').value.trim();

  const seed = seedVal ? hashStr(seedVal) : Math.floor(Math.random()*2147483647);
  lastSeed = seed;
  document.getElementById('seedInput').value = seed;
  document.getElementById('seedDisplay').textContent = `Seed: ${seed}`;

  const rng = createRNG(seed);
  const sz = SIZES[sizeKey];
  canvas.width = sz.w;
  canvas.height = sz.h;

  // Hide empty state, show map elements
  document.getElementById('mapEmpty').style.display = 'none';
  document.getElementById('mapCompass').style.display = 'block';
  document.getElementById('mapTitleOverlay').style.display = 'block';
  document.getElementById('mapLegend').style.display = 'block';

  // Generate map name
  const mapName = PREFIXES[Math.floor(rng()*PREFIXES.length)] + SUFFIXES[Math.floor(rng()*SUFFIXES.length)];
  document.getElementById('mapTitleText').textContent = `The Realm of ${mapName}`;

  const W = sz.w, H = sz.h;

  // ── Generate heightmap ──
  const noiseGrid = makeNoise(rng, 64, 64);
  const heightmap = [];
  for(let y=0;y<H;y++){
    heightmap[y]=[];
    for(let x=0;x<W;x++){
      const nx=x/W*8, ny=y/H*8;
      let h = fbm(noiseGrid,nx,ny,6);
      // Apply land type shaping
      if(landType==='island'||landType==='archipelago'){
        const dx=(x/W-0.5)*2, dy=(y/H-0.5)*2;
        const dist=Math.sqrt(dx*dx+dy*dy);
        h -= dist*0.7;
      } else if(landType==='peninsula'){
        const dx=x/W, dy=(y/H-0.5)*2;
        h -= Math.abs(dy)*0.4 + (1-dx)*0.3;
      } else if(landType==='coastal'){
        h -= (1-x/W)*0.5;
      } else if(landType==='inland'){
        const dx=(x/W-0.5)*2, dy=(y/H-0.5)*2;
        h += 0.2 - Math.sqrt(dx*dx+dy*dy)*0.15;
      }
      heightmap[y][x]=Math.max(0,Math.min(1,h));
    }
  }

  // Water threshold
  let waterThresh = 0.42;
  if(waterType==='arid') waterThresh=0.3;
  else if(waterType==='abundant'||waterType==='archipelago') waterThresh=0.52;
  else if(waterType==='coastal') waterThresh=0.45;

  // ── Draw base parchment ──
  const parchment = ctx.createLinearGradient(0,0,W,H);
  parchment.addColorStop(0,'#f5e6c4');
  parchment.addColorStop(0.3,'#f0ddb5');
  parchment.addColorStop(0.7,'#ecdaa8');
  parchment.addColorStop(1,'#e8d49e');
  ctx.fillStyle = parchment;
  ctx.fillRect(0,0,W,H);

  // Parchment texture noise
  for(let i=0;i<W*H*0.15;i++){
    const px=Math.floor(rng()*W), py=Math.floor(rng()*H);
    const a=rng()*0.06;
    ctx.fillStyle=`rgba(${rng()>0.5?180:140},${rng()>0.5?130:100},60,${a})`;
    ctx.fillRect(px,py,1+(rng()*2|0),1+(rng()*2|0));
  }

  // ── Draw terrain ──
  const imgData = ctx.getImageData(0,0,W,H);
  const data = imgData.data;

  for(let y=0;y<H;y++){
    for(let x=0;x<W;x++){
      const h=heightmap[y][x];
      const i=(y*W+x)*4;
      let r,g,b,a=255;

      if(h < waterThresh-0.08){
        // Deep water
        r=60;g=90;b=130;
      } else if(h < waterThresh){
        // Shallow water
        r=100;g=140;b=170;
      } else {
        // Land — apply terrain coloring
        const landH=(h-waterThresh)/(1-waterThresh);
        switch(terrain){
          case 'forest':
            r=Math.floor(60+landH*30);g=Math.floor(90+landH*40);b=Math.floor(50+landH*20);break;
          case 'mountains':
            if(landH>0.65){r=200;g=195;b=190;}
            else if(landH>0.4){r=140;g=120;b=100;}
            else{r=120;g=140;b=90;}
            break;
          case 'desert':
            r=Math.floor(195+landH*40);g=Math.floor(160+landH*30);b=Math.floor(80+landH*20);break;
          case 'tundra':
            r=Math.floor(200+landH*50);g=Math.floor(210+landH*40);b=Math.floor(220+landH*30);break;
          case 'swamp':
            r=Math.floor(70+landH*30);g=Math.floor(90+landH*40);b=Math.floor(60+landH*20);break;
          case 'volcanic':
            if(landH>0.7){r=220;g=80;b=30;}
            else{r=Math.floor(60+landH*50);g=Math.floor(40+landH*30);b=Math.floor(40+landH*20);}
            break;
          case 'plains':
            r=Math.floor(160+landH*40);g=Math.floor(170+landH*30);b=Math.floor(80+landH*20);break;
          default: // mixed
            if(landH>0.75){r=180;g=175;b=170;}
            else if(landH>0.5){r=130;g=115;b=90;}
            else if(landH>0.25){r=100;g=130;b=75;}
            else{r=140;g=160;b=100;}
        }
        // Blend toward parchment
        const blend=0.38;
        r=Math.floor(r*(1-blend)+210*blend);
        g=Math.floor(g*(1-blend)+185*blend);
        b=Math.floor(b*(1-blend)+140*blend);
      }

      data[i]=r; data[i+1]=g; data[i+2]=b; data[i+3]=a;
    }
  }
  ctx.putImageData(imgData,0,0);

  // ── Draw rivers ──
  if(waterType!=='arid'&&waterType!=='lakes'){
    const numRivers = waterType==='abundant'||waterType==='rivers'?6:3;
    ctx.strokeStyle='rgba(80,120,160,0.7)';
    for(let r=0;r<numRivers;r++){
      // Find high point to start river
      let sx=Math.floor(rng()*W*0.6+W*0.2);
      let sy=Math.floor(rng()*H*0.3);
      // Make sure start is on land
      if(heightmap[sy]&&heightmap[sy][sx]<waterThresh+0.1) continue;
      ctx.beginPath();
      ctx.moveTo(sx,sy);
      let cx2=sx,cy2=sy;
      for(let step=0;step<200;step++){
        // Flow downhill with some meandering
        let bestX=cx2,bestY=cy2,bestH=heightmap[cy2]&&heightmap[cy2][cx2]||0;
        const dirs=[[-1,-1],[0,-1],[1,-1],[-1,0],[1,0],[-1,1],[0,1],[1,1]];
        for(const [dx2,dy2] of dirs){
          const nx2=cx2+dx2,ny2=cy2+dy2;
          if(nx2<0||nx2>=W||ny2<0||ny2>=H) continue;
          const nh=heightmap[ny2][nx2];
          if(nh<bestH){bestH=nh;bestX=nx2;bestY=ny2;}
        }
        // Add slight meander
        bestX+=Math.floor((rng()-0.5)*4);
        bestX=Math.max(0,Math.min(W-1,bestX));
        cx2=bestX;cy2=bestY;
        const wid=(heightmap[cy2][cx2]<waterThresh)?3:1.2;
        ctx.lineWidth=wid;
        ctx.lineTo(cx2,cy2);
        if(heightmap[cy2][cx2]<waterThresh-0.05) break;
      }
      ctx.stroke();
    }
  }

  // ── Draw lakes ──
  if(waterType==='lakes'||waterType==='moderate'||waterType==='abundant'){
    const numLakes = waterType==='abundant'?5:waterType==='lakes'?6:2;
    for(let l=0;l<numLakes;l++){
      const lx=Math.floor(rng()*W*0.7+W*0.15);
      const ly=Math.floor(rng()*H*0.7+H*0.15);
      if(heightmap[ly]&&heightmap[ly][lx]<waterThresh+0.05) continue;
      const lw=Math.floor(20+rng()*50), lh2=Math.floor(15+rng()*35);
      ctx.fillStyle='rgba(80,130,170,0.65)';
      ctx.strokeStyle='rgba(60,100,140,0.5)';
      ctx.lineWidth=1.5;
      ctx.beginPath();
      ctx.ellipse(lx,ly,lw,lh2,rng()*Math.PI,0,Math.PI*2);
      ctx.fill();ctx.stroke();
    }
  }

  // ── Draw mountain symbols ──
  const drawMountain=(mx,my,size)=>{
    ctx.strokeStyle='rgba(60,40,20,0.6)';
    ctx.fillStyle='rgba(150,130,110,0.4)';
    ctx.lineWidth=1;
    // Main peak
    ctx.beginPath();
    ctx.moveTo(mx,my-size);
    ctx.lineTo(mx-size*0.8,my+size*0.4);
    ctx.lineTo(mx+size*0.8,my+size*0.4);
    ctx.closePath();ctx.fill();ctx.stroke();
    // Snow cap
    ctx.fillStyle='rgba(240,238,235,0.7)';
    ctx.beginPath();
    ctx.moveTo(mx,my-size);
    ctx.lineTo(mx-size*0.25,my-size*0.45);
    ctx.lineTo(mx+size*0.25,my-size*0.45);
    ctx.closePath();ctx.fill();
  };

  if(terrain==='mountains'||terrain==='mixed'||terrain==='volcanic'){
    const numMts = terrain==='mountains'?25:12;
    for(let m=0;m<numMts;m++){
      const mx=Math.floor(rng()*W), my=Math.floor(rng()*H);
      if(!heightmap[my]||heightmap[my][mx]<waterThresh+0.2) continue;
      if(heightmap[my][mx]<0.65) continue;
      drawMountain(mx,my,8+rng()*12);
    }
  }

  // ── Draw tree symbols ──
  const drawTree=(tx,ty,size)=>{
    ctx.fillStyle='rgba(50,90,40,0.55)';
    ctx.beginPath();
    ctx.arc(tx,ty-size*0.3,size*0.6,0,Math.PI*2);
    ctx.fill();
    ctx.strokeStyle='rgba(40,70,30,0.4)';
    ctx.lineWidth=1;
    ctx.beginPath();ctx.moveTo(tx,ty-size*0.3+size*0.6);ctx.lineTo(tx,ty+size*0.5);ctx.stroke();
  };

  if(terrain==='forest'||terrain==='swamp'||(terrain==='mixed'&&rng()>0.3)){
    const numTrees=terrain==='forest'?80:terrain==='swamp'?40:30;
    for(let t=0;t<numTrees;t++){
      const tx=Math.floor(rng()*W), ty=Math.floor(rng()*H);
      if(!heightmap[ty]||heightmap[ty][tx]<waterThresh+0.02) continue;
      if(heightmap[ty][tx]>0.75) continue;
      drawTree(tx,ty,5+rng()*5);
    }
  }

  // ── Draw settlements ──
  const numSettlements = settlements==='none'?0:settlements==='few'?3:settlements==='many'?12:6;
  const usedNames=new Set();
  const settlementList=[];

  for(let s=0;s<numSettlements;s++){
    let attempts=0;
    while(attempts<50){
      const sx=Math.floor(rng()*W*0.8+W*0.1);
      const sy=Math.floor(rng()*H*0.8+H*0.1);
      if(!heightmap[sy]||heightmap[sy][sx]<waterThresh+0.03){attempts++;continue;}
      // Pick unique name
      let name;
      do{ name=SETTLEMENT_NAMES[Math.floor(rng()*SETTLEMENT_NAMES.length)]; }
      while(usedNames.has(name));
      usedNames.add(name);

      // Draw settlement dot
      const isCity=rng()>0.6;
      ctx.fillStyle='rgba(44,24,16,0.85)';
      ctx.strokeStyle='rgba(44,24,16,0.5)';
      if(isCity){
        ctx.lineWidth=1.5;
        ctx.beginPath();ctx.rect(sx-4,sy-4,8,8);ctx.fill();ctx.stroke();
      } else {
        ctx.beginPath();ctx.arc(sx,sy,3.5,0,Math.PI*2);ctx.fill();
      }

      // Settlement name
      ctx.font=`${isCity?'bold ':''} ${isCity?10:8.5}px 'Crimson Text', serif`;
      ctx.fillStyle='rgba(30,15,8,0.85)';
      ctx.textAlign='center';
      ctx.fillText(name,sx,sy-(isCity?8:7));

      settlementList.push({name,x:sx,y:sy,isCity});
      break;
      attempts++;
    }
  }

  // ── Parchment edge vignette ──
  const vignette=ctx.createRadialGradient(W/2,H/2,H*0.3,W/2,H/2,H*0.85);
  vignette.addColorStop(0,'rgba(0,0,0,0)');
  vignette.addColorStop(1,'rgba(44,24,16,0.35)');
  ctx.fillStyle=vignette;
  ctx.fillRect(0,0,W,H);

  // Edge burn effect
  const edgeBurn=ctx.createLinearGradient(0,0,0,H);
  edgeBurn.addColorStop(0,'rgba(44,24,16,0.25)');
  edgeBurn.addColorStop(0.05,'rgba(0,0,0,0)');
  edgeBurn.addColorStop(0.95,'rgba(0,0,0,0)');
  edgeBurn.addColorStop(1,'rgba(44,24,16,0.25)');
  ctx.fillStyle=edgeBurn;
  ctx.fillRect(0,0,W,H);

  // ── Draw decorative border ──
  ctx.strokeStyle='rgba(100,60,20,0.5)';
  ctx.lineWidth=3;
  ctx.strokeRect(8,8,W-16,H-16);
  ctx.strokeStyle='rgba(100,60,20,0.25)';
  ctx.lineWidth=1;
  ctx.strokeRect(12,12,W-24,H-24);

  // ── Corner decorations ──
  const corners=[[14,14],[W-14,14],[14,H-14],[W-14,H-14]];
  ctx.fillStyle='rgba(100,60,20,0.5)';
  corners.forEach(([cx3,cy3])=>{
    ctx.beginPath();ctx.arc(cx3,cy3,3,0,Math.PI*2);ctx.fill();
  });

  // ── Build legend ──
  const legendItems=[];
  if(waterType!=='arid') legendItems.push({color:'#5a8fa8',label:'Water'});
  legendItems.push({color:terrainColor(terrain),label:terrainLabel(terrain)});
  if(numSettlements>0) legendItems.push({color:'rgba(44,24,16,0.8)',label:'Settlement'});
  if(terrain==='mountains'||terrain==='mixed') legendItems.push({color:'rgba(150,130,110,0.8)',label:'Mountains'});

  const legendEl=document.getElementById('legendItems');
  legendEl.innerHTML=legendItems.map(item=>`
    <div class="legend-item">
      <div class="legend-swatch" style="background:${item.color}"></div>
      <span>${item.label}</span>
    </div>
  `).join('');

  // ── Update info bar ──
  document.getElementById('infoText').textContent=
    `${sz.label} · ${landTypeLabel(landType)} · ${terrainLabel(terrain)} · ${settlementList.length} settlement${settlementList.length!==1?'s':''}`;
}

function terrainColor(t){
  const map={forest:'#4a7a3a',mountains:'#7a6a5a',desert:'#c8a050',plains:'#a8b870',tundra:'#c8d8e0',swamp:'#4a5a3a',volcanic:'#603020',mixed:'#7a9060'};
  return map[t]||'#8a9868';
}

function terrainLabel(t){
  const map={forest:'Forest',mountains:'Mountains',desert:'Desert',plains:'Plains',tundra:'Tundra',swamp:'Swamp',volcanic:'Volcanic',mixed:'Mixed'};
  return map[t]||'Land';
}

function landTypeLabel(t){
  const map={continent:'Continent',island:'Island',peninsula:'Peninsula',inland:'Inland',random:'Mixed Land'};
  return map[t]||'Region';
}

function hashStr(str){
  let h=0;
  for(let i=0;i<str.length;i++){h=Math.imul(31,h)+str.charCodeAt(i)|0;}
  return Math.abs(h);
}

// ── Event listeners ──────────────────────────────────────────────────────
document.getElementById('generateBtn').addEventListener('click',()=>{
  const btn=document.getElementById('generateBtn');
  btn.classList.add('loading');
  btn.textContent='⏳ Forging Realm…';
  setTimeout(()=>{
    generateMap();
    btn.classList.remove('loading');
    btn.textContent='⚔ Generate Map';
  },50);
});

document.getElementById('randomSeedBtn').addEventListener('click',()=>{
  document.getElementById('seedInput').value=Math.floor(Math.random()*999999);
});

document.getElementById('exportBtn').addEventListener('click',()=>{
  const link=document.createElement('a');
  link.download='realmforge-map.png';
  link.href=canvas.toDataURL('image/png');
  link.click();
});
</script>
</body>
</html>

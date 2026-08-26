<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>ODP Admin</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Big+Shoulders+Display:wght@600;700;800&family=Space+Mono:wght@400;700&family=Inter:wght@400;500;600&display=swap" rel="stylesheet">
<style>
  :root{
    --ink:#16181A; --paper:#EDEBE3; --paper-soft:#F6F4ED; --paper-deep:#E3E0D6;
    --signal:#FF5A36; --gold:#C9A227; --slate:#6B7280; --green:#3E7C59; --line:rgba(22,24,26,0.14);
  }
  *{box-sizing:border-box; margin:0; padding:0;}
  body{background:var(--paper); color:var(--ink); font-family:'Inter',sans-serif; -webkit-font-smoothing:antialiased;}
  .mono{font-family:'Space Mono',monospace;}
  .display{font-family:'Big Shoulders Display',sans-serif; text-transform:uppercase;}
  a{color:inherit; text-decoration:none;}

  /* ---------- LOGIN ---------- */
  #loginScreen{
    min-height:100vh; display:flex; align-items:center; justify-content:center; padding:20px;
    background:radial-gradient(circle at 30% 20%, #24211c, #16181A 60%);
  }
  .login-card{
    width:380px; max-width:100%; background:var(--paper); border-radius:3px; padding:38px 34px;
    box-shadow:0 40px 80px rgba(0,0,0,0.4);
  }
  .login-logo{display:flex; align-items:center; gap:10px; justify-content:center; margin-bottom:6px;}
  .logo-mark{
    width:32px; height:32px; border:2px solid var(--ink); border-radius:50%; display:flex; align-items:center;
    justify-content:center; font-family:'Space Mono',monospace; font-weight:700; font-size:12px;
  }
  .login-logo-text{font-family:'Big Shoulders Display',sans-serif; font-weight:800; font-size:26px;}
  .login-sub{text-align:center; color:var(--slate); font-size:12px; letter-spacing:1px; text-transform:uppercase; margin-bottom:30px;}

  .oauth-btn{
    width:100%; display:flex; align-items:center; justify-content:center; gap:10px; padding:13px;
    border:1px solid var(--line); background:#fff; border-radius:2px; font-size:14px; font-weight:500;
    cursor:pointer; margin-bottom:10px; transition:border-color .15s;
  }
  .oauth-btn:hover{border-color:var(--ink);}
  .oauth-btn svg{width:18px; height:18px;}

  .divider{display:flex; align-items:center; gap:12px; margin:20px 0; color:var(--slate); font-size:11px; text-transform:uppercase; letter-spacing:1px;}
  .divider::before, .divider::after{content:''; flex:1; height:1px; background:var(--line);}

  .field{margin-bottom:14px;}
  .field label{font-size:11px; letter-spacing:0.5px; text-transform:uppercase; color:var(--slate); display:block; margin-bottom:6px;}
  .field input{
    width:100%; border:1px solid var(--line); background:var(--paper-soft); padding:12px 14px; border-radius:2px;
    font-family:'Inter',sans-serif; font-size:14px; outline:none;
  }
  .field input:focus{border-color:var(--ink);}
  .login-btn{
    width:100%; background:var(--ink); color:var(--paper); border:none; padding:14px; border-radius:2px;
    font-weight:600; font-size:14px; cursor:pointer; margin-top:6px;
  }
  .login-error{color:var(--signal); font-size:12px; margin-top:10px; text-align:center; display:none;}
  .demo-note{
    margin-top:22px; padding:12px 14px; background:var(--paper-soft); border:1px dashed var(--line);
    border-radius:2px; font-size:11px; color:var(--slate); line-height:1.5;
  }
  .demo-note strong{color:var(--ink);}

  /* ---------- DASHBOARD ---------- */
  #dashboard{display:none;}
  .admin-header{
    display:flex; align-items:center; justify-content:space-between; padding:16px 32px;
    border-bottom:1px solid var(--line); background:rgba(237,235,227,0.94); position:sticky; top:0; z-index:10;
  }
  .admin-logo{display:flex; align-items:center; gap:10px;}
  .admin-logo-text{font-family:'Big Shoulders Display',sans-serif; font-weight:800; font-size:20px;}
  .admin-badge{font-size:10px; letter-spacing:1px; text-transform:uppercase; color:var(--slate); background:var(--paper-soft); border:1px solid var(--line); padding:3px 9px; border-radius:12px;}
  .admin-user{display:flex; align-items:center; gap:12px;}
  .admin-avatar{width:32px; height:32px; border-radius:50%; background:var(--ink); color:var(--paper); display:flex; align-items:center; justify-content:center; font-size:12px; font-weight:700;}
  .logout-btn{font-size:12px; color:var(--slate); background:none; border:none; cursor:pointer;}
  .logout-btn:hover{color:var(--ink);}

  .admin-body{padding:36px 32px; max-width:1200px; margin:0 auto;}
  .admin-title{font-family:'Big Shoulders Display',sans-serif; font-size:30px; text-transform:uppercase; margin-bottom:4px;}
  .admin-subtitle{color:var(--slate); font-size:13px; margin-bottom:30px;}

  .kpi-grid{display:grid; grid-template-columns:repeat(4,1fr); gap:16px; margin-bottom:32px;}
  @media (max-width:900px){ .kpi-grid{grid-template-columns:repeat(2,1fr);} }
  .kpi-card{background:var(--paper-soft); border:1px solid var(--line); border-radius:2px; padding:20px;}
  .kpi-label{font-size:11px; letter-spacing:1px; text-transform:uppercase; color:var(--slate); margin-bottom:10px;}
  .kpi-value{font-family:'Space Mono',monospace; font-size:26px; font-weight:700;}
  .kpi-delta{font-size:11px; margin-top:8px; display:flex; align-items:center; gap:5px;}
  .kpi-delta.up{color:var(--green);}
  .kpi-delta.down{color:var(--signal);}

  .panel-row{display:grid; grid-template-columns:1.4fr 1fr; gap:20px; margin-bottom:20px;}
  @media (max-width:900px){ .panel-row{grid-template-columns:1fr;} }
  .panel{background:var(--paper-soft); border:1px solid var(--line); border-radius:2px; padding:24px;}
  .panel-head{display:flex; justify-content:space-between; align-items:center; margin-bottom:18px;}
  .panel-title{font-weight:600; font-size:15px;}
  .panel-note{font-size:11px; color:var(--slate);}

  .curve-svg{width:100%; height:180px;}
  .curve-svg path.line{fill:none; stroke:var(--gold); stroke-width:2;}
  .curve-svg path.fill{stroke:none; fill:url(#curveGrad);}
  .curve-svg .dot{fill:var(--signal);}

  .cat-bar-row{display:flex; align-items:center; gap:12px; margin-bottom:14px;}
  .cat-bar-label{width:90px; font-size:12px; color:var(--slate);}
  .cat-bar-track{flex:1; height:8px; background:var(--paper-deep); border-radius:4px; overflow:hidden;}
  .cat-bar-fill{height:100%; background:var(--ink); border-radius:4px;}
  .cat-bar-value{width:36px; text-align:right; font-family:'Space Mono',monospace; font-size:12px;}

  table{width:100%; border-collapse:collapse; font-size:13px;}
  th{text-align:left; font-size:10px; letter-spacing:1px; text-transform:uppercase; color:var(--slate); padding:10px 12px; border-bottom:1px solid var(--line);}
  td{padding:12px; border-bottom:1px solid var(--line);}
  tr:last-child td{border-bottom:none;}
  .status-pill{font-size:10px; padding:3px 9px; border-radius:10px; background:#e5f0e9; color:var(--green); letter-spacing:0.3px;}
</style>
</head>
<body>

<!-- ================= LOGIN ================= -->
<div id="loginScreen">
  <div class="login-card">
    <div class="login-logo">
      <div class="logo-mark">$</div>
      <div class="login-logo-text">ODP Admin</div>
    </div>
    <div class="login-sub">Owner access only</div>

    <button class="oauth-btn" onclick="fakeGoogleLogin()">
      <svg viewBox="0 0 48 48"><path fill="#FFC107" d="M43.6 20.5H42V20H24v8h11.3C33.9 32.6 29.4 36 24 36c-6.6 0-12-5.4-12-12s5.4-12 12-12c3.1 0 5.9 1.2 8 3.1l5.7-5.7C34.5 6.1 29.5 4 24 4 12.9 4 4 12.9 4 24s8.9 20 20 20 20-8.9 20-20c0-1.3-.1-2.7-.4-4z"/><path fill="#FF3D00" d="M6.3 14.7l6.6 4.8C14.6 15.1 18.9 12 24 12c3.1 0 5.9 1.2 8 3.1l5.7-5.7C34.5 6.1 29.5 4 24 4 16.3 4 9.7 8.3 6.3 14.7z"/><path fill="#4CAF50" d="M24 44c5.3 0 10.1-2 13.7-5.4l-6.3-5.3C29.4 35 26.8 36 24 36c-5.3 0-9.8-3.4-11.4-8.1l-6.5 5C9.6 39.6 16.3 44 24 44z"/><path fill="#1976D2" d="M43.6 20.5H42V20H24v8h11.3c-1.1 3-3.1 5.5-5.9 7.3l6.3 5.3C39.4 37.4 44 31.4 44 24c0-1.3-.1-2.7-.4-3.5z"/></svg>
      Continue with Google
    </button>

    <div class="divider">or</div>

    <div class="field"><label>Email</label><input type="email" id="loginEmail" placeholder="you@odp.com"></div>
    <div class="field"><label>Password</label><input type="password" id="loginPass" placeholder="••••••••"></div>
    <button class="login-btn" onclick="fakeEmailLogin()">Sign in</button>
    <div class="login-error" id="loginError">That email isn't authorized for admin access.</div>

    <div class="demo-note">
      <strong>This is a visual demo, not real auth.</strong> No password is checked against a database — anyone with this file can view its source. To make this a real owner-only login, connect it to Supabase Auth or Firebase Auth (Google sign-in + an allow-list of one email), or skip building a login entirely and put the page behind Cloudflare Access / Netlify password protection.
      <br><br>Demo: click "Continue with Google," or type any email + password to enter.
    </div>
  </div>
</div>

<!-- ================= DASHBOARD ================= -->
<div id="dashboard">
  <div class="admin-header">
    <div class="admin-logo">
      <div class="logo-mark" style="width:26px;height:26px;font-size:10px;">$</div>
      <div class="admin-logo-text">ODP Admin</div>
      <span class="admin-badge">Owner</span>
    </div>
    <div class="admin-user">
      <div class="admin-avatar" id="userInitial">Y</div>
      <button class="logout-btn" onclick="logout()">Sign out</button>
    </div>
  </div>

  <div class="admin-body">
    <div class="admin-title">Today's Drop</div>
    <div class="admin-subtitle" id="adminSubtitle">Meridian Reading Lamp · live since midnight</div>

    <div class="kpi-grid">
      <div class="kpi-card">
        <div class="kpi-label">Current live price</div>
        <div class="kpi-value mono" id="kpiPrice">$0.00</div>
        <div class="kpi-delta up">↑ climbing $0.35 / tick</div>
      </div>
      <div class="kpi-card">
        <div class="kpi-label">Units sold today</div>
        <div class="kpi-value mono">23</div>
        <div class="kpi-delta up">↑ 4 vs. same hour yesterday</div>
      </div>
      <div class="kpi-card">
        <div class="kpi-label">Revenue today</div>
        <div class="kpi-value mono">$1,042</div>
        <div class="kpi-delta up">↑ 12% vs. yesterday's drop</div>
      </div>
      <div class="kpi-card">
        <div class="kpi-label">Avg. lock-in price</div>
        <div class="kpi-value mono">$45.30</div>
        <div class="kpi-delta down">↓ buyers arriving earlier</div>
      </div>
    </div>

    <div class="panel-row">
      <div class="panel">
        <div class="panel-head">
          <div class="panel-title">Price curve — today</div>
          <div class="panel-note">Dots = purchases</div>
        </div>
        <svg class="curve-svg" id="curveSvg" viewBox="0 0 600 180" preserveAspectRatio="none">
          <defs>
            <linearGradient id="curveGrad" x1="0" y1="0" x2="0" y2="1">
              <stop offset="0%" stop-color="#C9A227" stop-opacity="0.3"/>
              <stop offset="100%" stop-color="#C9A227" stop-opacity="0"/>
            </linearGradient>
          </defs>
          <path class="fill" id="curveFill" d=""></path>
          <path class="line" id="curveLine" d=""></path>
          <g id="curveDots"></g>
        </svg>
      </div>
      <div class="panel">
        <div class="panel-head"><div class="panel-title">Sales by category</div></div>
        <div id="catBars"></div>
      </div>
    </div>

    <div class="panel">
      <div class="panel-head">
        <div class="panel-title">Recent purchases</div>
        <div class="panel-note">Last 6 lock-ins</div>
      </div>
      <table>
        <thead><tr><th>Buyer</th><th>Item</th><th>Locked price</th><th>Time</th><th>Status</th></tr></thead>
        <tbody id="ordersBody"></tbody>
      </table>
    </div>
  </div>
</div>

<script>
  // ---------- Demo auth (visual only — see note in login card) ----------
  function enterDashboard(email){
    document.getElementById('loginScreen').style.display = 'none';
    document.getElementById('dashboard').style.display = 'block';
    document.getElementById('userInitial').textContent = (email||'Y').charAt(0).toUpperCase();
    document.getElementById('adminSubtitle').textContent = `Meridian Reading Lamp · live since midnight · signed in as ${email}`;
    startLiveKpi();
  }
  function fakeGoogleLogin(){ enterDashboard('you@gmail.com'); }
  function fakeEmailLogin(){
    const email = document.getElementById('loginEmail').value || 'you@odp.com';
    enterDashboard(email);
  }
  function logout(){
    document.getElementById('dashboard').style.display = 'none';
    document.getElementById('loginScreen').style.display = 'flex';
  }

  // ---------- Live KPI price ----------
  let price = 0;
  function startLiveKpi(){
    setInterval(()=>{
      price = Math.min(180, +(price+0.35).toFixed(2));
      document.getElementById('kpiPrice').textContent = '$' + price.toFixed(2);
    }, 300);
  }

  // ---------- Price curve with purchase dots ----------
  const curvePoints = [0,4,9,15,18,24,29,33,40,44,49,55,58,63,70,75,80,86,90,95];
  const purchaseIdx = [2,5,9,13,17];
  function drawCurve(){
    const w=600,h=180, max=Math.max(...curvePoints);
    const step = w/(curvePoints.length-1);
    let d='';
    curvePoints.forEach((p,i)=>{
      const x=i*step, y = h - (p/max)*h*0.85 - 8;
      d += (i===0?'M':'L') + x.toFixed(1)+','+y.toFixed(1)+' ';
    });
    document.getElementById('curveLine').setAttribute('d', d);
    document.getElementById('curveFill').setAttribute('d', d + `L${w},${h} L0,${h} Z`);
    const dotsG = document.getElementById('curveDots');
    purchaseIdx.forEach(i=>{
      const x=i*step, y = h - (curvePoints[i]/max)*h*0.85 - 8;
      const c = document.createElementNS('http://www.w3.org/2000/svg','circle');
      c.setAttribute('cx',x); c.setAttribute('cy',y); c.setAttribute('r',4);
      c.setAttribute('class','dot');
      dotsG.appendChild(c);
    });
  }
  drawCurve();

  // ---------- Category bars ----------
  const cats = [
    {name:'Lighting', pct:82}, {name:'Objects', pct:64}, {name:'Furniture', pct:55},
    {name:'Tools', pct:38}, {name:'Accessories', pct:29}
  ];
  document.getElementById('catBars').innerHTML = cats.map(c=>`
    <div class="cat-bar-row">
      <div class="cat-bar-label">${c.name}</div>
      <div class="cat-bar-track"><div class="cat-bar-fill" style="width:${c.pct}%;"></div></div>
      <div class="cat-bar-value mono">${c.pct}%</div>
    </div>`).join('');

  // ---------- Recent orders ----------
  const orders = [
    {buyer:'J. Ellis', item:'Meridian Reading Lamp', price:'$38.15', time:'2 min ago'},
    {buyer:'R. Ncube', item:'Meridian Reading Lamp', price:'$36.40', time:'9 min ago'},
    {buyer:'A. Voss', item:'Meridian Reading Lamp', price:'$33.85', time:'14 min ago'},
    {buyer:'M. Ito', item:'Meridian Reading Lamp', price:'$29.60', time:'27 min ago'},
    {buyer:'S. Cole', item:'Meridian Reading Lamp', price:'$24.05', time:'41 min ago'},
    {buyer:'D. Park', item:'Meridian Reading Lamp', price:'$18.90', time:'58 min ago'},
  ];
  document.getElementById('ordersBody').innerHTML = orders.map(o=>`
    <tr>
      <td>${o.buyer}</td><td>${o.item}</td><td class="mono">${o.price}</td><td>${o.time}</td>
      <td><span class="status-pill">Confirmed</span></td>
    </tr>`).join('');
</script>
</body>
</html>

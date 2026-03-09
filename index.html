<!DOCTYPE html>
<html lang="it">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>ArchivioFascicoli</title>
<script src="https://cdnjs.cloudflare.com/ajax/libs/qrcodejs/1.0.0/qrcode.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/xlsx/0.18.5/xlsx.full.min.js"></script>
<link href="https://fonts.googleapis.com/css2?family=DM+Serif+Display:ital@0;1&family=DM+Sans:opsz,wght@9..40,300;9..40,400;9..40,500;9..40,600&display=swap" rel="stylesheet">
<style>
:root {
  --bg:#0f0f0f; --surface:#1a1a1a; --surface2:#242424; --surface3:#2e2e2e;
  --border:#2e2e2e; --border2:#3a3a3a;
  --accent:#e8c97a; --accent2:#c4a35a; --accent-dim:rgba(232,201,122,0.12);
  --text:#f0ece0; --text2:#a09880; --text3:#6a6258;
  --danger:#e05555; --success:#5aad7a; --info:#5a8fad; --warning:#e0975a;
  --radius:8px; --radius-lg:12px; --shadow:0 8px 32px rgba(0,0,0,0.5);
}
*,*::before,*::after{box-sizing:border-box;margin:0;padding:0;}
html{scroll-behavior:smooth;}
body{font-family:'DM Sans',sans-serif;background:var(--bg);color:var(--text);min-height:100vh;font-size:14px;line-height:1.5;}

/* ── LAYOUT ── */
.shell{display:flex;min-height:100vh;}
.sidebar{width:250px;flex-shrink:0;background:var(--surface);border-right:1px solid var(--border);display:flex;flex-direction:column;position:sticky;top:0;height:100vh;overflow-y:auto;}
.logo{padding:28px 22px 18px;border-bottom:1px solid var(--border);}
.logo-mark{display:flex;align-items:center;gap:10px;margin-bottom:4px;}
.logo-icon{width:34px;height:34px;background:var(--accent-dim);border:1px solid rgba(232,201,122,0.3);border-radius:8px;display:flex;align-items:center;justify-content:center;}
.logo-icon svg{width:18px;height:18px;color:var(--accent);}
.logo h1{font-family:'DM Serif Display',serif;font-size:17px;color:var(--accent);line-height:1.2;}
.logo span{font-size:10.5px;color:var(--text3);letter-spacing:0.1em;text-transform:uppercase;}
.nav{padding:14px 10px;flex:1;}
.nav-sect{font-size:9.5px;letter-spacing:0.12em;text-transform:uppercase;color:var(--text3);padding:14px 12px 5px;margin-top:4px;}
.nav-item{display:flex;align-items:center;gap:9px;padding:9px 12px;border-radius:var(--radius);cursor:pointer;transition:all 0.15s;color:var(--text2);font-weight:500;font-size:13px;margin-bottom:1px;user-select:none;}
.nav-item:hover{background:var(--surface2);color:var(--text);}
.nav-item.active{background:var(--accent-dim);color:var(--accent);}
.nav-item svg{width:15px;height:15px;flex-shrink:0;}
.nav-badge{margin-left:auto;background:var(--danger);color:#fff;font-size:10px;font-weight:700;padding:1px 6px;border-radius:10px;}
.sidebar-footer{padding:14px 16px;border-top:1px solid var(--border);font-size:11px;color:var(--text3);}

.main{flex:1;overflow-x:hidden;display:flex;flex-direction:column;}
.topbar{background:var(--surface);border-bottom:1px solid var(--border);padding:0 28px;height:58px;display:flex;align-items:center;justify-content:space-between;position:sticky;top:0;z-index:50;flex-shrink:0;}
.topbar-left{display:flex;align-items:center;gap:14px;}
.topbar-title{font-family:'DM Serif Display',serif;font-size:20px;color:var(--text);}
.topbar-sub{font-size:12px;color:var(--text3);}
.topbar-right{display:flex;gap:8px;align-items:center;}
.content{padding:26px 28px;flex:1;}

/* ── BUTTONS ── */
.btn{display:inline-flex;align-items:center;gap:6px;padding:8px 15px;border-radius:var(--radius);font-family:'DM Sans',sans-serif;font-size:13px;font-weight:500;cursor:pointer;border:none;transition:all 0.15s;white-space:nowrap;}
.btn-primary{background:var(--accent);color:#15110a;}
.btn-primary:hover{background:var(--accent2);}
.btn-ghost{background:transparent;color:var(--text2);border:1px solid var(--border2);}
.btn-ghost:hover{background:var(--surface2);color:var(--text);}
.btn-danger{background:rgba(224,85,85,0.12);color:var(--danger);border:1px solid rgba(224,85,85,0.25);}
.btn-danger:hover{background:rgba(224,85,85,0.22);}
.btn-success{background:rgba(90,173,122,0.12);color:var(--success);border:1px solid rgba(90,173,122,0.25);}
.btn-success:hover{background:rgba(90,173,122,0.22);}
.btn-sm{padding:5px 10px;font-size:12px;}
.btn-xs{padding:3px 8px;font-size:11px;}
.btn svg{width:13px;height:13px;}
.btn-sm svg{width:12px;height:12px;}

/* ── CARDS ── */
.card{background:var(--surface);border:1px solid var(--border);border-radius:var(--radius-lg);padding:20px;}
.card-hd{display:flex;align-items:center;justify-content:space-between;margin-bottom:16px;}
.card-title{font-size:11px;font-weight:700;color:var(--text3);text-transform:uppercase;letter-spacing:0.1em;}

/* ── STATS ── */
.stats-row{display:grid;grid-template-columns:repeat(4,1fr);gap:12px;margin-bottom:22px;}
.stat{background:var(--surface);border:1px solid var(--border);border-radius:var(--radius-lg);padding:18px 20px;position:relative;overflow:hidden;}
.stat::after{content:'';position:absolute;bottom:0;left:0;right:0;height:2px;background:var(--accent-color,var(--accent));opacity:0.5;}
.stat-val{font-family:'DM Serif Display',serif;font-size:34px;line-height:1;margin-bottom:4px;}
.stat-lbl{font-size:11px;color:var(--text3);}
.stat-icon{position:absolute;top:16px;right:16px;opacity:0.1;}
.stat-icon svg{width:32px;height:32px;}

/* ── TABLE ── */
.tbl-wrap{overflow-x:auto;}
table{width:100%;border-collapse:collapse;}
thead th{padding:9px 13px;text-align:left;font-size:10.5px;font-weight:700;letter-spacing:0.08em;text-transform:uppercase;color:var(--text3);border-bottom:1px solid var(--border);white-space:nowrap;}
tbody tr{transition:background 0.1s;cursor:default;}
tbody tr:hover{background:var(--surface2);}
tbody td{padding:9px 13px;border-bottom:1px solid rgba(46,46,46,0.8);font-size:13px;vertical-align:middle;}
.td-primary{color:var(--accent);font-weight:600;font-size:14px;cursor:pointer;}
.td-primary:hover{text-decoration:underline;}
.td-muted{color:var(--text3);}

/* ── BADGE ── */
.badge{display:inline-flex;align-items:center;gap:4px;padding:2px 8px;border-radius:20px;font-size:11px;font-weight:600;white-space:nowrap;}
.badge::before{content:'';width:5px;height:5px;border-radius:50%;background:currentColor;opacity:0.7;}
.badge-in{background:rgba(90,173,122,0.12);color:var(--success);}
.badge-out{background:rgba(224,85,85,0.12);color:var(--danger);}
.badge-info{background:rgba(90,143,173,0.12);color:var(--info);}

/* ── FORM ── */
.fg{margin-bottom:14px;}
.fl{display:block;font-size:11px;font-weight:600;color:var(--text2);margin-bottom:5px;text-transform:uppercase;letter-spacing:0.06em;}
.fi,.fs,.ft{width:100%;padding:9px 12px;background:var(--surface2);border:1px solid var(--border2);border-radius:var(--radius);color:var(--text);font-family:'DM Sans',sans-serif;font-size:13.5px;outline:none;transition:border 0.15s;}
.fi:focus,.fs:focus,.ft:focus{border-color:var(--accent);background:var(--surface3);}
.fi::placeholder,.ft::placeholder{color:var(--text3);}
.fs option{background:var(--surface2);}
.ft{resize:vertical;min-height:76px;}
.frow{display:grid;grid-template-columns:1fr 1fr;gap:12px;}

/* ── SEARCH ── */
.srch{position:relative;}
.srch svg{position:absolute;left:11px;top:50%;transform:translateY(-50%);width:14px;height:14px;color:var(--text3);pointer-events:none;}
.srch input{padding-left:34px;}

/* ── MODAL ── */
.overlay{position:fixed;inset:0;z-index:200;background:rgba(0,0,0,0.75);backdrop-filter:blur(6px);display:flex;align-items:center;justify-content:center;opacity:0;pointer-events:none;transition:opacity 0.2s;padding:16px;}
.overlay.open{opacity:1;pointer-events:all;}
.modal{background:var(--surface);border:1px solid var(--border2);border-radius:16px;padding:28px;width:100%;max-width:500px;box-shadow:var(--shadow);transform:translateY(20px) scale(0.98);transition:transform 0.22s;max-height:92vh;overflow-y:auto;}
.overlay.open .modal{transform:none;}
.modal-lg{max-width:680px;}
.modal-xl{max-width:820px;}
.modal-title{font-family:'DM Serif Display',serif;font-size:21px;margin-bottom:20px;color:var(--text);}
.modal-foot{display:flex;gap:8px;justify-content:flex-end;margin-top:22px;padding-top:18px;border-top:1px solid var(--border);}

/* ── LUOGHI ── */
.luoghi-grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(250px,1fr));gap:12px;}
.lcard{background:var(--surface);border:1px solid var(--border);border-radius:var(--radius-lg);padding:18px;transition:all 0.15s;position:relative;}
.lcard::before{content:'';position:absolute;top:0;left:0;bottom:0;width:3px;background:var(--accent);border-radius:var(--radius-lg) 0 0 var(--radius-lg);opacity:0;transition:opacity 0.15s;}
.lcard:hover{border-color:var(--border2);transform:translateY(-1px);box-shadow:0 4px 20px rgba(0,0,0,0.3);}
.lcard:hover::before{opacity:1;}
.lcard-name{font-family:'DM Serif Display',serif;font-size:16px;margin-bottom:3px;}
.lcard-desc{font-size:12px;color:var(--text3);margin-bottom:12px;line-height:1.55;}
.lcard-meta{font-size:12px;color:var(--text2);margin-bottom:12px;}
.lcard-actions{display:flex;gap:6px;flex-wrap:wrap;}

/* ── QR ── */
#qr-box{display:inline-block;background:#fff;padding:14px;border-radius:10px;}
.qr-list{max-height:180px;overflow-y:auto;margin-top:12px;}
.qr-list-item{padding:5px 0;border-bottom:1px solid var(--border);font-size:12px;color:var(--text2);display:flex;justify-content:space-between;align-items:center;}
.qr-url-box{background:var(--surface2);border:1px solid var(--border);border-radius:6px;padding:8px 10px;font-size:11px;color:var(--text3);word-break:break-all;margin-top:10px;font-family:monospace;}

/* ── PRELIEVO ── */
.pinfo{background:var(--surface2);border-radius:var(--radius);padding:14px;margin-bottom:16px;}
.pinfo-row{display:flex;justify-content:space-between;align-items:center;padding:3px 0;font-size:13px;}
.pinfo-row span:first-child{color:var(--text3);}

/* ── DETAIL ── */
.drow{display:flex;padding:9px 0;border-bottom:1px solid var(--border);font-size:13px;}
.dlabel{width:150px;flex-shrink:0;color:var(--text3);}
.dval{color:var(--text);}

/* ── TABS ── */
.tabs{display:flex;border-bottom:1px solid var(--border);margin-bottom:18px;gap:0;}
.tab{padding:9px 16px;cursor:pointer;font-size:13px;font-weight:500;color:var(--text3);border-bottom:2px solid transparent;margin-bottom:-1px;transition:all 0.15s;}
.tab:hover{color:var(--text);}
.tab.active{color:var(--accent);border-bottom-color:var(--accent);}

/* ── IMPORT ── */
.dropzone{border:2px dashed var(--border2);border-radius:var(--radius-lg);padding:38px;text-align:center;cursor:pointer;transition:all 0.15s;color:var(--text3);}
.dropzone:hover,.dropzone.over{border-color:var(--accent);color:var(--text);background:var(--accent-dim);}
.dropzone svg{width:40px;height:40px;margin:0 auto 10px;display:block;opacity:0.5;}
.colmap{display:grid;grid-template-columns:1fr 1fr;gap:6px;margin-top:12px;}
.colmap-item{background:var(--surface2);border-radius:5px;padding:7px 10px;font-size:12px;display:flex;justify-content:space-between;align-items:center;gap:8px;}
.colmap-item span:first-child{color:var(--text3);white-space:nowrap;}

/* ── DEPLOY PAGE ── */
.deploy-wrap{max-width:740px;}
.step-card{background:var(--surface);border:1px solid var(--border);border-radius:var(--radius-lg);padding:22px;margin-bottom:14px;position:relative;padding-left:66px;}
.step-num{position:absolute;left:20px;top:22px;width:32px;height:32px;border-radius:50%;background:var(--accent-dim);border:1px solid rgba(232,201,122,0.3);display:flex;align-items:center;justify-content:center;font-family:'DM Serif Display',serif;font-size:16px;color:var(--accent);}
.step-title{font-size:15px;font-weight:600;margin-bottom:6px;}
.step-desc{font-size:13px;color:var(--text2);line-height:1.7;margin-bottom:12px;}
.step-desc code{background:var(--surface2);padding:1px 5px;border-radius:3px;font-family:monospace;font-size:12px;color:var(--accent);}
.code-block{background:#0a0a0a;border:1px solid var(--border);border-radius:var(--radius);padding:14px 16px;font-family:'Courier New',monospace;font-size:12px;color:#c8e6a0;overflow-x:auto;position:relative;margin-top:10px;line-height:1.7;}
.code-block .comment{color:var(--text3);}
.copy-btn{position:absolute;top:8px;right:8px;background:var(--surface2);border:1px solid var(--border);color:var(--text2);padding:3px 10px;border-radius:4px;font-size:11px;cursor:pointer;font-family:'DM Sans',sans-serif;}
.copy-btn:hover{color:var(--text);border-color:var(--accent);}
.deploy-note{background:rgba(232,201,122,0.07);border:1px solid rgba(232,201,122,0.2);border-radius:var(--radius);padding:12px 14px;font-size:12.5px;color:var(--text2);line-height:1.7;margin-top:10px;}
.deploy-note strong{color:var(--accent);}
.deploy-note code{background:rgba(232,201,122,0.1);padding:1px 5px;border-radius:3px;font-family:monospace;font-size:11.5px;}

/* ── EMPTY ── */
.empty{text-align:center;padding:60px 20px;color:var(--text3);}
.empty svg{width:44px;height:44px;margin:0 auto 12px;display:block;opacity:0.2;}
.empty p{font-size:13.5px;}

/* ── CONFIRM ── */
.confirm-modal{max-width:380px;text-align:center;padding:32px 28px;}
.confirm-icon{width:54px;height:54px;border-radius:50%;background:rgba(224,85,85,0.12);display:flex;align-items:center;justify-content:center;margin:0 auto 14px;}
.confirm-icon svg{width:26px;height:26px;color:var(--danger);}
.confirm-text{color:var(--text2);font-size:13.5px;margin-bottom:22px;line-height:1.65;}
.confirm-btns{display:flex;gap:8px;justify-content:center;}

/* ── TOAST ── */
#toasts{position:fixed;bottom:22px;right:22px;z-index:999;display:flex;flex-direction:column;gap:7px;pointer-events:none;}
.toast{background:var(--surface2);border:1px solid var(--border2);border-radius:var(--radius);padding:11px 16px;font-size:13px;min-width:210px;animation:tsin 0.2s ease;box-shadow:var(--shadow);pointer-events:all;}
.toast.ok{border-left:3px solid var(--success);}
.toast.err{border-left:3px solid var(--danger);}
.toast.info{border-left:3px solid var(--info);}
@keyframes tsin{from{opacity:0;transform:translateX(16px);}to{opacity:1;transform:none;}}

/* ── PAGE ── */
.page{display:none;animation:fadein 0.18s ease;}
.page.active{display:block;}
@keyframes fadein{from{opacity:0;transform:translateY(6px);}to{opacity:1;transform:none;}}

/* ── SCROLLBAR ── */
::-webkit-scrollbar{width:5px;height:5px;}
::-webkit-scrollbar-track{background:transparent;}
::-webkit-scrollbar-thumb{background:var(--surface3);border-radius:4px;}

/* ── LOADING ── */
.lrow{text-align:center;padding:38px;color:var(--text3);font-size:13px;}
.spinner{display:inline-block;width:16px;height:16px;border:2px solid var(--border2);border-top-color:var(--accent);border-radius:50%;animation:spin 0.7s linear infinite;vertical-align:middle;margin-right:8px;}
@keyframes spin{to{transform:rotate(360deg);}}

@media(max-width:700px){
  .sidebar{display:none;}
  .content{padding:14px;}
  .stats-row{grid-template-columns:1fr 1fr;}
  .frow{grid-template-columns:1fr;}
}
</style>
</head>
<body>
<div class="shell">

<!-- ══ SIDEBAR ══ -->
<nav class="sidebar">
  <div class="logo">
    <div class="logo-mark">
      <div class="logo-icon"><svg fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 8h14M5 8a2 2 0 110-4h14a2 2 0 110 4M5 8v10a2 2 0 002 2h10a2 2 0 002-2V8m-9 4h4"/></svg></div>
      <h1>Archivio<br>Fascicoli</h1>
    </div>
    <span>Gestione documentale</span>
  </div>
  <div class="nav">
    <div class="nav-sect">Principale</div>
    <div class="nav-item active" onclick="go('dashboard')">
      <svg fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 5a1 1 0 011-1h4a1 1 0 011 1v4a1 1 0 01-1 1H5a1 1 0 01-1-1V5zm10 0a1 1 0 011-1h4a1 1 0 011 1v4a1 1 0 01-1 1h-4a1 1 0 01-1-1V5zM4 15a1 1 0 011-1h4a1 1 0 011 1v4a1 1 0 01-1 1H5a1 1 0 01-1-1v-4zm10 0a1 1 0 011-1h4a1 1 0 011 1v4a1 1 0 01-1 1h-4a1 1 0 01-1-1v-4z"/></svg>
      Dashboard
    </div>
    <div class="nav-item" onclick="go('fascicoli')">
      <svg fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12h6m-6 4h6m2 5H7a2 2 0 01-2-2V5a2 2 0 012-2h5.586a1 1 0 01.707.293l5.414 5.414a1 1 0 01.293.707V19a2 2 0 01-2 2z"/></svg>
      Fascicoli
    </div>
    <div class="nav-item" onclick="go('luoghi')">
      <svg fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 8h14M5 8a2 2 0 110-4h14a2 2 0 110 4M5 8v10a2 2 0 002 2h10a2 2 0 002-2V8"/></svg>
      Luoghi
    </div>
    <div class="nav-item" onclick="go('prelievi')">
      <svg fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 8v4l3 3m6-3a9 9 0 11-18 0 9 9 0 0118 0z"/></svg>
      Prelievi
    </div>
    <div class="nav-sect">Strumenti</div>
    <div class="nav-item" onclick="go('import')">
      <svg fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 16v1a3 3 0 003 3h10a3 3 0 003-3v-1m-4-8l-4-4m0 0L8 8m4-4v12"/></svg>
      Import Excel
    </div>
    <div class="nav-item" onclick="go('deploy')">
      <svg fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 15a4 4 0 004 4h9a5 5 0 10-.1-9.999 5.002 5.002 0 10-9.78 2.096A4.001 4.001 0 003 15z"/></svg>
      Deploy Cloudflare
      <span class="nav-badge">!</span>
    </div>
  </div>
  <div class="sidebar-footer">v1.0 · localStorage mode</div>
</nav>

<!-- ══ MAIN ══ -->
<main class="main">
  <div class="topbar">
    <div class="topbar-left">
      <div class="topbar-title" id="pg-title">Dashboard</div>
      <div class="topbar-sub" id="pg-sub"></div>
    </div>
    <div class="topbar-right" id="pg-actions"></div>
  </div>

  <div class="content">

    <!-- ── DASHBOARD ── -->
    <div class="page active" id="page-dashboard">
      <div class="stats-row" id="stats"></div>
      <div style="display:grid;grid-template-columns:1fr 1fr;gap:14px">
        <div class="card">
          <div class="card-hd"><span class="card-title">Ultimi fascicoli aggiunti</span><a style="font-size:12px;color:var(--accent);cursor:pointer" onclick="go('fascicoli')">Tutti →</a></div>
          <div id="dash-fasc"></div>
        </div>
        <div class="card">
          <div class="card-hd"><span class="card-title">Ultimi prelievi</span><a style="font-size:12px;color:var(--accent);cursor:pointer" onclick="go('prelievi')">Tutti →</a></div>
          <div id="dash-prel"></div>
        </div>
      </div>
    </div>

    <!-- ── FASCICOLI ── -->
    <div class="page" id="page-fascicoli">
      <div style="display:flex;gap:10px;margin-bottom:18px;align-items:center;flex-wrap:wrap">
        <div class="srch" style="flex:1;min-width:200px">
          <svg fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z"/></svg>
          <input class="fi" id="q-fasc" placeholder="Cerca numero, anno, oggetto, parti..." oninput="renderFasc()">
        </div>
        <select class="fs" style="width:150px" id="filt-stato" onchange="renderFasc()">
          <option value="">Tutti gli stati</option>
          <option value="in">In sede</option>
          <option value="out">Prelevato</option>
        </select>
        <select class="fs" style="width:170px" id="filt-luogo" onchange="renderFasc()">
          <option value="">Tutti i luoghi</option>
        </select>
      </div>
      <div class="card">
        <div class="tbl-wrap">
          <table>
            <thead><tr><th>N° / Anno</th><th>Oggetto</th><th>Parte 1</th><th>Parte 2</th><th>Giudice</th><th>Luogo</th><th>Stato</th><th></th></tr></thead>
            <tbody id="tb-fasc"></tbody>
          </table>
        </div>
        <div id="empty-fasc" class="empty" style="display:none"><svg fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12h6m-6 4h6m2 5H7a2 2 0 01-2-2V5a2 2 0 012-2h5.586a1 1 0 01.707.293l5.414 5.414a1 1 0 01.293.707V19a2 2 0 01-2 2z"/></svg><p>Nessun fascicolo trovato</p></div>
      </div>
    </div>

    <!-- ── LUOGHI ── -->
    <div class="page" id="page-luoghi">
      <div class="luoghi-grid" id="grid-luoghi"></div>
      <div id="empty-luoghi" class="empty" style="display:none"><svg fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 8h14M5 8a2 2 0 110-4h14a2 2 0 110 4M5 8v10a2 2 0 002 2h10a2 2 0 002-2V8"/></svg><p>Nessun luogo creato. Aggiungi il primo!</p></div>
    </div>

    <!-- ── PRELIEVI ── -->
    <div class="page" id="page-prelievi">
      <div style="display:flex;gap:10px;margin-bottom:18px">
        <div class="srch" style="flex:1">
          <svg fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z"/></svg>
          <input class="fi" id="q-prel" placeholder="Cerca operatore, fascicolo..." oninput="renderPrel()">
        </div>
        <button class="btn btn-ghost" onclick="exportPrel()"><svg fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 16v1a3 3 0 003 3h10a3 3 0 003-3v-1m-4-4l-4 4m0 0l-4-4m4 4V4"/></svg> Esporta</button>
      </div>
      <div class="card">
        <div class="tbl-wrap">
          <table>
            <thead><tr><th>Data / Ora</th><th>Fascicolo</th><th>Operatore</th><th>Azione</th><th>Note</th></tr></thead>
            <tbody id="tb-prel"></tbody>
          </table>
        </div>
        <div id="empty-prel" class="empty" style="display:none"><svg fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 8v4l3 3m6-3a9 9 0 11-18 0 9 9 0 0118 0z"/></svg><p>Nessun prelievo registrato</p></div>
      </div>
    </div>

    <!-- ── IMPORT ── -->
    <div class="page" id="page-import">
      <div class="card" style="max-width:680px">
        <div class="modal-title" style="font-size:17px;margin-bottom:6px">Import da Excel</div>
        <p style="color:var(--text3);font-size:13px;margin-bottom:18px">Carica un file .xlsx/.xls con 8 colonne. La prima riga è l'intestazione.</p>
        <div class="dropzone" id="dz" onclick="document.getElementById('fi-file').click()">
          <svg fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M7 16a4 4 0 01-.88-7.903A5 5 0 1115.9 6L16 6a5 5 0 011 9.9M15 13l-3-3m0 0l-3 3m3-3v12"/></svg>
          <div style="font-weight:600;margin-bottom:3px">Trascina il file Excel qui</div>
          <div style="font-size:12px">oppure clicca per selezionare (.xlsx, .xls, .csv)</div>
        </div>
        <input type="file" id="fi-file" accept=".xlsx,.xls,.csv" style="display:none" onchange="onFile(event)">
        <div id="imp-preview" style="display:none;margin-top:18px">
          <div class="card-title" style="margin-bottom:8px">Mappa colonne → campi</div>
          <div id="imp-map" class="colmap"></div>
          <p id="imp-count" style="font-size:12px;color:var(--text3);margin-top:8px"></p>
          <div style="display:flex;gap:8px;margin-top:14px">
            <button class="btn btn-primary" onclick="doImport()"><svg fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 16v1a3 3 0 003 3h10a3 3 0 003-3v-1m-4-8l-4-4m0 0L8 8m4-4v12"/></svg> Importa</button>
            <button class="btn btn-ghost" onclick="resetImport()">Annulla</button>
          </div>
        </div>
        <div style="margin-top:22px;padding-top:18px;border-top:1px solid var(--border)">
          <div class="card-title" style="margin-bottom:10px">Struttura attesa (8 colonne)</div>
          <div class="colmap">
            <div class="colmap-item"><span>Colonna 1</span><strong>Numero</strong></div>
            <div class="colmap-item"><span>Colonna 2</span><strong>Anno</strong></div>
            <div class="colmap-item"><span>Colonna 3</span><strong>Oggetto</strong></div>
            <div class="colmap-item"><span>Colonna 4</span><strong>Parte 1</strong></div>
            <div class="colmap-item"><span>Colonna 5</span><strong>Parte 2</strong></div>
            <div class="colmap-item"><span>Colonna 6</span><strong>Giudice</strong></div>
            <div class="colmap-item"><span>Colonna 7</span><strong>Luogo</strong></div>
            <div class="colmap-item"><span>Colonna 8</span><strong>Note</strong></div>
          </div>
          <button class="btn btn-ghost btn-sm" style="margin-top:12px" onclick="dlTemplate()"><svg fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 16v1a3 3 0 003 3h10a3 3 0 003-3v-1m-4-4l-4 4m0 0l-4-4m4 4V4"/></svg> Scarica template</button>
        </div>
      </div>
    </div>

    <!-- ── DEPLOY ── -->
    <div class="page" id="page-deploy">
      <div class="deploy-wrap">
        <div style="margin-bottom:22px">
          <p style="color:var(--text2);font-size:13.5px;line-height:1.7">Questa app ora funziona con <strong style="color:var(--warning)">localStorage</strong> (dati solo sul tuo browser). Per averla su Cloudflare con database reale e QR funzionanti da smartphone, segui questi 4 passi.</p>
        </div>

        <!-- STEP 1 -->
        <div class="step-card">
          <div class="step-num">1</div>
          <div class="step-title">Crea il database D1 su Cloudflare</div>
          <div class="step-desc">
            Vai su <code>dash.cloudflare.com</code> → <strong>Workers & Pages → D1</strong> → <strong>Create database</strong><br>
            Nome: <code>archivio-db</code> · Poi vai su tab <strong>Console</strong> e incolla questo SQL:
          </div>
          <div class="code-block">
            <button class="copy-btn" onclick="copyCode(this)">Copia</button>
<span class="comment">-- Esegui nella console D1 di Cloudflare</span>
CREATE TABLE IF NOT EXISTS luoghi (
  id TEXT PRIMARY KEY,
  nome TEXT NOT NULL,
  descrizione TEXT DEFAULT '',
  creato_il TEXT DEFAULT (datetime('now'))
);
CREATE TABLE IF NOT EXISTS fascicoli (
  id TEXT PRIMARY KEY,
  numero TEXT NOT NULL,
  anno TEXT NOT NULL,
  oggetto TEXT DEFAULT '',
  parte1 TEXT DEFAULT '',
  parte2 TEXT DEFAULT '',
  giudice TEXT DEFAULT '',
  luogo_id TEXT DEFAULT '',
  note TEXT DEFAULT '',
  stato TEXT DEFAULT 'in_sede',
  creato_il TEXT DEFAULT (datetime('now'))
);
CREATE TABLE IF NOT EXISTS prelievi (
  id TEXT PRIMARY KEY,
  fascicolo_id TEXT NOT NULL,
  operatore TEXT NOT NULL,
  azione TEXT NOT NULL,
  note TEXT DEFAULT '',
  data_ora TEXT DEFAULT (datetime('now'))
);
CREATE INDEX IF NOT EXISTS idx_fl ON fascicoli(luogo_id);
CREATE INDEX IF NOT EXISTS idx_pf ON prelievi(fascicolo_id);</div>
        </div>

        <!-- STEP 2 -->
        <div class="step-card">
          <div class="step-num">2</div>
          <div class="step-title">Crea il file Worker (backend API)</div>
          <div class="step-desc">
            Vai su <strong>Workers & Pages → Create → Worker</strong> · Nome: <code>archivio-api</code><br>
            Sostituisci tutto il codice con questo:
          </div>
          <div class="code-block" id="worker-code">
            <button class="copy-btn" onclick="copyCode(this)">Copia</button>
export default {
  async fetch(request, env) {
    const url = new URL(request.url);
    const path = url.pathname.replace(/^\/api\/?/, '').replace(/\/$/, '');
    const method = request.method;
    const cors = {
      'Access-Control-Allow-Origin': '*',
      'Access-Control-Allow-Methods': 'GET,POST,PUT,DELETE,OPTIONS',
      'Access-Control-Allow-Headers': 'Content-Type',
      'Content-Type': 'application/json'
    };
    if (method === 'OPTIONS') return new Response(null, { headers: cors });
    const db = env.DB;
    if (!db) return R({ error: 'DB non configurato' }, 500, cors);
    try {
      <span class="comment">// STATS</span>
      if (path === 'stats') {
        const [t,i,p,l,up,uf] = await Promise.all([
          db.prepare("SELECT COUNT(*) n FROM fascicoli").first(),
          db.prepare("SELECT COUNT(*) n FROM fascicoli WHERE stato='in_sede'").first(),
          db.prepare("SELECT COUNT(*) n FROM fascicoli WHERE stato='prelevato'").first(),
          db.prepare("SELECT COUNT(*) n FROM luoghi").first(),
          db.prepare("SELECT p.*,f.numero,f.anno FROM prelievi p LEFT JOIN fascicoli f ON f.id=p.fascicolo_id ORDER BY p.data_ora DESC LIMIT 5").all(),
          db.prepare("SELECT * FROM fascicoli ORDER BY creato_il DESC LIMIT 5").all()
        ]);
        return R({tot:t.n,inSede:i.n,prelevati:p.n,luoghi:l.n,ultPrel:up.results,ultFasc:uf.results},200,cors);
      }
      <span class="comment">// LUOGHI</span>
      if (path === 'luoghi' && method === 'GET') {
        const {results} = await db.prepare("SELECT l.*,COUNT(f.id) cnt,SUM(CASE WHEN f.stato='prelevato' THEN 1 ELSE 0 END) out FROM luoghi l LEFT JOIN fascicoli f ON f.luogo_id=l.id GROUP BY l.id ORDER BY l.nome").all();
        return R(results,200,cors);
      }
      if (path === 'luoghi' && method === 'POST') {
        const b = await request.json(); const id = uid();
        await db.prepare("INSERT INTO luoghi(id,nome,descrizione) VALUES(?,?,?)").bind(id,b.nome,b.descrizione||'').run();
        return R({id,...b},201,cors);
      }
      const lm = path.match(/^luoghi\/([^/]+)$/);
      if (lm) {
        const id = lm[1];
        if (method==='PUT'){const b=await request.json();await db.prepare("UPDATE luoghi SET nome=?,descrizione=? WHERE id=?").bind(b.nome,b.descrizione||'',id).run();return R({ok:true},200,cors);}
        if (method==='DELETE'){await db.prepare("UPDATE fascicoli SET luogo_id='' WHERE luogo_id=?").bind(id).run();await db.prepare("DELETE FROM luoghi WHERE id=?").bind(id).run();return R({ok:true},200,cors);}
      }
      if (path.match(/^luoghi\/([^/]+)\/qr$/)) {
        const id = path.split('/')[1];
        const luogo = await db.prepare("SELECT * FROM luoghi WHERE id=?").bind(id).first();
        const {results} = await db.prepare("SELECT * FROM fascicoli WHERE luogo_id=? ORDER BY anno DESC,numero").bind(id).all();
        return R({luogo,fascicoli:results},200,cors);
      }
      <span class="comment">// FASCICOLI</span>
      if (path === 'fascicoli') {
        if (method==='GET'){
          const q=url.searchParams.get('q')||'',stato=url.searchParams.get('stato')||'',luogo=url.searchParams.get('luogo')||'';
          let sql="SELECT f.*,l.nome luogo_nome FROM fascicoli f LEFT JOIN luoghi l ON l.id=f.luogo_id WHERE 1=1",params=[];
          if(q){sql+=" AND(f.numero LIKE? OR f.anno LIKE? OR f.oggetto LIKE? OR f.parte1 LIKE? OR f.parte2 LIKE? OR f.giudice LIKE?)";const p='%'+q+'%';params.push(p,p,p,p,p,p);}
          if(stato){sql+=" AND f.stato=?";params.push(stato==='in'?'in_sede':'prelevato');}
          if(luogo){sql+=" AND f.luogo_id=?";params.push(luogo);}
          sql+=" ORDER BY f.anno DESC,CAST(f.numero AS INT)";
          const {results}=await db.prepare(sql).bind(...params).all();
          return R(results,200,cors);
        }
        if (method==='POST'){
          const b=await request.json();
          if(Array.isArray(b)){let n=0;for(const f of b){await db.prepare("INSERT INTO fascicoli(id,numero,anno,oggetto,parte1,parte2,giudice,luogo_id,note)VALUES(?,?,?,?,?,?,?,?,?)").bind(uid(),f.numero||'',f.anno||'',f.oggetto||'',f.parte1||'',f.parte2||'',f.giudice||'',f.luogo_id||'',f.note||'').run();n++;}return R({added:n},201,cors);}
          const id=uid();await db.prepare("INSERT INTO fascicoli(id,numero,anno,oggetto,parte1,parte2,giudice,luogo_id,note)VALUES(?,?,?,?,?,?,?,?,?)").bind(id,b.numero,b.anno,b.oggetto||'',b.parte1||'',b.parte2||'',b.giudice||'',b.luogo_id||'',b.note||'').run();
          return R({id},201,cors);
        }
      }
      const fm=path.match(/^fascicoli\/([^/]+)$/);
      if(fm){
        const id=fm[1];
        if(method==='GET'){const f=await db.prepare("SELECT f.*,l.nome luogo_nome FROM fascicoli f LEFT JOIN luoghi l ON l.id=f.luogo_id WHERE f.id=?").bind(id).first();return R(f,200,cors);}
        if(method==='PUT'){const b=await request.json();await db.prepare("UPDATE fascicoli SET numero=?,anno=?,oggetto=?,parte1=?,parte2=?,giudice=?,luogo_id=?,note=? WHERE id=?").bind(b.numero,b.anno,b.oggetto||'',b.parte1||'',b.parte2||'',b.giudice||'',b.luogo_id||'',b.note||'',id).run();return R({ok:true},200,cors);}
        if(method==='DELETE'){await db.prepare("DELETE FROM prelievi WHERE fascicolo_id=?").bind(id).run();await db.prepare("DELETE FROM fascicoli WHERE id=?").bind(id).run();return R({ok:true},200,cors);}
      }
      if(path.match(/^fascicoli\/([^/]+)\/prelievi$/)){
        const id=path.split('/')[1];
        const {results}=await db.prepare("SELECT * FROM prelievi WHERE fascicolo_id=? ORDER BY data_ora DESC").bind(id).all();
        return R(results,200,cors);
      }
      <span class="comment">// PRELIEVI</span>
      if(path==='prelievi'){
        if(method==='GET'){
          const q=url.searchParams.get('q')||'';
          let sql="SELECT p.*,f.numero,f.anno FROM prelievi p LEFT JOIN fascicoli f ON f.id=p.fascicolo_id WHERE 1=1",params=[];
          if(q){sql+=" AND(f.numero LIKE? OR p.operatore LIKE?)";const p2='%'+q+'%';params.push(p2,p2);}
          sql+=" ORDER BY p.data_ora DESC LIMIT 300";
          const {results}=await db.prepare(sql).bind(...params).all();
          return R(results,200,cors);
        }
        if(method==='POST'){
          const b=await request.json();const id=uid();
          await db.prepare("INSERT INTO prelievi(id,fascicolo_id,operatore,azione,note)VALUES(?,?,?,?,?)").bind(id,b.fascicolo_id,b.operatore,b.azione,b.note||'').run();
          await db.prepare("UPDATE fascicoli SET stato=? WHERE id=?").bind(b.azione==='prelievo'?'prelevato':'in_sede',b.fascicolo_id).run();
          return R({id,stato:b.azione==='prelievo'?'prelevato':'in_sede'},201,cors);
        }
      }
      return R({error:'Not found'},404,cors);
    } catch(e) { return R({error:e.message},500,cors); }
  }
};
function R(d,s,h){return new Response(JSON.stringify(d),{status:s,headers:h});}
function uid(){return Date.now().toString(36)+Math.random().toString(36).slice(2,7);}</div>
          <div class="deploy-note">Dopo aver salvato il Worker, vai su <strong>Settings → Variables → D1 Database Bindings</strong> → aggiungi binding con nome <code>DB</code> → seleziona <code>archivio-db</code></div>
        </div>

        <!-- STEP 3 -->
        <div class="step-card">
          <div class="step-num">3</div>
          <div class="step-title">Crea la pagina mobile per i QR</div>
          <div class="step-desc">
            Crea un file <code>prelievo.html</code> e caricalo su Cloudflare Pages insieme a questo <code>index.html</code>.<br>
            Oppure vai su <strong>Workers & Pages → Pages → Upload assets</strong> e carica entrambi i file.
          </div>
          <div class="code-block">
            <button class="copy-btn" onclick="copyCode(this)">Copia</button>
<span id="prelievo-code">&lt;!DOCTYPE html&gt;
&lt;html lang="it"&gt;
&lt;head&gt;
&lt;meta charset="UTF-8"&gt;
&lt;meta name="viewport" content="width=device-width,initial-scale=1,maximum-scale=1"&gt;
&lt;title&gt;Prelievo Fascicolo&lt;/title&gt;
&lt;link href="https://fonts.googleapis.com/css2?family=DM+Serif+Display&amp;family=DM+Sans:opsz,wght@9..40,400;9..40,500;9..40,600&amp;display=swap" rel="stylesheet"&gt;
&lt;style&gt;
:root{--bg:#0f0f0f;--s:#1a1a1a;--s2:#242424;--b:#333;--a:#e8c97a;--t:#f0ece0;--t2:#a09880;--t3:#6a6258;--ok:#5aad7a;--err:#e05555;}
*{box-sizing:border-box;margin:0;padding:0;}
body{font-family:'DM Sans',sans-serif;background:var(--bg);color:var(--t);min-height:100vh;}
.hdr{background:var(--s);border-bottom:1px solid var(--b);padding:16px 20px;}
.hdr h1{font-family:'DM Serif Display',serif;font-size:18px;color:var(--a);}
.hdr p{font-size:11px;color:var(--t3);}
.wrap{padding:18px;max-width:480px;margin:0 auto;}
.lcard{background:var(--s);border:1px solid var(--b);border-radius:10px;padding:16px;margin-bottom:18px;border-left:3px solid var(--a);}
.lcard h2{font-family:'DM Serif Display',serif;font-size:19px;margin-bottom:3px;}
.lcard p{font-size:12px;color:var(--t3);}
.sect{font-size:10px;font-weight:700;letter-spacing:.1em;text-transform:uppercase;color:var(--t3);margin-bottom:9px;}
.fitem{background:var(--s);border:1px solid var(--b);border-radius:8px;padding:13px;margin-bottom:7px;cursor:pointer;transition:all .15s;}
.fitem.sel{border-color:var(--a);background:rgba(232,201,122,.07);}
.fnum{font-size:15px;font-weight:700;color:var(--a);margin-bottom:2px;}
.fogg{font-size:12px;color:var(--t2);margin-bottom:5px;}
.fmeta{font-size:11px;color:var(--t3);}
.badge{display:inline-flex;align-items:center;padding:2px 8px;border-radius:20px;font-size:11px;font-weight:600;}
.badge::before{content:'';width:4px;height:4px;border-radius:50%;background:currentColor;margin-right:5px;}
.bin{background:rgba(90,173,122,.12);color:var(--ok);}
.bout{background:rgba(224,85,85,.12);color:var(--err);}
.panel{background:var(--s);border:1px solid var(--b);border-radius:10px;padding:18px;margin-top:14px;display:none;}
.panel.show{display:block;}
label{display:block;font-size:10.5px;font-weight:700;color:var(--t2);text-transform:uppercase;letter-spacing:.06em;margin-bottom:5px;}
input{width:100%;padding:11px 13px;background:var(--s2);border:1px solid var(--b);border-radius:7px;color:var(--t);font-family:'DM Sans',sans-serif;font-size:15px;outline:none;margin-bottom:12px;}
input:focus{border-color:var(--a);}
.btn{width:100%;padding:13px;border:none;border-radius:8px;font-family:'DM Sans',sans-serif;font-size:14px;font-weight:600;cursor:pointer;margin-bottom:7px;}
.bp{background:var(--err);color:#fff;}
.br{background:var(--ok);color:#fff;}
.bc{background:var(--s2);color:var(--t2);border:1px solid var(--b);}
.err{background:rgba(224,85,85,.1);border:1px solid rgba(224,85,85,.3);border-radius:7px;padding:11px 13px;color:var(--err);font-size:12.5px;margin-bottom:12px;}
.ok-screen{text-align:center;padding:44px 20px;}
.ok-screen .ic{font-size:54px;margin-bottom:12px;}
.ok-screen h2{font-family:'DM Serif Display',serif;font-size:24px;color:var(--ok);margin-bottom:8px;}
.ok-screen p{color:var(--t2);font-size:13px;margin-bottom:20px;line-height:1.6;}
.ok-screen button{background:var(--s2);border:1px solid var(--b);color:var(--t);padding:10px 22px;border-radius:7px;font-family:'DM Sans',sans-serif;font-size:13px;cursor:pointer;}
&lt;/style&gt;
&lt;/head&gt;
&lt;body&gt;
&lt;div class="hdr"&gt;&lt;h1&gt;Archivio Fascicoli&lt;/h1&gt;&lt;p&gt;Registra prelievo o restituzione&lt;/p&gt;&lt;/div&gt;
&lt;div class="wrap" id="app"&gt;&lt;p style="padding:30px;text-align:center;color:#6a6258"&gt;Caricamento...&lt;/p&gt;&lt;/div&gt;
&lt;script&gt;
const luogoId=new URLSearchParams(location.search).get('luogo');
<span class="comment">// ⬇ Sostituisci con l'URL del tuo Worker Cloudflare</span>
const API='https://archivio-api.TUO-ACCOUNT.workers.dev';
let data=null,sel=null;
async function init(){
  if(!luogoId){document.getElementById('app').innerHTML='&lt;p style="padding:30px;text-align:center;color:#e05555"&gt;QR non valido&lt;/p&gt;';return;}
  try{
    const r=await fetch(API+'/api/luoghi/'+luogoId+'/qr');
    if(!r.ok)throw new Error();
    data=await r.json();render();
  }catch{document.getElementById('app').innerHTML='&lt;p style="padding:30px;text-align:center;color:#e05555"&gt;Impossibile caricare i dati&lt;/p&gt;';}
}
function render(){
  const {luogo,fascicoli}=data;
  document.getElementById('app').innerHTML=`
    &lt;div class="lcard"&gt;&lt;h2&gt;${luogo.nome}&lt;/h2&gt;${luogo.descrizione?'&lt;p&gt;'+luogo.descrizione+'&lt;/p&gt;':''}&lt;/div&gt;
    &lt;div class="sect"&gt;${fascicoli.length} fascicoli — selezionane uno&lt;/div&gt;
    ${fascicoli.map(f=>`&lt;div class="fitem" id="fi-${f.id}" onclick="pick('${f.id}')"&gt;
      &lt;div style="display:flex;justify-content:space-between;align-items:flex-start"&gt;
        &lt;div class="fnum"&gt;${f.numero}/${f.anno}&lt;/div&gt;
        &lt;span class="badge ${f.stato==='prelevato'?'bout':'bin'}"&gt;${f.stato==='prelevato'?'Prelevato':'In sede'}&lt;/span&gt;
      &lt;/div&gt;
      ${f.oggetto?'&lt;div class="fogg"&gt;'+f.oggetto+'&lt;/div&gt;':''}
      &lt;div class="fmeta"&gt;${[f.parte1,f.parte2].filter(Boolean).join(' vs ')}&lt;/div&gt;
    &lt;/div&gt;`).join('')}
    &lt;div class="panel" id="panel"&gt;
      &lt;div style="font-size:14px;font-weight:600;margin-bottom:12px" id="ptitle"&gt;&lt;/div&gt;
      &lt;div id="perr"&gt;&lt;/div&gt;
      &lt;label&gt;Il tuo nome *&lt;/label&gt;
      &lt;input id="pnome" placeholder="Es. Mario Rossi" autocomplete="name"&gt;
      &lt;label&gt;Note (opzionale)&lt;/label&gt;
      &lt;input id="pnote" placeholder="Motivo..."&gt;
      &lt;button class="btn" id="pbtn" onclick="submit()"&gt;&lt;/button&gt;
      &lt;button class="btn bc" onclick="desel()"&gt;Annulla&lt;/button&gt;
    &lt;/div&gt;`;
}
function pick(id){
  document.querySelectorAll('.fitem').forEach(e=>e.classList.remove('sel'));
  document.getElementById('fi-'+id).classList.add('sel');
  sel=data.fascicoli.find(f=>f.id===id);
  const isOut=sel.stato==='prelevato';
  document.getElementById('ptitle').textContent=isOut?'Registra restituzione':'Registra prelievo';
  const btn=document.getElementById('pbtn');
  btn.textContent=isOut?'↩ Restituisci':'↑ Preleva';
  btn.className='btn '+(isOut?'br':'bp');
  btn.dataset.azione=isOut?'restituzione':'prelievo';
  document.getElementById('panel').classList.add('show');
  document.getElementById('panel').scrollIntoView({behavior:'smooth'});
  document.getElementById('pnome').focus();
}
function desel(){sel=null;document.querySelectorAll('.fitem').forEach(e=>e.classList.remove('sel'));document.getElementById('panel').classList.remove('show');}
async function submit(){
  const nome=document.getElementById('pnome').value.trim();
  if(!nome){document.getElementById('perr').innerHTML='&lt;div class="err"&gt;Inserisci il tuo nome&lt;/div&gt;';return;}
  document.getElementById('perr').innerHTML='';
  const azione=document.getElementById('pbtn').dataset.azione;
  try{
    const r=await fetch(API+'/api/prelievi',{method:'POST',headers:{'Content-Type':'application/json'},body:JSON.stringify({fascicolo_id:sel.id,operatore:nome,azione,note:document.getElementById('pnote').value.trim()})});
    if(!r.ok)throw new Error();
    document.getElementById('app').innerHTML=`&lt;div class="ok-screen"&gt;&lt;div class="ic"&gt;${azione==='prelievo'?'📤':'📥'}&lt;/div&gt;&lt;h2&gt;${azione==='prelievo'?'Prelievo registrato':'Restituzione registrata'}&lt;/h2&gt;&lt;p&gt;Fascicolo &lt;strong style="color:#e8c97a"&gt;${sel.numero}/${sel.anno}&lt;/strong&gt;&lt;br&gt;Operatore: &lt;strong&gt;${nome}&lt;/strong&gt;&lt;br&gt;${new Date().toLocaleString('it-IT')}&lt;/p&gt;&lt;button onclick="location.reload()"&gt;← Torna all'elenco&lt;/button&gt;&lt;/div&gt;`;
  }catch{document.getElementById('perr').innerHTML='&lt;div class="err"&gt;Errore. Riprova.&lt;/div&gt;';}
}
init();
&lt;/script&gt;
&lt;/body&gt;&lt;/html&gt;</span></div>
        </div>

        <!-- STEP 4 -->
        <div class="step-card">
          <div class="step-num">4</div>
          <div class="step-title">Configura e carica su Cloudflare Pages</div>
          <div class="step-desc">
            1. Nel codice del Worker (Step 2), annota l'URL del Worker: es. <code>https://archivio-api.tuoaccount.workers.dev</code><br>
            2. Nel file <code>prelievo.html</code> (Step 3), sostituisci <code>TUO-ACCOUNT</code> con il tuo valore<br>
            3. In questo file <code>index.html</code>, trova la riga <code>const API_URL</code> e aggiorna con il tuo Worker URL<br>
            4. Vai su <strong>Workers & Pages → Pages → Upload assets</strong> → carica <code>index.html</code> + <code>prelievo.html</code>
          </div>
          <div class="deploy-note">
            <strong>Configurazione API URL in questo file:</strong> trova la riga <code>const API_URL = ''</code> nello script JS e metti l'URL del tuo Worker. Finché rimane vuoto, l'app usa localStorage come demo locale.
          </div>
        </div>

        <div style="margin-top:18px;padding:16px 18px;background:rgba(90,173,122,0.07);border:1px solid rgba(90,173,122,0.2);border-radius:var(--radius-lg);font-size:13px;color:var(--text2);line-height:1.7">
          ✅ <strong style="color:var(--success)">Una volta completato il deploy:</strong> i QR dei luoghi puntano a <code style="font-size:11px">https://tuo-progetto.pages.dev/prelievo.html?luogo=ID</code> — scansionali con lo smartphone e registra prelievi in tempo reale, sincronizzati su tutti i dispositivi.
        </div>
      </div>
    </div>

  </div><!-- /content -->
</main>
</div><!-- /shell -->

<!-- ══ MODALS ══ -->

<!-- Fascicolo -->
<div class="overlay" id="m-fasc">
  <div class="modal modal-lg">
    <div class="modal-title" id="m-fasc-title">Nuovo fascicolo</div>
    <div class="frow">
      <div class="fg"><label class="fl">Numero *</label><input class="fi" id="fn" placeholder="1234"></div>
      <div class="fg"><label class="fl">Anno *</label><input class="fi" id="fa" placeholder="2024" type="number"></div>
    </div>
    <div class="fg"><label class="fl">Oggetto</label><input class="fi" id="fo" placeholder="Descrizione oggetto"></div>
    <div class="frow">
      <div class="fg"><label class="fl">Parte 1</label><input class="fi" id="fp1" placeholder="Ricorrente / Attore"></div>
      <div class="fg"><label class="fl">Parte 2</label><input class="fi" id="fp2" placeholder="Resistente / Convenuto"></div>
    </div>
    <div class="frow">
      <div class="fg"><label class="fl">Giudice</label><input class="fi" id="fg2"></div>
      <div class="fg"><label class="fl">Luogo</label><select class="fs" id="fl2"><option value="">-- Nessun luogo --</option></select></div>
    </div>
    <div class="fg"><label class="fl">Note</label><textarea class="ft" id="fnt"></textarea></div>
    <input type="hidden" id="fid">
    <div class="modal-foot">
      <button class="btn btn-ghost" onclick="close_m('m-fasc')">Annulla</button>
      <button class="btn btn-primary" onclick="saveFasc()">Salva fascicolo</button>
    </div>
  </div>
</div>

<!-- Luogo -->
<div class="overlay" id="m-luogo">
  <div class="modal">
    <div class="modal-title" id="m-luogo-title">Nuovo luogo</div>
    <div class="fg"><label class="fl">Nome *</label><input class="fi" id="ln" placeholder="es. Scaffale A3 – Piano 2"></div>
    <div class="fg"><label class="fl">Descrizione</label><textarea class="ft" id="ld" placeholder="Posizione fisica, note..."></textarea></div>
    <input type="hidden" id="lid">
    <div class="modal-foot">
      <button class="btn btn-ghost" onclick="close_m('m-luogo')">Annulla</button>
      <button class="btn btn-primary" onclick="saveLuogo()">Salva luogo</button>
    </div>
  </div>
</div>

<!-- QR -->
<div class="overlay" id="m-qr">
  <div class="modal">
    <div class="modal-title">QR Code — Luogo</div>
    <div style="text-align:center;margin-bottom:12px"><div id="qr-box"></div></div>
    <div style="font-size:14px;font-weight:600;margin-bottom:4px" id="qr-nome"></div>
    <div class="qr-url-box" id="qr-url"></div>
    <div class="qr-list" id="qr-list"></div>
    <div class="modal-foot">
      <button class="btn btn-ghost" onclick="close_m('m-qr')">Chiudi</button>
      <button class="btn btn-primary" onclick="printQR()"><svg fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17 17h2a2 2 0 002-2v-4a2 2 0 00-2-2H5a2 2 0 00-2 2v4a2 2 0 002 2h2m2 4h6a2 2 0 002-2v-4a2 2 0 00-2-2H9a2 2 0 00-2 2v4a2 2 0 002 2zm8-12V5a2 2 0 00-2-2H9a2 2 0 00-2 2v4h10z"/></svg> Stampa</button>
    </div>
  </div>
</div>

<!-- Prelievo -->
<div class="overlay" id="m-prel">
  <div class="modal">
    <div class="modal-title" id="m-prel-title">Registra prelievo</div>
    <div class="pinfo" id="pinfo"></div>
    <div class="fg"><label class="fl">Operatore *</label><input class="fi" id="pop" placeholder="Nome e cognome"></div>
    <div class="fg"><label class="fl">Note</label><input class="fi" id="pnote" placeholder="Motivo..."></div>
    <input type="hidden" id="pfid">
    <input type="hidden" id="paz">
    <div class="modal-foot">
      <button class="btn btn-ghost" onclick="close_m('m-prel')">Annulla</button>
      <button class="btn btn-primary" id="p-btn" onclick="savePrel()">Conferma</button>
    </div>
  </div>
</div>

<!-- Detail -->
<div class="overlay" id="m-det">
  <div class="modal modal-lg">
    <div class="modal-title" id="det-title"></div>
    <div class="tabs">
      <div class="tab active" onclick="switchTab('det',this)">Dettagli</div>
      <div class="tab" onclick="switchTab('hist',this)">Storico prelievi</div>
    </div>
    <div id="tab-det"></div>
    <div id="tab-hist" style="display:none"></div>
    <div class="modal-foot">
      <button class="btn btn-ghost" onclick="close_m('m-det')">Chiudi</button>
      <button class="btn btn-primary" id="det-prel-btn">Registra prelievo</button>
    </div>
  </div>
</div>

<!-- Confirm -->
<div class="overlay" id="m-conf">
  <div class="modal confirm-modal">
    <div class="confirm-icon"><svg fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 9v2m0 4h.01M10.29 3.86L1.82 18a2 2 0 001.71 3h16.94a2 2 0 001.71-3L13.71 3.86a2 2 0 00-3.42 0z"/></svg></div>
    <div style="font-size:16px;font-weight:600;margin-bottom:8px">Conferma eliminazione</div>
    <div class="confirm-text" id="conf-txt"></div>
    <div class="confirm-btns">
      <button class="btn btn-ghost" onclick="close_m('m-conf')">Annulla</button>
      <button class="btn btn-danger" id="conf-yes">Elimina</button>
    </div>
  </div>
</div>

<div id="toasts"></div>

<script>
// ═══════════════════════════════════════════════════════════
// CONFIGURAZIONE
// Se hai deployato il Worker su Cloudflare, metti qui l'URL.
// Es: const API_URL = 'https://archivio-api.tuoaccount.workers.dev';
// Se vuoto → modalità localStorage (demo locale, un solo dispositivo)
const API_URL = '';
// ═══════════════════════════════════════════════════════════

const USE_API = !!API_URL;
let DB = { fascicoli:[], luoghi:[], prelievi:[] };
let luoghiCache = [];
let _importData = null, _importHdr = null;

// ── STORAGE ──
function ls_load(){ const d=localStorage.getItem('af_db'); if(d) DB=JSON.parse(d); }
function ls_save(){ localStorage.setItem('af_db', JSON.stringify(DB)); }
function uid(){ return Date.now().toString(36)+Math.random().toString(36).slice(2,7); }

// ── API LAYER ──
async function req(path, method='GET', body=null){
  if(!USE_API) return ls_op(path, method, body);
  const opts={method,headers:{'Content-Type':'application/json'}};
  if(body) opts.body=JSON.stringify(body);
  const r=await fetch(API_URL+'/api/'+path, opts);
  if(!r.ok){ const e=await r.json().catch(()=>({})); throw new Error(e.error||'Errore'); }
  return r.json();
}

// ── LOCALSTORAGE OPS (demo) ──
function ls_op(path, method, body){
  const p=path.replace(/[?].*$/,''), qs=path.includes('?')?Object.fromEntries(new URLSearchParams(path.split('?')[1])):{};
  if(p==='stats'){
    return Promise.resolve({
      tot:DB.fascicoli.length,
      inSede:DB.fascicoli.filter(f=>!f.stato||f.stato==='in_sede').length,
      prelevati:DB.fascicoli.filter(f=>f.stato==='prelevato').length,
      luoghi:DB.luoghi.length,
      ultPrel:[...DB.prelievi].reverse().slice(0,5).map(p=>{const f=DB.fascicoli.find(x=>x.id===p.fascicolo_id)||{};return{...p,numero:f.numero,anno:f.anno};}),
      ultFasc:[...DB.fascicoli].reverse().slice(0,5)
    });
  }
  if(p==='luoghi'){
    if(method==='GET') return Promise.resolve(DB.luoghi.map(l=>({...l,cnt:DB.fascicoli.filter(f=>f.luogo_id===l.id).length,out:DB.fascicoli.filter(f=>f.luogo_id===l.id&&f.stato==='prelevato').length})));
    if(method==='POST'){const id=uid();const obj={id,...body};DB.luoghi.push(obj);ls_save();return Promise.resolve(obj);}
  }
  const lm=p.match(/^luoghi\/([^/]+)$/);
  if(lm){
    const id=lm[1];
    if(method==='PUT'){const i=DB.luoghi.findIndex(x=>x.id===id);if(i>=0){DB.luoghi[i]={...DB.luoghi[i],...body};ls_save();}return Promise.resolve({ok:true});}
    if(method==='DELETE'){DB.luoghi=DB.luoghi.filter(x=>x.id!==id);DB.fascicoli.forEach(f=>{if(f.luogo_id===id)f.luogo_id='';});ls_save();return Promise.resolve({ok:true});}
  }
  if(p.match(/^luoghi\/([^/]+)\/qr$/)){
    const id=p.split('/')[1];
    const luogo=DB.luoghi.find(x=>x.id===id);
    const fascicoli=DB.fascicoli.filter(f=>f.luogo_id===id);
    return Promise.resolve({luogo,fascicoli});
  }
  if(p==='fascicoli'){
    if(method==='GET'){
      const q=(qs.q||'').toLowerCase(), stato=qs.stato||'', luogo=qs.luogo||'';
      const lmap=Object.fromEntries(DB.luoghi.map(x=>[x.id,x.nome]));
      let list=DB.fascicoli.map(f=>({...f,luogo_nome:f.luogo_id?lmap[f.luogo_id]||'':''}));
      if(q) list=list.filter(f=>[f.numero,f.anno,f.oggetto,f.parte1,f.parte2,f.giudice].some(v=>(v||'').toLowerCase().includes(q)));
      if(stato) list=list.filter(f=>(f.stato||'in_sede')===(stato==='in'?'in_sede':'prelevato'));
      if(luogo) list=list.filter(f=>f.luogo_id===luogo);
      return Promise.resolve(list);
    }
    if(method==='POST'){
      if(Array.isArray(body)){body.forEach(f=>DB.fascicoli.push({id:uid(),...f,stato:'in_sede',creato_il:new Date().toISOString()}));ls_save();return Promise.resolve({added:body.length});}
      const obj={id:uid(),...body,stato:'in_sede',creato_il:new Date().toISOString()};DB.fascicoli.push(obj);ls_save();return Promise.resolve(obj);
    }
  }
  const fm=p.match(/^fascicoli\/([^/]+)$/);
  if(fm){
    const id=fm[1],lmap=Object.fromEntries(DB.luoghi.map(x=>[x.id,x.nome]));
    if(method==='GET'){const f=DB.fascicoli.find(x=>x.id===id);return Promise.resolve({...f,luogo_nome:f&&f.luogo_id?lmap[f.luogo_id]||'':''});}
    if(method==='PUT'){const i=DB.fascicoli.findIndex(x=>x.id===id);if(i>=0)DB.fascicoli[i]={...DB.fascicoli[i],...body};ls_save();return Promise.resolve({ok:true});}
    if(method==='DELETE'){DB.fascicoli=DB.fascicoli.filter(x=>x.id!==id);DB.prelievi=DB.prelievi.filter(x=>x.fascicolo_id!==id);ls_save();return Promise.resolve({ok:true});}
  }
  if(p.match(/^fascicoli\/([^/]+)\/prelievi$/)){
    const id=p.split('/')[1];
    return Promise.resolve(DB.prelievi.filter(x=>x.fascicolo_id===id).reverse());
  }
  if(p==='prelievi'){
    if(method==='GET'){
      const q=(qs.q||'').toLowerCase();
      let list=[...DB.prelievi].reverse().map(p=>{const f=DB.fascicoli.find(x=>x.id===p.fascicolo_id)||{};return{...p,numero:f.numero,anno:f.anno};});
      if(q) list=list.filter(p=>(p.operatore||'').toLowerCase().includes(q)||(p.numero||'').includes(q)||(p.anno||'').includes(q));
      return Promise.resolve(list);
    }
    if(method==='POST'){
      const id=uid();const obj={id,...body,data_ora:new Date().toISOString()};DB.prelievi.push(obj);
      const i=DB.fascicoli.findIndex(x=>x.id===body.fascicolo_id);
      if(i>=0) DB.fascicoli[i].stato=body.azione==='prelievo'?'prelevato':'in_sede';
      ls_save();return Promise.resolve({id,stato:body.azione==='prelievo'?'prelevato':'in_sede'});
    }
  }
  return Promise.resolve(null);
}

// ── NAVIGATE ──
function go(page){
  document.querySelectorAll('.page').forEach(p=>p.classList.remove('active'));
  document.querySelectorAll('.nav-item').forEach(n=>n.classList.remove('active'));
  document.getElementById('page-'+page).classList.add('active');
  document.querySelectorAll('.nav-item').forEach(n=>{if((n.getAttribute('onclick')||'').includes("'"+page+"'"))n.classList.add('active');});
  const titles={dashboard:'Dashboard',fascicoli:'Fascicoli',luoghi:'Luoghi',prelievi:'Prelievi',import:'Import Excel',deploy:'Deploy Cloudflare'};
  document.getElementById('pg-title').textContent=titles[page]||page;
  document.getElementById('pg-sub').textContent=USE_API?'● Cloudflare D1':'○ localStorage (demo)';
  const acts=document.getElementById('pg-actions');acts.innerHTML='';
  if(page==='fascicoli') acts.innerHTML=`<button class="btn btn-ghost btn-sm" onclick="exportFasc()">⬇ Esporta</button><button class="btn btn-primary btn-sm" onclick="openFasc()">+ Nuovo fascicolo</button>`;
  if(page==='luoghi') acts.innerHTML=`<button class="btn btn-primary btn-sm" onclick="openLuogo()">+ Nuovo luogo</button>`;
  if(page==='dashboard') loadDash();
  if(page==='fascicoli'){loadLuoghiCache().then(()=>{fillLuogoFilter();renderFasc();});}
  if(page==='luoghi') renderLuoghi();
  if(page==='prelievi') renderPrel();
}

// ── DASHBOARD ──
async function loadDash(){
  try{
    const s=await req('stats');
    const colors=['--accent','--success','--danger','--info'];
    const labels=['Fascicoli totali','In sede','Prelevati','Luoghi attivi'];
    const vals=[s.tot,s.inSede,s.prelevati,s.luoghi];
    document.getElementById('stats').innerHTML=vals.map((v,i)=>`
      <div class="stat" style="--accent-color:var(${colors[i]})">
        <div class="stat-val" style="color:var(${colors[i]})">${v}</div>
        <div class="stat-lbl">${labels[i]}</div>
      </div>`).join('');
    const rf=s.ultFasc||[];
    document.getElementById('dash-fasc').innerHTML=rf.length?rf.map(f=>`
      <div style="display:flex;justify-content:space-between;align-items:center;padding:8px 0;border-bottom:1px solid var(--border);font-size:13px">
        <span style="color:var(--accent);font-weight:600">${f.numero}/${f.anno}</span>
        <span style="color:var(--text2);flex:1;margin:0 10px;overflow:hidden;text-overflow:ellipsis;white-space:nowrap">${f.oggetto||'—'}</span>
        <span class="badge ${f.stato==='prelevato'?'badge-out':'badge-in'}">${f.stato==='prelevato'?'Prelevato':'In sede'}</span>
      </div>`).join(''):'<div style="padding:18px;text-align:center;color:var(--text3);font-size:13px">Nessun fascicolo ancora</div>';
    const rp=s.ultPrel||[];
    document.getElementById('dash-prel').innerHTML=rp.length?rp.map(p=>{const d=new Date(p.data_ora);return`
      <div style="display:flex;justify-content:space-between;align-items:center;padding:8px 0;border-bottom:1px solid var(--border);font-size:13px">
        <span style="color:var(--text3);font-size:11px">${d.toLocaleDateString('it-IT')}</span>
        <span style="color:var(--accent);font-weight:600">${p.numero||''}/${p.anno||''}</span>
        <span style="color:var(--text2)">${p.operatore}</span>
      </div>`}).join(''):'<div style="padding:18px;text-align:center;color:var(--text3);font-size:13px">Nessun prelievo ancora</div>';
  }catch(e){toast('Errore dashboard','err');}
}

// ── FASCICOLI ──
async function loadLuoghiCache(){ luoghiCache=await req('luoghi'); return luoghiCache; }
function fillLuogoFilter(){
  const sel=document.getElementById('filt-luogo'),cur=sel.value;
  sel.innerHTML='<option value="">Tutti i luoghi</option>'+luoghiCache.map(l=>`<option value="${l.id}">${l.nome}</option>`).join('');
  sel.value=cur;
}
async function renderFasc(){
  const q=document.getElementById('q-fasc').value||'';
  const stato=document.getElementById('filt-stato').value;
  const luogo=document.getElementById('filt-luogo').value;
  try{
    const list=await req(`fascicoli?q=${encodeURIComponent(q)}&stato=${stato}&luogo=${luogo}`);
    const tb=document.getElementById('tb-fasc'),em=document.getElementById('empty-fasc');
    if(!list.length){tb.innerHTML='';em.style.display='block';return;}
    em.style.display='none';
    tb.innerHTML=list.map(f=>`<tr>
      <td class="td-primary" onclick="openDet('${f.id}')">${f.numero}/${f.anno}</td>
      <td>${f.oggetto||'—'}</td>
      <td>${f.parte1||'—'}</td>
      <td>${f.parte2||'—'}</td>
      <td class="td-muted">${f.giudice||'—'}</td>
      <td>${f.luogo_nome||'—'}</td>
      <td><span class="badge ${f.stato==='prelevato'?'badge-out':'badge-in'}">${f.stato==='prelevato'?'Prelevato':'In sede'}</span></td>
      <td><div style="display:flex;gap:4px">
        <button class="btn btn-sm ${f.stato==='prelevato'?'btn-success':'btn-ghost'}" onclick="openPrel('${f.id}','${f.stato||'in_sede'}')" title="${f.stato==='prelevato'?'Restituisci':'Preleva'}">${f.stato==='prelevato'?'↩':'↑'}</button>
        <button class="btn btn-sm btn-ghost" onclick="openFasc('${f.id}')">✏</button>
        <button class="btn btn-sm btn-danger" onclick="confirmDel('fascicolo','${f.id}')">✕</button>
      </div></td>
    </tr>`).join('');
  }catch(e){document.getElementById('tb-fasc').innerHTML=`<tr><td colspan="8" class="lrow" style="color:var(--danger)">${e.message}</td></tr>`;}
}
async function openFasc(id){
  await loadLuoghiCache();
  document.getElementById('fl2').innerHTML='<option value="">-- Nessun luogo --</option>'+luoghiCache.map(l=>`<option value="${l.id}">${l.nome}</option>`).join('');
  if(id){
    try{
      const f=await req('fascicoli/'+id);
      document.getElementById('m-fasc-title').textContent='Modifica fascicolo';
      document.getElementById('fn').value=f.numero||'';
      document.getElementById('fa').value=f.anno||'';
      document.getElementById('fo').value=f.oggetto||'';
      document.getElementById('fp1').value=f.parte1||'';
      document.getElementById('fp2').value=f.parte2||'';
      document.getElementById('fg2').value=f.giudice||'';
      document.getElementById('fl2').value=f.luogo_id||'';
      document.getElementById('fnt').value=f.note||'';
      document.getElementById('fid').value=id;
    }catch{toast('Errore','err');return;}
  }else{
    document.getElementById('m-fasc-title').textContent='Nuovo fascicolo';
    ['fn','fa','fo','fp1','fp2','fg2','fnt'].forEach(x=>document.getElementById(x).value='');
    document.getElementById('fid').value='';
    document.getElementById('fl2').value='';
  }
  open_m('m-fasc');
}
async function saveFasc(){
  const n=document.getElementById('fn').value.trim(),a=document.getElementById('fa').value.trim();
  if(!n||!a){toast('Numero e Anno sono obbligatori','err');return;}
  const id=document.getElementById('fid').value;
  const d={numero:n,anno:a,oggetto:document.getElementById('fo').value.trim(),parte1:document.getElementById('fp1').value.trim(),parte2:document.getElementById('fp2').value.trim(),giudice:document.getElementById('fg2').value.trim(),luogo_id:document.getElementById('fl2').value,note:document.getElementById('fnt').value.trim()};
  try{
    if(id) await req('fascicoli/'+id,'PUT',d);
    else await req('fascicoli','POST',d);
    toast(id?'Fascicolo aggiornato':'Fascicolo creato','ok');
    close_m('m-fasc');renderFasc();
  }catch(e){toast(e.message,'err');}
}

// ── LUOGHI ──
async function renderLuoghi(){
  try{
    const list=await req('luoghi');
    luoghiCache=list;
    const grid=document.getElementById('grid-luoghi'),em=document.getElementById('empty-luoghi');
    if(!list.length){grid.innerHTML='';em.style.display='block';return;}
    em.style.display='none';
    grid.innerHTML=list.map(l=>`
      <div class="lcard">
        <div class="lcard-name">${l.nome}</div>
        <div class="lcard-desc">${l.descrizione||'Nessuna descrizione'}</div>
        <div class="lcard-meta">${l.cnt||0} fascicoli${l.out>0?` · <span style="color:var(--danger)">${l.out} prelevati</span>`:''}</div>
        <div class="lcard-actions">
          <button class="btn btn-sm btn-ghost" onclick="showQR('${l.id}','${esc(l.nome)}')">
            <svg fill="none" stroke="currentColor" viewBox="0 0 24 24"><rect x="3" y="3" width="7" height="7" rx="1"/><rect x="14" y="3" width="7" height="7" rx="1"/><rect x="3" y="14" width="7" height="7" rx="1"/><path d="M14 14h3v3"/><path d="M17 20h3"/><path d="M20 17v3"/></svg> QR
          </button>
          <button class="btn btn-sm btn-ghost" onclick="openLuogo('${l.id}')">✏ Modifica</button>
          <button class="btn btn-sm btn-danger" onclick="confirmDel('luogo','${l.id}')">✕</button>
        </div>
      </div>`).join('');
  }catch(e){toast('Errore luoghi','err');}
}
function openLuogo(id){
  if(id){
    const l=luoghiCache.find(x=>x.id===id);
    if(l){document.getElementById('m-luogo-title').textContent='Modifica luogo';document.getElementById('ln').value=l.nome||'';document.getElementById('ld').value=l.descrizione||'';document.getElementById('lid').value=id;}
  }else{
    document.getElementById('m-luogo-title').textContent='Nuovo luogo';
    document.getElementById('ln').value='';document.getElementById('ld').value='';document.getElementById('lid').value='';
  }
  open_m('m-luogo');
}
async function saveLuogo(){
  const nome=document.getElementById('ln').value.trim();
  if(!nome){toast('Il nome è obbligatorio','err');return;}
  const id=document.getElementById('lid').value;
  try{
    if(id) await req('luoghi/'+id,'PUT',{nome,descrizione:document.getElementById('ld').value.trim()});
    else await req('luoghi','POST',{nome,descrizione:document.getElementById('ld').value.trim()});
    toast(id?'Luogo aggiornato':'Luogo creato','ok');
    close_m('m-luogo');renderLuoghi();
  }catch(e){toast(e.message,'err');}
}

// ── QR ──
async function showQR(luogoId, luogoNome){
  const qrUrl = USE_API
    ? `${location.origin}/prelievo.html?luogo=${luogoId}`
    : `[Deploy su Cloudflare per QR funzionale] — luogo ID: ${luogoId}`;
  document.getElementById('qr-nome').textContent=luogoNome;
  document.getElementById('qr-url').textContent=qrUrl;
  const box=document.getElementById('qr-box');
  box.innerHTML='';
  new QRCode(box,{text:qrUrl,width:200,height:200,colorDark:'#000',colorLight:'#fff'});
  try{
    const d=await req('luoghi/'+luogoId+'/qr');
    document.getElementById('qr-list').innerHTML=(d.fascicoli||[]).length
      ?(d.fascicoli||[]).map(f=>`<div class="qr-list-item"><span><strong>${f.numero}/${f.anno}</strong>${f.oggetto?' · '+f.oggetto:''}</span><span class="badge ${f.stato==='prelevato'?'badge-out':'badge-in'}">${f.stato==='prelevato'?'Prelevato':'In sede'}</span></div>`).join('')
      :'<div style="padding:10px;color:var(--text3);font-size:12px">Nessun fascicolo assegnato</div>';
  }catch{}
  open_m('m-qr');
}
function printQR(){
  const canvas=document.querySelector('#qr-box canvas');if(!canvas)return;
  const nome=document.getElementById('qr-nome').textContent;
  const url=document.getElementById('qr-url').textContent;
  const list=document.getElementById('qr-list').innerText;
  const w=window.open('','_blank');
  w.document.write(`<html><head><title>QR ${nome}</title><style>body{font-family:sans-serif;padding:28px;text-align:center}h2{font-size:20px;margin-bottom:4px}p{color:#888;font-size:11px;margin-bottom:14px}pre{text-align:left;font-size:11px;line-height:1.7;max-width:300px;margin:14px auto 0;white-space:pre-wrap}</style></head><body><h2>${nome}</h2><p>${url}</p><img src="${canvas.toDataURL()}" width="210" style="border-radius:8px"><pre>${list}</pre><script>window.onload=()=>print()<\/script></body></html>`);
  w.document.close();
}

// ── PRELIEVI ──
function openPrel(fascicoloId, stato){
  const isOut=stato==='prelevato';
  document.getElementById('m-prel-title').textContent=isOut?'Registra restituzione':'Registra prelievo';
  document.getElementById('p-btn').textContent=isOut?'Conferma restituzione':'Conferma prelievo';
  document.getElementById('pinfo').innerHTML=`
    <div class="pinfo-row"><span>Fascicolo</span><strong style="color:var(--accent)">${fascicoloId.slice(-8)}</strong></div>
    <div class="pinfo-row"><span>Stato attuale</span><span class="badge ${isOut?'badge-out':'badge-in'}">${isOut?'Prelevato':'In sede'}</span></div>`;
  document.getElementById('pfid').value=fascicoloId;
  document.getElementById('paz').value=isOut?'restituzione':'prelievo';
  document.getElementById('pop').value='';document.getElementById('pnote').value='';
  open_m('m-prel');
}
async function savePrel(){
  const op=document.getElementById('pop').value.trim();
  if(!op){toast('Inserisci il nome operatore','err');return;}
  try{
    await req('prelievi','POST',{fascicolo_id:document.getElementById('pfid').value,operatore:op,azione:document.getElementById('paz').value,note:document.getElementById('pnote').value.trim()});
    toast(document.getElementById('paz').value==='prelievo'?'Prelievo registrato':'Restituzione registrata','ok');
    close_m('m-prel');renderFasc();renderPrel();
  }catch(e){toast(e.message,'err');}
}
async function renderPrel(){
  const q=document.getElementById('q-prel').value||'';
  try{
    const list=await req(`prelievi?q=${encodeURIComponent(q)}`);
    const tb=document.getElementById('tb-prel'),em=document.getElementById('empty-prel');
    if(!list.length){tb.innerHTML='';em.style.display='block';return;}
    em.style.display='none';
    tb.innerHTML=list.map(p=>{const d=new Date(p.data_ora);return`<tr>
      <td class="td-muted">${d.toLocaleDateString('it-IT')} ${d.toLocaleTimeString('it-IT',{hour:'2-digit',minute:'2-digit'})}</td>
      <td style="color:var(--accent);font-weight:600">${p.numero||'?'}/${p.anno||'?'}</td>
      <td>${p.operatore}</td>
      <td><span class="badge ${p.azione==='prelievo'?'badge-out':'badge-in'}">${p.azione==='prelievo'?'↑ Prelievo':'↩ Restituzione'}</span></td>
      <td class="td-muted">${p.note||'—'}</td>
    </tr>`;}).join('');
  }catch(e){document.getElementById('tb-prel').innerHTML=`<tr><td colspan="5" class="lrow" style="color:var(--danger)">${e.message}</td></tr>`;}
}

// ── DETAIL ──
async function openDet(id){
  document.getElementById('det-title').textContent='Caricamento...';
  document.getElementById('tab-det').innerHTML='<div class="lrow"><span class="spinner"></span>Caricamento...</div>';
  document.getElementById('tab-hist').innerHTML='';
  document.querySelectorAll('#m-det .tab').forEach(t=>t.classList.remove('active'));
  document.querySelectorAll('#m-det .tab')[0].classList.add('active');
  document.getElementById('tab-det').style.display='';
  document.getElementById('tab-hist').style.display='none';
  open_m('m-det');
  try{
    const [f,hist]=await Promise.all([req('fascicoli/'+id),req('fascicoli/'+id+'/prelievi')]);
    document.getElementById('det-title').textContent=`Fascicolo ${f.numero}/${f.anno}`;
    document.getElementById('tab-det').innerHTML=[
      ['Numero / Anno',`${f.numero} / ${f.anno}`],
      ['Oggetto',f.oggetto||'—'],['Parte 1',f.parte1||'—'],['Parte 2',f.parte2||'—'],
      ['Giudice',f.giudice||'—'],['Luogo',f.luogo_nome||'—'],
      ['Stato',`<span class="badge ${f.stato==='prelevato'?'badge-out':'badge-in'}">${f.stato==='prelevato'?'Prelevato':'In sede'}</span>`],
      ['Note',f.note||'—']
    ].map(([l,v])=>`<div class="drow"><span class="dlabel">${l}</span><span class="dval">${v}</span></div>`).join('');
    document.getElementById('tab-hist').innerHTML=hist.length
      ?`<table><thead><tr><th>Data/Ora</th><th>Operatore</th><th>Azione</th><th>Note</th></tr></thead><tbody>${
        hist.map(p=>{const d=new Date(p.data_ora);return`<tr><td class="td-muted">${d.toLocaleDateString('it-IT')} ${d.toLocaleTimeString('it-IT',{hour:'2-digit',minute:'2-digit'})}</td><td>${p.operatore}</td><td><span class="badge ${p.azione==='prelievo'?'badge-out':'badge-in'}">${p.azione==='prelievo'?'↑ Prelievo':'↩ Restituzione'}</span></td><td class="td-muted">${p.note||'—'}</td></tr>`;}).join('')
      }</tbody></table>`
      :'<div class="lrow">Nessun prelievo per questo fascicolo</div>';
    const btn=document.getElementById('det-prel-btn');
    btn.textContent=f.stato==='prelevato'?'↩ Registra restituzione':'↑ Registra prelievo';
    btn.onclick=()=>{close_m('m-det');openPrel(id,f.stato||'in_sede');};
  }catch(e){document.getElementById('tab-det').innerHTML=`<div class="lrow" style="color:var(--danger)">${e.message}</div>`;}
}
function switchTab(which,el){
  document.querySelectorAll('#m-det .tab').forEach(t=>t.classList.remove('active'));
  el.classList.add('active');
  document.getElementById('tab-det').style.display=which==='det'?'':'none';
  document.getElementById('tab-hist').style.display=which==='hist'?'':'none';
}

// ── DELETE ──
function confirmDel(type,id){
  const msgs={fascicolo:'Eliminare questo fascicolo? Verranno rimossi anche tutti i prelievi associati.',luogo:'Eliminare questo luogo? I fascicoli perderanno il collegamento.'};
  document.getElementById('conf-txt').textContent=msgs[type];
  document.getElementById('conf-yes').onclick=async()=>{
    close_m('m-conf');
    try{
      await req((type==='fascicolo'?'fascicoli':'luoghi')+'/'+id,'DELETE');
      toast('Eliminato','ok');
      if(type==='fascicolo') renderFasc();
      else renderLuoghi();
    }catch(e){toast(e.message,'err');}
  };
  open_m('m-conf');
}

// ── IMPORT ──
function onFile(e){
  const file=e.target.files[0];if(!file)return;
  const reader=new FileReader();
  reader.onload=ev=>{
    const wb=XLSX.read(ev.target.result,{type:'binary'});
    const ws=wb.Sheets[wb.SheetNames[0]];
    const data=XLSX.utils.sheet_to_json(ws,{header:1});
    if(data.length<2){toast('File vuoto','err');return;}
    _importHdr=data[0].map((h,i)=>h||'Col '+(i+1));
    _importData=data.slice(1).filter(r=>r.some(c=>c));
    renderImpPreview();
  };
  reader.readAsBinaryString(file);
}
function renderImpPreview(){
  const fields=['numero','anno','oggetto','parte1','parte2','giudice','luogo','note'];
  const fnames=['Numero','Anno','Oggetto','Parte 1','Parte 2','Giudice','Luogo','Note'];
  document.getElementById('imp-map').innerHTML=fields.map((f,i)=>`
    <div class="colmap-item"><span>${fnames[i]}</span>
      <select class="fs" id="m-${f}" style="width:auto;padding:3px 7px;font-size:11.5px">
        <option value="">—</option>
        ${_importHdr.map((h,j)=>`<option value="${j}" ${j===i?'selected':''}>${h}</option>`).join('')}
      </select>
    </div>`).join('');
  document.getElementById('imp-count').textContent=`${_importData.length} righe da importare`;
  document.getElementById('imp-preview').style.display='block';
}
async function doImport(){
  const fields=['numero','anno','oggetto','parte1','parte2','giudice','luogo','note'];
  const map={};fields.forEach(f=>{const v=document.getElementById('m-'+f).value;if(v!=='')map[f]=parseInt(v);});
  if(map.numero===undefined||map.anno===undefined){toast('Mappa almeno Numero e Anno','err');return;}
  await loadLuoghiCache();
  const batch=[];
  for(const row of _importData){
    const luogoNome=map.luogo!==undefined?(row[map.luogo]||'').toString().trim():'';
    let luogo_id='';
    if(luogoNome){
      let l=luoghiCache.find(x=>x.nome.toLowerCase()===luogoNome.toLowerCase());
      if(!l){try{l=await req('luoghi','POST',{nome:luogoNome,descrizione:''});luoghiCache.push(l);}catch{}}
      luogo_id=(l&&l.id)||'';
    }
    batch.push({numero:(row[map.numero]||'').toString().trim(),anno:(row[map.anno]||'').toString().trim(),oggetto:map.oggetto!==undefined?(row[map.oggetto]||'').toString().trim():'',parte1:map.parte1!==undefined?(row[map.parte1]||'').toString().trim():'',parte2:map.parte2!==undefined?(row[map.parte2]||'').toString().trim():'',giudice:map.giudice!==undefined?(row[map.giudice]||'').toString().trim():'',luogo_id,note:map.note!==undefined?(row[map.note]||'').toString().trim():''});
  }
  try{
    const r=await req('fascicoli','POST',batch.filter(f=>f.numero&&f.anno));
    toast(`Importati ${r.added} fascicoli`,'ok');
    resetImport();go('fascicoli');
  }catch(e){toast(e.message,'err');}
}
function resetImport(){_importData=null;_importHdr=null;document.getElementById('imp-preview').style.display='none';document.getElementById('fi-file').value='';}
function dlTemplate(){
  const ws=XLSX.utils.aoa_to_sheet([['Numero','Anno','Oggetto','Parte 1','Parte 2','Giudice','Luogo','Note'],['1234','2024','Causa civile','Mario Rossi','Luigi Bianchi','Dr. Verdi','Scaffale A1','Urgente'],['5678','2023','Ricorso','Anna Ferrari','','Dr. Neri','Scaffale B2','']]);
  const wb=XLSX.utils.book_new();XLSX.utils.book_append_sheet(wb,ws,'Fascicoli');XLSX.writeFile(wb,'template_fascicoli.xlsx');
}

// ── EXPORT ──
async function exportFasc(){
  try{
    const list=await req('fascicoli');
    const d=[['Numero','Anno','Oggetto','Parte 1','Parte 2','Giudice','Luogo','Stato','Note']];
    list.forEach(f=>d.push([f.numero,f.anno,f.oggetto,f.parte1,f.parte2,f.giudice,f.luogo_nome||'',f.stato==='prelevato'?'Prelevato':'In sede',f.note]));
    const ws=XLSX.utils.aoa_to_sheet(d);const wb=XLSX.utils.book_new();XLSX.utils.book_append_sheet(wb,ws,'Fascicoli');XLSX.writeFile(wb,'fascicoli.xlsx');
  }catch(e){toast(e.message,'err');}
}
async function exportPrel(){
  try{
    const list=await req('prelievi');
    const d=[['Data','Ora','Fascicolo','Operatore','Azione','Note']];
    list.forEach(p=>{const dt=new Date(p.data_ora);d.push([dt.toLocaleDateString('it-IT'),dt.toLocaleTimeString('it-IT'),`${p.numero||''}/${p.anno||''}`,p.operatore,p.azione,p.note]);});
    const ws=XLSX.utils.aoa_to_sheet(d);const wb=XLSX.utils.book_new();XLSX.utils.book_append_sheet(wb,ws,'Prelievi');XLSX.writeFile(wb,'prelievi.xlsx');
  }catch(e){toast(e.message,'err');}
}

// ── COPY CODE ──
function copyCode(btn){
  const block=btn.parentElement;
  const text=block.innerText.replace('Copia','').replace('Copiato!','').trim();
  navigator.clipboard.writeText(text).then(()=>{btn.textContent='Copiato!';setTimeout(()=>btn.textContent='Copia',2000);});
}

// ── MODAL ──
function open_m(id){document.getElementById(id).classList.add('open');}
function close_m(id){document.getElementById(id).classList.remove('open');}
document.querySelectorAll('.overlay').forEach(o=>{o.addEventListener('click',e=>{if(e.target===o)close_m(o.id);});});

// ── TOAST ──
function toast(msg,type='info'){
  const t=document.createElement('div');
  t.className='toast '+type;t.textContent=msg;
  document.getElementById('toasts').appendChild(t);
  setTimeout(()=>t.remove(),3500);
}

// ── DRAG DROP ──
function esc(s){return(s||'').replace(/'/g,"\\'")}
const dz=document.getElementById('dz');
dz.addEventListener('dragover',e=>{e.preventDefault();dz.classList.add('over');});
dz.addEventListener('dragleave',()=>dz.classList.remove('over'));
dz.addEventListener('drop',e=>{e.preventDefault();dz.classList.remove('over');const f=e.dataTransfer.files[0];if(f){const dt=new DataTransfer();dt.items.add(f);document.getElementById('fi-file').files=dt.files;onFile({target:{files:[f]}});}});

// ── INIT ──
ls_load();
go('dashboard');
</script>
</body>
</html>
# registro-fascicoli

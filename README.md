# Newenzo7__
Sensibilidad y configuraciónes 
<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>newenzo7 | Links</title>
<link href="https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Inter:wght@400;600;700;800&display=swap" rel="stylesheet"/>
<style>
*,*::before,*::after{box-sizing:border-box;margin:0;padding:0}
:root{
  --red:#e00000;--red-dark:#a80000;--red-glow:rgba(224,0,0,0.35);
  --black:#0a0a0a;--card:#1a1a1a;--card-hover:#222;
  --border:rgba(224,0,0,0.2);--text:#fff;--muted:#777
}
html,body{min-height:100%;font-family:'Inter',sans-serif;color:var(--text)}
body{
  background:radial-gradient(ellipse 80% 40% at 50% 0%,rgba(200,0,0,0.18) 0%,transparent 70%),#0a0a0a;
  min-height:100vh;display:flex;flex-direction:column;align-items:center;padding:48px 16px 64px
}
body::before{content:'';position:fixed;inset:0;background:repeating-linear-gradient(0deg,transparent,transparent 2px,rgba(0,0,0,0.04) 2px,rgba(0,0,0,0.04) 4px);pointer-events:none;z-index:0}

.container{position:relative;z-index:1;width:100%;max-width:480px;display:flex;flex-direction:column;align-items:center}

.avatar-ring{width:100px;height:100px;border-radius:50%;background:conic-gradient(var(--red),var(--red-dark),#000,var(--red));padding:3px;animation:spin 6s linear infinite;margin-bottom:18px}
@keyframes spin{to{transform:rotate(360deg)}}
.avatar-inner{width:100%;height:100%;border-radius:50%;background:#0a0a0a;display:flex;align-items:center;justify-content:center;font-family:'Bebas Neue',sans-serif;font-size:36px;color:var(--red);text-shadow:0 0 20px var(--red-glow)}

h1.username{font-family:'Bebas Neue',sans-serif;font-size:34px;letter-spacing:3px;text-shadow:0 0 30px var(--red-glow);margin-bottom:6px}
.tagline{font-size:13px;color:var(--muted);margin-bottom:28px;letter-spacing:.5px}

.socials{display:flex;gap:18px;margin-bottom:32px}
.social-btn{width:44px;height:44px;border-radius:50%;background:var(--card);border:1px solid var(--border);display:flex;align-items:center;justify-content:center;color:var(--text);text-decoration:none;transition:all .2s}
.social-btn:hover{background:var(--red-dark);border-color:var(--red);transform:translateY(-3px);box-shadow:0 6px 24px var(--red-glow)}
.social-btn svg{width:20px;height:20px;fill:currentColor}

.divider{width:100%;height:1px;background:linear-gradient(90deg,transparent,var(--red),transparent);margin-bottom:28px;opacity:.5}

.links{width:100%;display:flex;flex-direction:column;gap:12px}

.sec-label{width:100%;font-size:10px;font-weight:700;letter-spacing:2px;color:var(--red);text-transform:uppercase;display:flex;align-items:center;gap:8px;margin:8px 0 4px}
.sec-label::after{content:'';flex:1;height:1px;background:var(--border)}

.link-card{
  display:flex;align-items:center;gap:14px;width:100%;
  padding:18px 20px;
  background:var(--card);
  border:1px solid var(--border);
  border-radius:16px;
  text-decoration:none;color:var(--text);font-weight:600;
  transition:all .22s cubic-bezier(.4,0,.2,1);
  position:relative;overflow:hidden;cursor:pointer;text-align:left;
  font-family:'Inter',sans-serif;font-size:15px;
}
.link-card::before{content:'';position:absolute;left:0;top:0;bottom:0;width:4px;background:var(--red);border-radius:16px 0 0 16px;opacity:0;transition:opacity .2s}
.link-card:hover,.link-card:focus{background:var(--card-hover);outline:none;transform:translateY(-2px);box-shadow:0 6px 28px var(--red-glow)}
.link-card:hover::before,.link-card:focus::before{opacity:1}
.link-card:hover{border-color:rgba(224,0,0,0.5)}

.licon{width:42px;height:42px;border-radius:11px;background:rgba(224,0,0,0.12);border:1px solid rgba(224,0,0,0.25);display:flex;align-items:center;justify-content:center;flex-shrink:0}
.licon svg{width:22px;height:22px;fill:var(--red)}
.ltxt{flex:1}
.llabel{display:block;font-size:15px;font-weight:700}
.lsub{display:block;font-size:12px;color:var(--muted);font-weight:400;margin-top:2px}
.larrow{color:var(--muted);transition:all .2s;flex-shrink:0}
.link-card:hover .larrow{color:var(--red);transform:translateX(4px)}

footer{margin-top:48px;font-size:12px;color:#444;letter-spacing:1px}
footer span{color:var(--red)}

/* OVERLAY */
.modal-overlay{position:fixed;inset:0;z-index:100;background:rgba(0,0,0,0);pointer-events:none;opacity:0;transition:opacity .3s}
.modal-overlay.open{opacity:1;pointer-events:all;background:rgba(0,0,0,0.85)}

/* MODAL */
.modal{
  position:fixed;bottom:0;left:0;right:0;z-index:101;
  max-height:92vh;overflow-y:auto;
  background:#0f0f0f;
  border-top:2px solid var(--red);
  border-radius:20px 20px 0 0;
  padding:0 0 48px;
  transform:translateY(100%);
  transition:transform .35s cubic-bezier(.4,0,.2,1);
  box-shadow:0 -8px 40px rgba(224,0,0,0.2)
}
.modal.open{transform:translateY(0)}

.modal-handle{width:40px;height:4px;background:#333;border-radius:2px;margin:12px auto 0}
.modal-header{display:flex;align-items:center;gap:12px;padding:16px 20px 10px;border-bottom:1px solid var(--border)}
.modal-back{width:36px;height:36px;border-radius:50%;background:var(--card);border:1px solid var(--border);display:flex;align-items:center;justify-content:center;color:var(--text);cursor:pointer;transition:all .2s;flex-shrink:0}
.modal-back:hover{background:var(--red-dark);border-color:var(--red)}
.modal-back svg{width:18px;height:18px;fill:none;stroke:currentColor;stroke-width:2.5;stroke-linecap:round;stroke-linejoin:round}
.modal-title{font-family:'Bebas Neue',sans-serif;font-size:22px;letter-spacing:2px}
.modal-user{font-size:11px;color:var(--red);letter-spacing:1px}

.modal-hero{text-align:center;padding:24px 20px 16px}
.modal-icon{width:64px;height:64px;border-radius:50%;background:rgba(224,0,0,0.12);border:2px solid var(--red);display:inline-flex;align-items:center;justify-content:center;margin-bottom:12px;box-shadow:0 0 28px var(--red-glow)}
.modal-icon svg{width:32px;height:32px;fill:var(--red)}
.modal-h1{font-family:'Bebas Neue',sans-serif;font-size:28px;letter-spacing:3px;text-shadow:0 0 20px var(--red-glow)}
.modal-p{font-size:12px;color:var(--muted);margin-top:3px}

.mdivider{height:1px;background:linear-gradient(90deg,transparent,var(--red),transparent);opacity:.4;margin:0 20px 20px}

.msec{padding:0 20px;margin-bottom:18px}
.msec-label{font-size:10px;font-weight:700;letter-spacing:2px;color:var(--red);text-transform:uppercase;display:flex;align-items:center;gap:8px;margin-bottom:12px}
.msec-label::after{content:'';flex:1;height:1px;background:var(--border)}

.cfg-card{background:var(--card);border:1px solid var(--border);border-radius:12px;padding:14px 16px;margin-bottom:10px}
.cfg-row{display:flex;justify-content:space-between;align-items:center;margin-bottom:10px}
.cfg-name{font-size:13px;font-weight:600}
.cfg-val{font-family:'Bebas Neue',sans-serif;font-size:22px;color:var(--red);line-height:1}
.slider-track{width:100%;height:6px;background:#2a2a2a;border-radius:3px;position:relative}
.slider-fill{height:100%;border-radius:3px;background:linear-gradient(90deg,var(--red-dark),var(--red));position:relative}
.slider-thumb{width:14px;height:14px;border-radius:50%;background:var(--red);box-shadow:0 0 8px var(--red-glow);position:absolute;right:-7px;top:50%;transform:translateY(-50%)}

.badge-row{background:var(--card);border:1px solid var(--border);border-radius:12px;padding:13px 16px;margin-bottom:10px;display:flex;justify-content:space-between;align-items:center}
.badge-name{font-size:13px;font-weight:600}
.badge{display:inline-block;border-radius:6px;font-size:10px;font-weight:700;padding:3px 10px;letter-spacing:1px}
.b-red{background:rgba(224,0,0,0.15);border:1px solid rgba(224,0,0,0.3);color:var(--red)}
.b-green{background:rgba(0,200,80,0.12);border:1px solid rgba(0,200,80,0.3);color:#00c850}
.b-yellow{background:rgba(255,180,0,0.12);border:1px solid rgba(255,180,0,0.3);color:#ffb400}

.dpi-grid{display:grid;grid-template-columns:1fr 1fr;gap:10px;margin-bottom:10px}
.dpi-card{background:var(--card);border:1px solid var(--border);border-radius:12px;padding:16px;text-align:center}
.dpi-val{font-family:'Bebas Neue',sans-serif;font-size:30px;color:var(--red);text-shadow:0 0 16px var(--red-glow);line-height:1}
.dpi-label{font-size:11px;color:var(--muted);margin-top:4px}

.tip{background:rgba(224,0,0,0.08);border:1px solid rgba(224,0,0,0.25);border-radius:10px;padding:12px 14px;font-size:12px;color:var(--muted);line-height:1.6}
.tip strong{color:var(--red)}
</style>
</head>
<body>

<div class="container">

  <div class="avatar-ring"><div class="avatar-inner">N7</div></div>
  <h1 class="username">newenzo7</h1>
  <p class="tagline">Free Fire • Gaming • Contenido</p>

  <div class="socials">
    <a href="https://www.instagram.com/newenzo7_" target="_blank" rel="noopener" class="social-btn" title="Instagram">
      <svg viewBox="0 0 24 24"><path d="M12 2.163c3.204 0 3.584.012 4.85.07 3.252.148 4.771 1.691 4.919 4.919.058 1.265.069 1.645.069 4.849 0 3.205-.012 3.584-.069 4.849-.149 3.225-1.664 4.771-4.919 4.919-1.266.058-1.644.07-4.85.07-3.204 0-3.584-.012-4.849-.07-3.26-.149-4.771-1.699-4.919-4.92-.058-1.265-.07-1.644-.07-4.849 0-3.204.013-3.583.07-4.849.149-3.227 1.664-4.771 4.919-4.919 1.266-.057 1.645-.069 4.849-.069zm0-2.163c-3.259 0-3.667.014-4.947.072-4.358.2-6.78 2.618-6.98 6.98-.059 1.281-.073 1.689-.073 4.948 0 3.259.014 3.668.072 4.948.2 4.358 2.618 6.78 6.98 6.98 1.281.058 1.689.072 4.948.072 3.259 0 3.668-.014 4.948-.072 4.354-.2 6.782-2.618 6.979-6.98.059-1.28.073-1.689.073-4.948 0-3.259-.014-3.667-.072-4.947-.196-4.354-2.617-6.78-6.979-6.98-1.281-.059-1.69-.073-4.949-.073zm0 5.838c-3.403 0-6.162 2.759-6.162 6.162s2.759 6.163 6.162 6.163 6.162-2.759 6.162-6.163c0-3.403-2.759-6.162-6.162-6.162zm0 10.162c-2.209 0-4-1.79-4-4 0-2.209 1.791-4 4-4s4 1.791 4 4c0 2.21-1.791 4-4 4zm6.406-11.845c-.796 0-1.441.645-1.441 1.44s.645 1.44 1.441 1.44c.795 0 1.439-.645 1.439-1.44s-.644-1.44-1.439-1.44z"/></svg>
    </a>
    <a href="https://www.youtube.com/@newenzo7" target="_blank" rel="noopener" class="social-btn" title="YouTube">
      <svg viewBox="0 0 24 24"><path d="M23.498 6.186a3.016 3.016 0 0 0-2.122-2.136C19.505 3.545 12 3.545 12 3.545s-7.505 0-9.377.505A3.017 3.017 0 0 0 .502 6.186C0 8.07 0 12 0 12s0 3.93.502 5.814a3.016 3.016 0 0 0 2.122 2.136c1.871.505 9.376.505 9.376.505s7.505 0 9.377-.505a3.015 3.015 0 0 0 2.122-2.136C24 15.93 24 12 24 12s0-3.93-.502-5.814zM9.545 15.568V8.432L15.818 12l-6.273 3.568z"/></svg>
    </a>
    <a href="https://www.tiktok.com/@newenzo7" target="_blank" rel="noopener" class="social-btn" title="TikTok">
      <svg viewBox="0 0 24 24"><path d="M19.59 6.69a4.83 4.83 0 0 1-3.77-4.25V2h-3.45v13.67a2.89 2.89 0 0 1-2.88 2.5 2.89 2.89 0 0 1-2.89-2.89 2.89 2.89 0 0 1 2.89-2.89c.28 0 .54.04.79.1V9.01a6.33 6.33 0 0 0-.79-.05 6.34 6.34 0 0 0-6.34 6.34 6.34 6.34 0 0 0 6.34 6.34 6.34 6.34 0 0 0 6.33-6.34V8.8a8.18 8.18 0 0 0 4.78 1.52V6.87a4.85 4.85 0 0 1-1.01-.18z"/></svg>
    </a>
  </div>

  <div class="divider"></div>

  <div class="links">

    <div class="sec-label">Redes</div>

    <a href="https://www.tiktok.com/@kg.enz7" target="_blank" rel="noopener" class="link-card">
      <div class="licon"><svg viewBox="0 0 24 24"><path d="M19.59 6.69a4.83 4.83 0 0 1-3.77-4.25V2h-3.45v13.67a2.89 2.89 0 0 1-2.88 2.5 2.89 2.89 0 0 1-2.89-2.89 2.89 2.89 0 0 1 2.89-2.89c.28 0 .54.04.79.1V9.01a6.33 6.33 0 0 0-.79-.05 6.34 6.34 0 0 0-6.34 6.34 6.34 6.34 0 0 0 6.34 6.34 6.34 6.34 0 0 0 6.33-6.34V8.8a8.18 8.18 0 0 0 4.78 1.52V6.87a4.85 4.85 0 0 1-1.01-.18z"/></svg></div>
      <div class="ltxt"><span class="llabel">TikTok Secundario</span><span class="lsub">@kg.enz7</span></div>
      <svg class="larrow" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><path d="M9 18l6-6-6-6"/></svg>
    </a>

    <a href="https://gearup-game-booster-lower-lag.en.softonic.com/android" target="_blank" rel="noopener" class="link-card">
      <div class="licon"><svg viewBox="0 0 24 24"><path d="M17 1H7c-1.1 0-2 .9-2 2v18c0 1.1.9 2 2 2h10c1.1 0 2-.9 2-2V3c0-1.1-.9-2-2-2zm-5 21c-.83 0-1.5-.67-1.5-1.5S11.17 19 12 19s1.5.67 1.5 1.5S12.83 22 12 22zm5-4H7V4h10v14z"/></svg></div>
      <div class="ltxt"><span class="llabel">App de newenzo7 🔴</span><span class="lsub">GearUp Booster — reduce lag y ping</span></div>
      <svg class="larrow" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><path d="M9 18l6-6-6-6"/></svg>
    </a>

    <div class="sec-label" style="margin-top:8px">Configuraciones Free Fire</div>

    <button class="link-card" onclick="openModal('sensibilidad')">
      <div class="licon"><svg viewBox="0 0 24 24"><path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm-1 14H9V8h2v8zm4 0h-2V8h2v8z"/></svg></div>
      <div class="ltxt"><span class="llabel">Sensibilidad</span><span class="lsub">Mira libre · Scopes · Con mira</span></div>
      <svg class="larrow" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><path d="M9 18l6-6-6-6"/></svg>
    </button>

    <button class="link-card" onclick="openModal('controles')">
      <div class="licon"><svg viewBox="0 0 24 24"><path d="M15 7.5V2H9v5.5l3 3 3-3zM7.5 9H2v6h5.5l3-3-3-3zM9 16.5V22h6v-5.5l-3-3-3 3zM16.5 9l-3 3 3 3H22V9h-5.5z"/></svg></div>
      <div class="ltxt"><span class="llabel">Controles</span><span class="lsub">HUD layout · 4 dedos · Tamaños</span></div>
      <svg class="larrow" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><path d="M9 18l6-6-6-6"/></svg>
    </button>

    <button class="link-card" onclick="openModal('disparo')">
      <div class="licon"><svg viewBox="0 0 24 24"><path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm-1 14l-4-4 1.41-1.41L11 13.17l6.59-6.59L19 8l-8 8z"/></svg></div>
      <div class="ltxt"><span class="llabel">Botón de Disparo &amp; DPI</span><span class="lsub">Posición · Tamaño · DPI recomendado</span></div>
      <svg class="larrow" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><path d="M9 18l6-6-6-6"/></svg>
    </button>

  </div>

  <footer>newenzo7 &nbsp;•&nbsp; <span>♥</span> &nbsp;Todos los derechos reservados</footer>
</div>

<!-- OVERLAY -->
<div class="modal-overlay" id="overlay" onclick="closeModal()"></div>

<!-- MODAL: SENSIBILIDAD -->
<div class="modal" id="modal-sensibilidad">
  <div class="modal-handle"></div>
  <div class="modal-header">
    <button class="modal-back" onclick="closeModal()"><svg viewBox="0 0 24 24"><path d="M15 18l-6-6 6-6"/></svg></button>
    <div><div class="modal-title">Sensibilidad</div><div class="modal-user">newenzo7 • Free Fire</div></div>
  </div>
  <div class="modal-hero">
    <div class="modal-icon"><svg viewBox="0 0 24 24"><path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm-1 14H9V8h2v8zm4 0h-2V8h2v8z"/></svg></div>
    <div class="modal-h1">SENSIBILIDAD</div>
    <div class="modal-p">Configuración oficial de newenzo7</div>
  </div>
  <div class="mdivider"></div>

  <div class="msec">
    <div class="msec-label">Mira libre</div>
    <div class="cfg-card">
      <div class="cfg-row"><span class="cfg-name">General</span><span class="cfg-val">100</span></div>
      <div class="slider-track"><div class="slider-fill" style="width:100%"><div class="slider-thumb"></div></div></div>
    </div>
    <div class="cfg-card">
      <div class="cfg-row"><span class="cfg-name">Mira roja</span><span class="cfg-val">85</span></div>
      <div class="slider-track"><div class="slider-fill" style="width:85%"><div class="slider-thumb"></div></div></div>
    </div>
    <div class="cfg-card">
      <div class="cfg-row"><span class="cfg-name">2x Scope</span><span class="cfg-val">78</span></div>
      <div class="slider-track"><div class="slider-fill" style="width:78%"><div class="slider-thumb"></div></div></div>
    </div>
    <div class="cfg-card">
      <div class="cfg-row"><span class="cfg-name">4x Scope</span><span class="cfg-val">65</span></div>
      <div class="slider-track"><div class="slider-fill" style="width:65%"><div class="slider-thumb"></div></div></div>
    </div>
    <div class="cfg-card">
      <div class="cfg-row"><span class="cfg-name">AWM Scope</span><span class="cfg-val">50</span></div>
      <div class="slider-track"><div class="slider-fill" style="width:50%"><div class="slider-thumb"></div></div></div>
    </div>
  </div>

  <div class="msec">
    <div class="msec-label">Con mira activada</div>
    <div class="cfg-card">
      <div class="cfg-row"><span class="cfg-name">General</span><span class="cfg-val">90</span></div>
      <div class="slider-track"><div class="slider-fill" style="width:90%"><div class="slider-thumb"></div></div></div>
    </div>
    <div class="cfg-card">
      <div class="cfg-row"><span class="cfg-name">Mira roja</span><span class="cfg-val">80</span></div>
      <div class="slider-track"><div class="slider-fill" style="width:80%"><div class="slider-thumb"></div></div></div>
    </div>
    <div class="cfg-card">
      <div class="cfg-row"><span class="cfg-name">2x Scope</span><span class="cfg-val">70</span></div>
      <div class="slider-track"><div class="slider-fill" style="width:70%"><div class="slider-thumb"></div></div></div>
    </div>
    <div class="cfg-card">
      <div class="cfg-row"><span class="cfg-name">4x Scope</span><span class="cfg-val">55</span></div>
      <div class="slider-track"><div class="slider-fill" style="width:55%"><div class="slider-thumb"></div></div></div>
    </div>
    <div class="cfg-card">
      <div class="cfg-row"><span class="cfg-name">AWM Scope</span><span class="cfg-val">40</span></div>
      <div class="slider-track"><div class="slider-fill" style="width:40%"><div class="slider-thumb"></div></div></div>
    </div>
  </div>

  <div class="msec">
    <div class="tip">💡 <strong>Tip de newenzo7:</strong> Empieza con estos valores y ajusta ±5 según tu dispositivo. En móviles de gama baja, baja todo un 10%.</div>
  </div>
</div>

<!-- MODAL: CONTROLES -->
<div class="modal" id="modal-controles">
  <div class="modal-handle"></div>
  <div class="modal-header">
    <button class="modal-back" onclick="closeModal()"><svg viewBox="0 0 24 24"><path d="M15 18l-6-6 6-6"/></svg></button>
    <div><div class="modal-title">Controles</div><div class="modal-user">newenzo7 • Free Fire</div></div>
  </div>
  <div class="modal-hero">
    <div class="modal-icon"><svg viewBox="0 0 24 24"><path d="M15 7.5V2H9v5.5l3 3 3-3zM7.5 9H2v6h5.5l3-3-3-3zM9 16.5V22h6v-5.5l-3-3-3 3zM16.5 9l-3 3 3 3H22V9h-5.5z"/></svg></div>
    <div class="modal-h1">CONTROLES</div>
    <div class="modal-p">Layout HUD de newenzo7 • 4 dedos</div>
  </div>
  <div class="mdivider"></div>

  <div class="msec">
    <div class="msec-label">Estilo de juego</div>
    <div class="badge-row"><span class="badge-name">Modo</span><span class="badge b-red">4 DEDOS</span></div>
    <div class="badge-row"><span class="badge-name">Disparo automático</span><span class="badge b-red">OFF</span></div>
    <div class="badge-row"><span class="badge-name">Agacharse automático</span><span class="badge b-green">ON</span></div>
    <div class="badge-row"><span class="badge-name">Saltar automático</span><span class="badge b-red">OFF</span></div>
  </div>

  <div class="msec">
    <div class="msec-label">Tamaño de botones</div>
    <div class="cfg-card">
      <div class="cfg-row"><span class="cfg-name">Disparar</span><span class="cfg-val">85</span></div>
      <div class="slider-track"><div class="slider-fill" style="width:85%"><div class="slider-thumb"></div></div></div>
    </div>
    <div class="cfg-card">
      <div class="cfg-row"><span class="cfg-name">Mira / Apuntar</span><span class="cfg-val">80</span></div>
      <div class="slider-track"><div class="slider-fill" style="width:80%"><div class="slider-thumb"></div></div></div>
    </div>
    <div class="cfg-card">
      <div class="cfg-row"><span class="cfg-name">Joystick</span><span class="cfg-val">75</span></div>
      <div class="slider-track"><div class="slider-fill" style="width:75%"><div class="slider-thumb"></div></div></div>
    </div>
    <div class="cfg-card">
      <div class="cfg-row"><span class="cfg-name">Saltar</span><span class="cfg-val">70</span></div>
      <div class="slider-track"><div class="slider-fill" style="width:70%"><div class="slider-thumb"></div></div></div>
    </div>
    <div class="cfg-card">
      <div class="cfg-row"><span class="cfg-name">Agachar</span><span class="cfg-val">70</span></div>
      <div class="slider-track"><div class="slider-fill" style="width:70%"><div class="slider-thumb"></div></div></div>
    </div>
    <div class="cfg-card">
      <div class="cfg-row"><span class="cfg-name">Recargar</span><span class="cfg-val">65</span></div>
      <div class="slider-track"><div class="slider-fill" style="width:65%"><div class="slider-thumb"></div></div></div>
    </div>
  </div>

  <div class="msec">
    <div class="msec-label">Diagrama HUD</div>
    <div style="background:var(--card);border:1px solid var(--border);border-radius:12px;padding:14px;position:relative;height:160px;overflow:hidden;margin-bottom:10px">
      <div style="position:absolute;inset:0;background:linear-gradient(135deg,#111,#1a0000);border-radius:12px"></div>
      <div style="position:absolute;left:9%;bottom:22%;width:48px;height:48px;border-radius:50%;background:rgba(224,0,0,0.15);border:2px solid rgba(224,0,0,0.5);display:flex;align-items:center;justify-content:center;font-size:9px;color:var(--red);font-weight:700">JOY</div>
      <div style="position:absolute;right:9%;bottom:22%;width:40px;height:40px;border-radius:50%;background:rgba(224,0,0,0.25);border:2px solid var(--red);display:flex;align-items:center;justify-content:center;font-size:16px;box-shadow:0 0 12px var(--red-glow)">🔥</div>
      <div style="position:absolute;right:24%;bottom:36%;width:32px;height:32px;border-radius:50%;background:rgba(224,0,0,0.15);border:1px solid rgba(224,0,0,0.4);display:flex;align-items:center;justify-content:center;font-size:7px;color:var(--red);font-weight:700">MIRA</div>
      <div style="position:absolute;left:40%;bottom:12%;width:28px;height:28px;border-radius:50%;background:rgba(255,255,255,0.05);border:1px solid #333;display:flex;align-items:center;justify-content:center;font-size:11px;color:var(--muted)">↓</div>
      <div style="position:absolute;right:40%;top:14%;width:28px;height:28px;border-radius:50%;background:rgba(255,255,255,0.05);border:1px solid #333;display:flex;align-items:center;justify-content:center;font-size:11px;color:var(--muted)">↑</div>
      <div style="position:absolute;top:8px;left:50%;transform:translateX(-50%);font-size:8px;color:var(--muted);letter-spacing:1px;white-space:nowrap">LAYOUT 4 DEDOS — newenzo7</div>
    </div>
    <div class="tip">💡 <strong>Tip de newenzo7:</strong> Botón de disparo esquina superior derecha, mira a la izquierda. Disparas y te mueves sin cruzar dedos.</div>
  </div>
</div>

<!-- MODAL: DISPARO Y DPI -->
<div class="modal" id="modal-disparo">
  <div class="modal-handle"></div>
  <div class="modal-header">
    <button class="modal-back" onclick="closeModal()"><svg viewBox="0 0 24 24"><path d="M15 18l-6-6 6-6"/></svg></button>
    <div><div class="modal-title">Disparo &amp; DPI</div><div class="modal-user">newenzo7 • Free Fire</div></div>
  </div>
  <div class="modal-hero">
    <div class="modal-icon"><svg viewBox="0 0 24 24"><path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm-1 14l-4-4 1.41-1.41L11 13.17l6.59-6.59L19 8l-8 8z"/></svg></div>
    <div class="modal-h1">DISPARO &amp; DPI</div>
    <div class="modal-p">Configuración de newenzo7 para mayor precisión</div>
  </div>
  <div class="mdivider"></div>

  <div class="msec">
    <div class="msec-label">Botón de disparo</div>
    <div class="badge-row"><span class="badge-name">Posición</span><span class="badge b-red">SUPERIOR DER.</span></div>
    <div class="cfg-card">
      <div class="cfg-row"><span class="cfg-name">Tamaño del botón</span><span class="cfg-val">85</span></div>
      <div class="slider-track"><div class="slider-fill" style="width:85%"><div class="slider-thumb"></div></div></div>
    </div>
    <div class="cfg-card">
      <div class="cfg-row"><span class="cfg-name">Transparencia</span><span class="cfg-val">40</span></div>
      <div class="slider-track"><div class="slider-fill" style="width:40%"><div class="slider-thumb"></div></div></div>
    </div>
    <div class="badge-row"><span class="badge-name">Modo disparo</span><span class="badge b-yellow">SINGLE TAP</span></div>
    <div class="badge-row"><span class="badge-name">Retroceso táctil</span><span class="badge b-red">OFF</span></div>
  </div>

  <div class="msec">
    <div class="msec-label">Posición en pantalla</div>
    <div style="background:var(--card);border:1px solid var(--border);border-radius:12px;padding:14px;position:relative;height:160px;overflow:hidden;margin-bottom:10px">
      <div style="position:absolute;inset:0;background:linear-gradient(135deg,#111,#1a0000);border-radius:12px"></div>
      <div style="position:absolute;left:9%;bottom:22%;width:48px;height:48px;border-radius:50%;background:rgba(224,0,0,0.12);border:2px solid rgba(224,0,0,0.4);display:flex;align-items:center;justify-content:center;font-size:9px;color:var(--muted);font-weight:700">JOY</div>
      <div style="position:absolute;right:6%;top:10%;width:52px;height:52px;border-radius:50%;background:rgba(224,0,0,0.3);border:3px solid var(--red);display:flex;align-items:center;justify-content:center;font-size:20px;box-shadow:0 0 20px var(--red-glow)">🔥</div>
      <div style="position:absolute;right:5%;top:66%;font-size:8px;color:var(--red);font-weight:700;letter-spacing:.5px">DISPARO</div>
      <div style="position:absolute;left:50%;top:8px;transform:translateX(-50%);font-size:8px;color:var(--muted);letter-spacing:1px;white-space:nowrap">ZONA DE DISPARO — newenzo7</div>
    </div>
  </div>

  <div class="msec">
    <div class="msec-label">DPI recomendado</div>
    <div class="dpi-grid">
      <div class="dpi-card"><div class="dpi-val">240</div><div class="dpi-label">DPI mínimo</div></div>
      <div class="dpi-card"><div class="dpi-val">320</div><div class="dpi-label">DPI óptimo</div></div>
      <div class="dpi-card"><div class="dpi-val">400</div><div class="dpi-label">DPI máximo</div></div>
      <div class="dpi-card" style="border-color:var(--red);box-shadow:0 0 12px var(--red-glow)">
        <div class="dpi-val" style="font-size:22px">newenzo7</div>
        <div class="dpi-label" style="color:var(--red)">usa 320 DPI</div>
      </div>
    </div>
    <div class="badge-row"><span class="badge-name">DPI pantalla</span><span class="badge b-red">320</span></div>
    <div class="badge-row"><span class="badge-name">Velocidad puntero</span><span class="badge b-yellow">MEDIA</span></div>
    <div class="badge-row"><span class="badge-name">Toque largo</span><span class="badge b-red">DESACTIVADO</span></div>
  </div>

  <div class="msec">
    <div class="tip">💡 <strong>Tip de newenzo7:</strong> Con 320 DPI tienes el balance ideal entre velocidad y precisión. Sube a 400 si juegas en modo agresivo con 4 dedos.</div>
  </div>
</div>

<script>
  function openModal(id) {
    document.getElementById('overlay').classList.add('open');
    document.getElementById('modal-' + id).classList.add('open');
    document.body.style.overflow = 'hidden';
  }
  function closeModal() {
    document.getElementById('overlay').classList.remove('open');
    document.querySelectorAll('.modal').forEach(m => m.classList.remove('open'));
    document.body.style.overflow = '';
  }
  let startY = 0;
  document.querySelectorAll('.modal').forEach(modal => {
    modal.addEventListener('touchstart', e => { startY = e.touches[0].clientY; }, {passive:true});
    modal.addEventListener('touchend', e => {
      if (e.changedTouches[0].clientY - startY > 80) closeModal();
    }, {passive:true});
  });
  document.addEventListener('keydown', e => { if(e.key==='Escape') closeModal(); });
</script>
</body>
</html>

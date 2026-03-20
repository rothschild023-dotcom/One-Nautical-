<!DOCTYPE html>

<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ONE Nautical Refit — Documento Completo</title>
    <style>
        :root {
            --primary: #d4af37;
            --primary-light: #f4d03f;
            --bg: #0a1628;
            --bg-secondary: #0d1b2a;
            --card: rgba(212, 175, 55, 0.05);
            --card-hover: rgba(212, 175, 55, 0.1);
            --border: rgba(212, 175, 55, 0.3);
            --text: #ffffff;
            --text-muted: #94a3b8;
            --accent: #1e3a5f;
            --danger: #ef4444;
            --success: #22c55e;
        }

```
    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
        font-family: 'Segoe UI', Roboto, Helvetica, Arial, sans-serif;
        background: linear-gradient(135deg, var(--bg) 0%, var(--bg-secondary) 100%);
        color: var(--text);
        line-height: 1.7;
        min-height: 100vh;
    }

    /* ── TAB NAV ── */
    .tab-nav {
        position: sticky;
        top: 0;
        z-index: 999;
        background: rgba(10, 22, 40, 0.97);
        backdrop-filter: blur(12px);
        border-bottom: 2px solid var(--border);
        display: flex;
        align-items: center;
        gap: 0;
        padding: 0 20px;
        overflow-x: auto;
    }

    .tab-nav-logo {
        font-size: 18px;
        font-weight: 900;
        color: var(--primary);
        letter-spacing: 2px;
        text-transform: uppercase;
        white-space: nowrap;
        padding: 16px 20px 16px 0;
        border-right: 1px solid var(--border);
        margin-right: 10px;
        flex-shrink: 0;
    }

    .tab-btn {
        background: transparent;
        border: none;
        color: var(--text-muted);
        padding: 18px 22px;
        font-size: 13px;
        font-weight: 600;
        text-transform: uppercase;
        letter-spacing: 1px;
        cursor: pointer;
        white-space: nowrap;
        border-bottom: 3px solid transparent;
        margin-bottom: -2px;
        transition: all 0.25s ease;
        display: flex;
        align-items: center;
        gap: 8px;
    }

    .tab-btn:hover { color: var(--primary-light); }

    .tab-btn.active {
        color: var(--primary);
        border-bottom-color: var(--primary);
    }

    /* ── PAGES ── */
    .page { display: none; }
    .page.active { display: block; }

    /* ── SHARED STYLES (copied from original docs) ── */

    .doc-wrap {
        max-width: 210mm;
        margin: 0 auto;
        padding: 40px;
    }

    .doc-wrap-wide {
        max-width: 1000px;
        margin: 0 auto;
        padding: 40px 20px;
    }

    /* Header */
    .header {
        text-align: center;
        border-bottom: 3px solid var(--primary);
        padding-bottom: 30px;
        margin-bottom: 35px;
        position: relative;
    }
    .header::after {
        content: "⚓";
        position: absolute;
        bottom: -15px;
        left: 50%;
        transform: translateX(-50%);
        background: var(--bg);
        padding: 0 15px;
        color: var(--primary);
        font-size: 20px;
    }
    .logo-container {
        display: flex;
        align-items: center;
        justify-content: center;
        gap: 15px;
        margin-bottom: 10px;
    }
    .logo-icon {
        width: 60px; height: 60px;
        background: linear-gradient(135deg, var(--primary) 0%, var(--primary-light) 100%);
        border-radius: 50%;
        display: flex; align-items: center; justify-content: center;
        font-size: 30px; color: var(--bg); font-weight: bold;
        border: 3px solid var(--primary);
        box-shadow: 0 0 20px rgba(212,175,55,.3);
    }
    .logo-text { text-align: left; }
    .logo-title {
        font-size: 42px; font-weight: 900; color: var(--primary);
        letter-spacing: 3px; text-transform: uppercase; margin: 0; line-height: 1;
        text-shadow: 0 2px 10px rgba(212,175,55,.3);
    }
    .logo-subtitle {
        font-size: 14px; color: var(--primary-light);
        letter-spacing: 6px; text-transform: uppercase; font-weight: 600; margin-top: 5px;
    }
    .tagline { font-size: 13px; color: var(--text-muted); margin-top: 15px; font-style: italic; letter-spacing: 1px; }

    /* Section titles */
    .section-title {
        font-size: 22px; color: var(--primary);
        margin: 35px 0 20px; font-weight: 700;
        display: flex; align-items: center; gap: 10px;
        border-bottom: 1px solid var(--border); padding-bottom: 10px;
    }
    .section-title.anchor-blue::before { content: "🔹"; font-size: 18px; }
    .section-title.anchor-diamond::before { content: "🔷"; font-size: 18px; }

    /* Cards */
    .card {
        background: var(--card); border: 1px solid var(--border);
        border-radius: 12px; padding: 25px; margin: 20px 0; position: relative;
    }
    .card::before {
        content: ""; position: absolute; top: 0; left: 0;
        width: 4px; height: 100%;
        background: linear-gradient(to bottom, var(--primary), transparent);
        border-radius: 12px 0 0 12px;
    }
    .card-highlight {
        background: linear-gradient(135deg, rgba(212,175,55,.1) 0%, rgba(30,58,95,.3) 100%);
        border: 2px solid var(--primary);
    }
    .card-highlight::after {
        content: "★"; position: absolute; top: -12px; right: 20px;
        background: var(--bg); padding: 0 10px; color: var(--primary); font-size: 16px;
    }

    .intro-text { font-size: 16px; color: var(--text); font-style: italic; text-align: center; line-height: 1.8; }

    /* Lists */
    .feature-list { list-style: none; padding: 0; }
    .feature-list li { display: flex; align-items: flex-start; gap: 12px; margin-bottom: 12px; font-size: 14px; color: var(--text); }
    .feature-list li::before { content: "⚓"; color: var(--primary); font-size: 12px; flex-shrink: 0; margin-top: 4px; }

    .check-list { list-style: none; padding: 0; columns: 2; column-gap: 30px; }
    .check-list li { display: flex; align-items: center; gap: 10px; margin-bottom: 10px; font-size: 14px; color: var(--text); break-inside: avoid; }
    .check-list li::before {
        content: "✓"; color: var(--primary); font-weight: bold; font-size: 14px;
        width: 20px; height: 20px; background: rgba(212,175,55,.1);
        border-radius: 50%; display: flex; align-items: center; justify-content: center; flex-shrink: 0;
    }

    .warning-box { background: rgba(239,68,68,.05); border: 1px solid rgba(239,68,68,.3); border-radius: 10px; padding: 20px; margin: 20px 0; }
    .warning-title { color: #fca5a5; font-weight: 700; margin-bottom: 12px; font-size: 14px; }
    .warning-list { list-style: none; padding: 0; }
    .warning-list li { color: #fca5a5; font-size: 13px; margin-bottom: 8px; display: flex; align-items: center; gap: 8px; }
    .warning-list li::before { content: "✕"; color: #ef4444; font-weight: bold; }

    /* Process flow */
    .process-flow { display: flex; flex-wrap: wrap; gap: 10px; margin: 20px 0; justify-content: center; }
    .process-item { background: rgba(0,0,0,.2); border: 1px solid var(--border); border-radius: 8px; padding: 12px 16px; text-align: center; min-width: 110px; }
    .process-number { display: inline-block; width: 24px; height: 24px; background: var(--primary); color: var(--bg); border-radius: 50%; font-weight: 900; font-size: 12px; line-height: 24px; margin-bottom: 6px; }
    .process-text { font-size: 12px; color: var(--text); font-weight: 600; }

    /* Equipment */
    .equipment-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(130px,1fr)); gap: 12px; margin: 20px 0; }
    .equipment-item { background: rgba(30,58,95,.3); border: 1px solid rgba(255,255,255,.1); border-radius: 8px; padding: 15px; text-align: center; font-size: 12px; color: var(--text); }
    .equipment-icon { font-size: 20px; margin-bottom: 8px; display: block; }

    /* Values row */
    .values-row { display: flex; justify-content: center; gap: 40px; margin: 25px 0; flex-wrap: wrap; }
    .value-item { text-align: center; }
    .value-icon { font-size: 28px; margin-bottom: 8px; }
    .value-text { color: var(--primary); font-weight: 700; font-size: 14px; letter-spacing: 1px; }

    /* Highlight box */
    .highlight-box {
        background: linear-gradient(135deg, rgba(212,175,55,.1) 0%, rgba(30,58,95,.3) 100%);
        border: 2px solid var(--primary); border-radius: 12px; padding: 25px;
        margin: 25px 0; text-align: center; position: relative;
    }
    .highlight-box::before { content: "★"; position: absolute; top: -12px; left: 50%; transform: translateX(-50%); background: var(--bg); padding: 0 15px; color: var(--primary); font-size: 16px; }
    .highlight-text { font-size: 18px; color: var(--text); font-weight: 600; }
    .highlight-sub { font-size: 14px; color: var(--primary); margin-top: 8px; }

    /* Footer */
    .footer { margin-top: 50px; padding-top: 30px; border-top: 2px solid var(--primary); text-align: center; }
    .footer-logo { font-size: 28px; color: var(--primary); font-weight: 900; letter-spacing: 3px; margin-bottom: 10px; }
    .footer-tagline { font-size: 14px; color: var(--text-muted); font-style: italic; margin-bottom: 20px; }
    .contact-info { display: flex; justify-content: center; gap: 40px; margin: 20px 0; flex-wrap: wrap; }
    .contact-item { text-align: center; }
    .contact-label { font-size: 11px; color: var(--primary); text-transform: uppercase; letter-spacing: 1px; margin-bottom: 5px; }
    .contact-value { font-size: 16px; color: var(--text); font-weight: 600; }
    .footer-note { font-size: 11px; color: var(--text-muted); margin-top: 20px; font-style: italic; }

    /* ── BUDGET PAGE SPECIFIC ── */
    [contenteditable="true"] {
        transition: all .3s; padding: 2px 6px; border-radius: 4px; outline: none;
        border-bottom: 1px dashed transparent;
    }
    [contenteditable="true"]:hover { background: rgba(212,175,55,.1); border-bottom: 1px dashed var(--primary); }
    [contenteditable="true"]:focus { background: rgba(212,175,55,.15); border-bottom: 1px solid var(--primary); }

    .client-card {
        display: grid; grid-template-columns: 1fr 1fr 1fr; gap: 25px;
        background: var(--card); border: 1px solid var(--border);
        padding: 25px; border-radius: 12px; margin-bottom: 30px;
        position: relative; overflow: hidden;
    }
    .client-card::before { content: ""; position: absolute; top: 0; left: 0; width: 4px; height: 100%; background: linear-gradient(to bottom, var(--primary), transparent); }

    .label-sm { font-size: 11px; text-transform: uppercase; color: var(--primary); font-weight: 800; display: block; margin-bottom: 8px; letter-spacing: 1px; }

    .size-selector { display: grid; grid-template-columns: repeat(4,1fr); gap: 15px; margin-bottom: 30px; }
    .size-btn { background: var(--card); border: 2px solid var(--border); color: var(--text); padding: 20px; border-radius: 12px; cursor: pointer; transition: all .3s; text-align: center; }
    .size-btn:hover, .size-btn.active { background: rgba(212,175,55,.1); border-color: var(--primary); transform: translateY(-2px); }
    .size-btn.active { background: rgba(212,175,55,.2); box-shadow: 0 0 20px rgba(212,175,55,.2); }
    .size-btn h3 { color: var(--primary); font-size: 18px; margin-bottom: 5px; }
    .size-btn p { font-size: 12px; color: var(--text-muted); }

    .section {
        background: var(--card); border: 1px solid var(--border);
        border-radius: 12px; padding: 30px; margin-bottom: 30px;
        position: relative; transition: transform .3s, box-shadow .3s;
    }
    .section:hover { transform: translateY(-2px); box-shadow: 0 10px 30px rgba(0,0,0,.3); }

    .badge { display: inline-block; background: rgba(212,175,55,.15); color: var(--primary); padding: 6px 16px; border-radius: 50px; font-size: 11px; font-weight: 800; text-transform: uppercase; margin-bottom: 20px; letter-spacing: 1px; border: 1px solid rgba(212,175,55,.3); }
    .badge-secondary { background: rgba(30,58,95,.5); color: var(--text-muted); border-color: rgba(255,255,255,.1); }
    .badge-danger { background: rgba(239,68,68,.15); color: var(--danger); border-color: rgba(239,68,68,.3); }

    .section h2 { margin-top: 0; margin-bottom: 20px; color: var(--text); font-size: 24px; font-weight: 700; }

    .item-row { display: flex; justify-content: space-between; align-items: center; padding: 15px 0; border-bottom: 1px solid var(--border); transition: background .3s; }
    .item-row:hover { background: var(--card-hover); margin: 0 -10px; padding-left: 10px; padding-right: 10px; border-radius: 6px; }
    .item-row:last-child { border-bottom: none; }
    .price-tag { color: var(--primary); font-weight: bold; font-family: 'Courier New', monospace; font-size: 16px; }

    .materials-detail { background: rgba(0,0,0,.3); padding: 15px; border-radius: 8px; margin-top: 10px; font-size: 12px; color: var(--text-muted); display: none; }
    .materials-detail.show { display: block; }
    .materials-detail strong { color: var(--primary-light); }

    .total-container {
        background: linear-gradient(135deg, rgba(212,175,55,.1) 0%, rgba(30,58,95,.3) 100%);
        padding: 35px; border-radius: 15px; text-align: center;
        border: 2px solid var(--primary); position: relative; overflow: hidden;
    }
    .total-container::before {
        content: ""; position: absolute; top: -50%; left: -50%;
        width: 200%; height: 200%;
        background: radial-gradient(circle, rgba(212,175,55,.1) 0%, transparent 70%);
        animation: pulse 4s ease-in-out infinite;
    }
    @keyframes pulse { 0%,100%{transform:scale(1);opacity:.5} 50%{transform:scale(1.1);opacity:.8} }
    .total-label { color: var(--text-muted); font-weight: 600; font-size: 14px; text-transform: uppercase; letter-spacing: 2px; position: relative; z-index: 1; }
    .total-value { font-size: 48px; color: var(--primary); font-weight: 900; display: block; margin: 10px 0; position: relative; z-index: 1; text-shadow: 0 2px 10px rgba(212,175,55,.3); }
    .payment-info { font-size: 13px; color: var(--text-muted); margin-top: 15px; position: relative; z-index: 1; }

    .btn-toggle { background: transparent; border: 1px solid var(--primary); color: var(--primary); padding: 8px 16px; border-radius: 20px; cursor: pointer; font-size: 11px; margin-left: 10px; transition: all .3s; }
    .btn-toggle:hover { background: var(--primary); color: var(--bg); }

    .labor-section { background: rgba(30,58,95,.3); border: 1px solid rgba(255,255,255,.1); padding: 20px; border-radius: 10px; margin-top: 20px; }
    .labor-row { display: flex; justify-content: space-between; padding: 8px 0; font-size: 13px; border-bottom: 1px dashed rgba(255,255,255,.1); }
    .labor-row:last-child { border-bottom: none; font-weight: bold; color: var(--primary); font-size: 15px; margin-top: 10px; padding-top: 10px; border-top: 2px solid var(--primary); }

    .checkbox-wrapper { display: flex; align-items: center; gap: 12px; cursor: pointer; }
    .custom-checkbox { width: 20px; height: 20px; border: 2px solid var(--primary); border-radius: 4px; display: flex; align-items: center; justify-content: center; transition: all .3s; background: transparent; }
    .custom-checkbox.checked { background: var(--primary); }
    .custom-checkbox.checked::after { content: "✓"; color: var(--bg); font-weight: bold; font-size: 14px; }
    input[type="checkbox"] { display: none; }

    /* ── BIOGRAPHY PAGE SPECIFIC ── */
    .profile-header { display: flex; align-items: center; gap: 25px; margin-bottom: 25px; }
    .profile-avatar { width: 100px; height: 100px; background: linear-gradient(135deg, var(--primary) 0%, var(--primary-light) 100%); border-radius: 50%; display: flex; align-items: center; justify-content: center; font-size: 50px; flex-shrink: 0; border: 4px solid var(--primary); box-shadow: 0 0 30px rgba(212,175,55,.3); }
    .profile-info h2 { font-size: 28px; color: var(--primary); margin-bottom: 5px; }
    .profile-info .subtitle { font-size: 16px; color: var(--text-muted); font-style: italic; }

    .brands-grid { display: flex; flex-wrap: wrap; gap: 12px; margin: 20px 0; justify-content: center; }
    .brand-tag { background: rgba(212,175,55,.15); border: 1px solid var(--border); border-radius: 20px; padding: 8px 16px; font-size: 13px; color: var(--primary); font-weight: 600; }

    .skills-list { display: grid; grid-template-columns: repeat(auto-fit, minmax(200px,1fr)); gap: 12px; margin-top: 15px; }
    .skill-item { display: flex; align-items: center; gap: 10px; font-size: 14px; color: var(--text); }
    .skill-item::before { content: "⚓"; color: var(--primary); }

    .pillars-grid { display: grid; grid-template-columns: repeat(3,1fr); gap: 20px; margin: 25px 0; }
    .pillar-item { background: rgba(0,0,0,.2); border: 1px solid var(--border); border-radius: 10px; padding: 20px; text-align: center; }
    .pillar-number { width: 35px; height: 35px; background: var(--primary); color: var(--bg); border-radius: 50%; display: flex; align-items: center; justify-content: center; font-weight: 900; font-size: 16px; margin: 0 auto 12px; }
    .pillar-title { font-size: 13px; color: var(--text); font-weight: 600; line-height: 1.4; }

    .quote-box { border-left: 4px solid var(--primary); padding: 20px 25px; margin: 25px 0; background: rgba(212,175,55,.05); font-style: italic; font-size: 16px; color: var(--text); line-height: 1.8; }
    .quote-author { margin-top: 10px; font-size: 13px; color: var(--primary); font-style: normal; font-weight: 600; }

    .footer-slogan { font-size: 18px; color: var(--text); font-weight: 600; margin-top: 20px; }

    /* ── PRINT BUTTON ── */
    .btn-print {
        position: fixed; bottom: 30px; right: 30px;
        background: linear-gradient(135deg, var(--primary) 0%, var(--primary-light) 100%);
        color: var(--bg); border: none; padding: 15px 25px;
        border-radius: 50px; font-weight: bold; font-size: 13px;
        cursor: pointer; box-shadow: 0 10px 30px rgba(212,175,55,.4);
        z-index: 1000; transition: all .3s; text-transform: uppercase; letter-spacing: 1px;
    }
    .btn-print:hover { transform: translateY(-3px); box-shadow: 0 15px 40px rgba(212,175,55,.5); }

    /* ── RESPONSIVE ── */
    @media (max-width: 768px) {
        .doc-wrap, .doc-wrap-wide { padding: 20px 15px; }
        .logo-title { font-size: 32px; }
        .client-card, .pillars-grid { grid-template-columns: 1fr; }
        .check-list { columns: 1; }
        .size-selector { grid-template-columns: 1fr 1fr; }
        .total-value { font-size: 36px; }
        .profile-header { flex-direction: column; text-align: center; }
        .tab-btn { padding: 14px 14px; font-size: 11px; }
    }

    /* ── PRINT ── */
    @media print {
        .tab-nav, .btn-print { display: none !important; }
        .page { display: block !important; }
        .doc-wrap, .doc-wrap-wide { max-width: 100%; padding: 20px; }
        body { background: #fff; color: #000; }
        .card, .section, .equipment-item, .process-item, .warning-box, .pillar-item, .brand-tag, .quote-box {
            background: #f5f5f5; border: 1px solid #ddd; break-inside: avoid;
        }
        .logo-title, .value-text, .contact-label, .footer-logo, .profile-info h2, .pillar-number, .quote-author, .price-tag, .total-value { color: #b8860b !important; }
        .section-title { color: #b8860b; }
        .total-container { border: 2px solid #b8860b; background: #fff; }
        .warning-list li, .warning-title { color: #991b1b; }
        .materials-detail { display: block !important; background: #f5f5f5; color: #333; }
    }
</style>
```

</head>
<body>

<!-- ══════════════════════════════════════════════
     TAB NAVIGATION
═══════════════════════════════════════════════ -->

<nav class="tab-nav">
    <div class="tab-nav-logo">⚓ ONE</div>
    <button class="tab-btn active" onclick="showTab('apresentacao', this)">📋 Apresentação</button>
    <button class="tab-btn" onclick="showTab('orcamento', this)">💰 Orçamento</button>
    <button class="tab-btn" onclick="showTab('biografia', this)">👤 Biografia</button>
</nav>

<button class="btn-print" onclick="window.print()">📄 Imprimir / PDF</button>

<!-- ══════════════════════════════════════════════
     PAGE 1 — APRESENTAÇÃO
═══════════════════════════════════════════════ -->

<div id="page-apresentacao" class="page active">
<div class="doc-wrap">

```
<div class="header">
    <div class="logo-container">
        <div class="logo-icon">☠</div>
        <div class="logo-text">
            <div class="logo-title">ONE</div>
            <div class="logo-subtitle">Nautical Refit</div>
        </div>
    </div>
    <div class="tagline">Excelência em Restauração e Manutenção Náutica</div>
</div>

<div class="card">
    <p class="intro-text">
        "Nosso objetivo não é apenas executar um serviço, mas entregar uma embarcação 
        estruturalmente segura, esteticamente valorizada e pronta para uso, 
        seguindo um padrão técnico profissional."
    </p>
    <p style="text-align:center;margin-top:15px;font-size:13px;color:var(--text-muted);">
        Transparência e qualidade são os pilares da ONE Nautical Refit
    </p>
</div>

<h2 class="section-title anchor-blue">Como Trabalhamos</h2>
<p style="color:var(--text-muted);font-size:14px;margin-bottom:15px;">Nosso processo segue etapas técnicas fundamentais:</p>

<div class="process-flow">
    <div class="process-item"><div class="process-number">1</div><div class="process-text">Diagnóstico<br>completo</div></div>
    <div class="process-item"><div class="process-number">2</div><div class="process-text">Preparação<br>superfície</div></div>
    <div class="process-item"><div class="process-number">3</div><div class="process-text">Correção<br>estrutural</div></div>
    <div class="process-item"><div class="process-number">4</div><div class="process-text">Execução<br>técnica</div></div>
    <div class="process-item"><div class="process-number">5</div><div class="process-text">Acabamento<br>e lixamento</div></div>
    <div class="process-item"><div class="process-number">6</div><div class="process-text">Montagem<br>ambiente</div></div>
    <div class="process-item"><div class="process-number">7</div><div class="process-text">Aplicação<br>pintura</div></div>
    <div class="process-item"><div class="process-number">8</div><div class="process-text">Finalização<br>e inspeção</div></div>
</div>

<p style="color:var(--text-muted);font-size:13px;text-align:center;margin:15px 0;">Cada etapa é essencial para garantir o resultado final</p>

<div class="card">
    <h3 style="color:var(--primary);margin-bottom:15px;font-size:16px;">Nosso trabalho envolve:</h3>
    <ul class="feature-list">
        <li>Uso correto de materiais (resina, manta, catalisadores, etc.)</li>
        <li>Tempo de cura respeitado</li>
        <li>Reforço estrutural quando necessário</li>
        <li>Técnicas profissionais de execução</li>
        <li>Acabamento alinhado ao padrão da embarcação</li>
    </ul>
</div>

<div class="warning-box">
    <div class="warning-title">⚠️ Isso evita problemas futuros como:</div>
    <ul class="warning-list">
        <li>Trincas recorrentes</li>
        <li>Delaminação</li>
        <li>Infiltração</li>
        <li>Perda de resistência estrutural</li>
    </ul>
</div>

<h2 class="section-title anchor-blue">O Que Será Feito</h2>
<p style="color:var(--text-muted);font-size:14px;margin-bottom:15px;">Resumo do que será realizado nesta embarcação:</p>

<div class="card">
    <ul class="check-list">
        <li>Correção das áreas identificadas</li>
        <li>Preparação completa da superfície</li>
        <li>Execução técnica do serviço</li>
        <li>Acabamento e nivelamento</li>
        <li>Montagem e desmontagem de ambiente para pintura</li>
        <li>Aplicação de pintura (gelcoat, PU, poliéster, verniz e/ou primer)</li>
        <li>Finalização profissional</li>
    </ul>
</div>

<div class="highlight-box">
    <div class="highlight-text">👉 Serviço completo, do início ao fim</div>
    <div class="highlight-sub">sem necessidade de terceiros</div>
</div>

<h2 class="section-title anchor-blue">Padrão de Entrega</h2>
<p style="color:var(--text-muted);font-size:14px;margin-bottom:15px;">A ONE Nautical Refit utiliza equipamentos profissionais para garantir qualidade e produtividade:</p>

<div class="equipment-grid">
    <div class="equipment-item"><span class="equipment-icon">🔧</span>Lixadeiras roto orbitais</div>
    <div class="equipment-item"><span class="equipment-icon">✨</span>Politriz profissional</div>
    <div class="equipment-item"><span class="equipment-icon">⚙️</span>Esmerilhadeiras</div>
    <div class="equipment-item"><span class="equipment-icon">🔩</span>Parafusadeiras</div>
    <div class="equipment-item"><span class="equipment-icon">💨</span>Compressores de ar</div>
    <div class="equipment-item"><span class="equipment-icon">🎨</span>Pistolas de pintura</div>
    <div class="equipment-item"><span class="equipment-icon">🌪️</span>Aspiração industrial</div>
</div>

<p style="color:var(--text-muted);font-size:14px;margin:20px 0;text-align:center;">Seguimos um padrão de trabalho alinhado aos principais estaleiros do mercado</p>

<div class="values-row">
    <div class="value-item"><div class="value-icon">🎯</div><div class="value-text">TÉCNICA</div></div>
    <div class="value-item"><div class="value-icon">📐</div><div class="value-text">PRECISÃO</div></div>
    <div class="value-item"><div class="value-icon">⚓</div><div class="value-text">RESPONSABILIDADE</div></div>
</div>

<p style="text-align:center;font-size:14px;color:var(--text);font-style:italic;margin-top:20px;">
    Nosso objetivo é crescer como uma empresa sólida, entregando serviços de alto nível e construindo confiança com cada cliente.
</p>

<h2 class="section-title anchor-blue">Valor Real do Serviço Executado</h2>
<p style="color:var(--text-muted);font-size:14px;margin-bottom:15px;">Entendemos que o investimento pode gerar comparação. Porém, é importante considerar que serviços com valor inferior geralmente:</p>

<div class="warning-box">
    <ul class="warning-list">
        <li>Não incluem todos os materiais</li>
        <li>Não seguem processos técnicos completos</li>
        <li>Entregam apenas solução estética (não estrutural)</li>
    </ul>
</div>

<div class="highlight-box">
    <p style="color:var(--text-muted);font-size:14px;margin-bottom:10px;">Nosso compromisso é entregar um serviço definitivo, evitando:</p>
    <div class="highlight-text" style="color:var(--primary);">Retrabalho e novos custos futuros</div>
</div>

<h3 style="color:var(--primary);margin:30px 0 15px;font-size:16px;text-align:center;">Ao final do serviço, sua embarcação estará:</h3>

<div class="card">
    <ul class="check-list">
        <li>Estruturalmente segura</li>
        <li>Com acabamento renovado</li>
        <li>Sem necessidade de retrabalho na área executada</li>
        <li>Pronta para uso</li>
        <li>Valorizada</li>
    </ul>
</div>

<p style="text-align:center;margin-top:30px;font-size:18px;color:var(--primary);font-weight:700;">
    Nosso compromisso é com qualidade e confiança.
</p>

<div class="footer">
    <div class="footer-logo">ONE NAUTICAL REFIT</div>
    <div class="footer-tagline">"O Rei dos Mares"</div>
    <div class="contact-info">
        <div class="contact-item"><div class="contact-label">📱 Telefone</div><div class="contact-value">(13) 97403-0334</div></div>
        <div class="contact-item"><div class="contact-label">📍 Localização</div><div class="contact-value">Base Náutica - Guarujá/SP</div></div>
    </div>
    <p style="font-size:13px;color:var(--text-muted);margin-bottom:10px;">Especialistas em Restauração e Manutenção Náutica de Alto Padrão</p>
    <p class="footer-note">Obrigado pela oportunidade de avaliar sua embarcação.</p>
</div>
```

</div><!-- /doc-wrap -->
</div><!-- /page-apresentacao -->

<!-- ══════════════════════════════════════════════
     PAGE 2 — ORÇAMENTO
═══════════════════════════════════════════════ -->

<div id="page-orcamento" class="page">
<div class="doc-wrap-wide">

```
<div class="header">
    <div class="logo-container">
        <div class="logo-icon">☠</div>
        <div class="logo-text">
            <div class="logo-title">ONE</div>
            <div class="logo-subtitle">Nautical Refit</div>
        </div>
    </div>
    <div class="tagline">Excelência em Restauração e Manutenção Náutica</div>
</div>

<div class="client-card">
    <div>
        <span class="label-sm">Cliente</span>
        <div contenteditable="true" style="font-size:1.3rem;font-weight:600;">Nome do Cliente</div>
    </div>
    <div>
        <span class="label-sm">Embarcação</span>
        <div contenteditable="true" style="font-size:1.3rem;font-weight:600;">Modelo da Embarcação</div>
    </div>
    <div>
        <span class="label-sm">Data</span>
        <div id="orcDataHoje" style="font-size:1.3rem;font-weight:600;"></div>
    </div>
</div>

<div class="section">
    <span class="badge">Selecione o Porte da Embarcação</span>
    <h2>Categorias de Tamanho</h2>
    <div class="size-selector">
        <div class="size-btn active" onclick="selectSize('P',event)">
            <h3>PEQUENO</h3><p>até 6 metros</p><p style="font-size:10px;margin-top:5px;">Ex: Lanchas 15-19 pés</p>
        </div>
        <div class="size-btn" onclick="selectSize('M',event)">
            <h3>MÉDIO</h3><p>6 a 10 metros</p><p style="font-size:10px;margin-top:5px;">Ex: Lanchas 20-32 pés</p>
        </div>
        <div class="size-btn" onclick="selectSize('G',event)">
            <h3>GRANDE</h3><p>10 a 15 metros</p><p style="font-size:10px;margin-top:5px;">Ex: Lanchas 33-50 pés</p>
        </div>
        <div class="size-btn" onclick="selectSize('GG',event)">
            <h3>EXTRA</h3><p>acima de 15m</p><p style="font-size:10px;margin-top:5px;">Ex: Iates +50 pés</p>
        </div>
    </div>
</div>

<!-- Laminação -->
<div class="section">
    <span class="badge">Serviços de Laminação</span>
    <h2 contenteditable="true">Laminação Estrutural (Reparos)</h2>
    <p style="color:var(--text-muted);font-size:13px;margin-bottom:20px;">Resina poliéster isoftálica + Manta fibra de vidro 300/450 + Acabamento</p>
    <div class="item-row" data-service="lamination" data-size="P">
        <div><span contenteditable="true">Pequenas Reparações (até 0,5m²)</span><button class="btn-toggle" onclick="toggleMaterials(this)">Ver Materiais</button><div class="materials-detail"><strong>Materiais:</strong> Resina Poliéster 1kg (R$25), Manta 450 2kg (R$62), Catalisador 30ml, Acetona 1L (R$15), Lixa 80/120/220, EPI básico</div></div>
        <span class="price-tag">R$ <span class="calc-trigger service-price" contenteditable="true">850,00</span></span>
    </div>
    <div class="item-row" data-service="lamination" data-size="M">
        <div><span contenteditable="true">Reparos Médios (0,5m² a 2m²)</span><button class="btn-toggle" onclick="toggleMaterials(this)">Ver Materiais</button><div class="materials-detail"><strong>Materiais:</strong> Resina Poliéster 5kg (R$110), Manta 450 5kg (R$145), Manta 300 3kg, Catalisador 100ml, Acetona 5L (R$45), Massa poliéster 1kg (R$35), Lixas diversas, EPI completo</div></div>
        <span class="price-tag">R$ <span class="calc-trigger service-price" contenteditable="true">2.800,00</span></span>
    </div>
    <div class="item-row" data-service="lamination" data-size="G">
        <div><span contenteditable="true">Reparos Extensivos (2m² a 5m²)</span><button class="btn-toggle" onclick="toggleMaterials(this)">Ver Materiais</button><div class="materials-detail"><strong>Materiais:</strong> Resina Poliéster 10kg (R$200), Manta 450 10kg (R$290), Manta 300 5kg, Gel coat 2kg (R$90), Catalisador 250ml, Acetona 10L (R$80), Massa poliéster 3kg (R$85), Lixas, EPI completo + Bota</div></div>
        <span class="price-tag">R$ <span class="calc-trigger service-price" contenteditable="true">6.500,00</span></span>
    </div>
    <div class="item-row" data-service="lamination" data-size="GG">
        <div><span contenteditable="true">Grandes Reparos Estruturais (+5m²)</span><button class="btn-toggle" onclick="toggleMaterials(this)">Ver Materiais</button><div class="materials-detail"><strong>Materiais:</strong> Resina Poliéster 20kg (R$380), Mantas 450 20kg (R$550), Mantas 300 10kg, Gel coat 5kg (R$200), Catalisador 500ml, Acetona 20L (R$140), Massa poliéster 5kg (R$130), Fitilho 2kg (R$30), Lixas, EPI completo + Bota + Cinta de segurança</div></div>
        <span class="price-tag">R$ <span class="calc-trigger service-price" contenteditable="true">14.000,00</span></span>
    </div>
    <div class="labor-section">
        <span class="label-sm">Composição de Mão de Obra - Laminação</span>
        <div class="labor-row"><span>Profissional Especializado (R$ 350,00/dia)</span><span id="lam-prof">2 dias = R$ 700,00</span></div>
        <div class="labor-row"><span>Ajudante (R$ 120,00/dia)</span><span id="lam-ajud">2 dias = R$ 240,00</span></div>
        <div class="labor-row"><span>Total Mão de Obra</span><span id="lam-total-mo">R$ 940,00</span></div>
    </div>
</div>

<!-- Pintura -->
<div class="section">
    <span class="badge badge-secondary">Pintura e Acabamento</span>
    <h2 contenteditable="true">Pintura Completa (Gel Coat / PU / Poliéster)</h2>
    <p style="color:var(--text-muted);font-size:13px;margin-bottom:20px;">Inclui: Estruturação com andaimes (aluguel), empapelamento completo, proteção de vidros</p>
    <div class="item-row" data-service="paint" data-size="P">
        <div><span contenteditable="true">Pintura Pequena (até 6m) - Gel Coat</span><button class="btn-toggle" onclick="toggleMaterials(this)">Ver Materiais</button><div class="materials-detail"><strong>Preparação:</strong> Andaime simples 3 dias (R$180), Empapelamento (R$80), Plástico azul vidros (R$40), Fitilho 1kg (R$15)<br><strong>Pintura:</strong> Gel coat 4kg (R$180), Catalisador 60ml, Thinner acrílico 18L (R$260), Massa poliéster 2kg (R$55), Lixa 320/400/600, Verniz UV 3,6L (R$420)</div></div>
        <span class="price-tag">R$ <span class="calc-trigger service-price" contenteditable="true">4.200,00</span></span>
    </div>
    <div class="item-row" data-service="paint" data-size="M">
        <div><span contenteditable="true">Pintura Média (6-10m) - PU ou Poliéster</span><button class="btn-toggle" onclick="toggleMaterials(this)">Ver Materiais</button><div class="materials-detail"><strong>Preparação:</strong> Andaime estruturado 5 dias (R$400), Empapelamento completo (R$200), Plástico azul vidros (R$80), Fitilho 2kg (R$30), Fita crepe 10 rolos (R$50)<br><strong>Pintura:</strong> Tinta PU/Poliéster 18L (R$1.200), Catalisador 300ml, Thinner PU 18L (R$320), Massa poliéster 4kg (R$100), Primer 5L (R$280), Lixas 320/400/600/800/1200, Verniz PU 7,2L (R$850)</div></div>
        <span class="price-tag">R$ <span class="calc-trigger service-price" contenteditable="true">8.500,00</span></span>
    </div>
    <div class="item-row" data-service="paint" data-size="G">
        <div><span contenteditable="true">Pintura Grande (10-15m) - PU Premium</span><button class="btn-toggle" onclick="toggleMaterials(this)">Ver Materiais</button><div class="materials-detail"><strong>Preparação:</strong> Andaime estruturado 8 dias (R$750), Empapelamento industrial (R$450), Plástico azul 200m² (R$180), Fitilho 4kg (R$55), Fita crepe 20 rolos (R$100)<br><strong>Pintura:</strong> Tinta PU Premium 36L (R$2.400), Catalisador 600ml, Thinner PU 36L (R$600), Massa poliéster 8kg (R$180), Primer 10L (R$520), Verniz PU 14L (R$1.600), Polish 5L (R$180)</div></div>
        <span class="price-tag">R$ <span class="calc-trigger service-price" contenteditable="true">18.000,00</span></span>
    </div>
    <div class="item-row" data-service="paint" data-size="GG">
        <div><span contenteditable="true">Laqueação Completa (+15m) - Alto Brilho</span><button class="btn-toggle" onclick="toggleMaterials(this)">Ver Materiais</button><div class="materials-detail"><strong>Preparação:</strong> Andaime complexo 12 dias (R$1.500), Empapelamento total (R$900), Plástico azul 400m² (R$350), Fitilho 8kg (R$110), Fita crepe 40 rolos (R$200)<br><strong>Pintura:</strong> Sistema PU 72L (R$4.800), Catalisadores 1,2L, Thinner 72L (R$1.100), Massas 15kg (R$320), Primers 20L (R$980), Verniz náutico premium 28L (R$3.200), Polish 10L (R$320)</div></div>
        <span class="price-tag">R$ <span class="calc-trigger service-price" contenteditable="true">38.000,00</span></span>
    </div>
    <div class="labor-section">
        <span class="label-sm">Composição de Mão de Obra - Pintura</span>
        <div class="labor-row"><span>Pintor Profissional Náutico (R$ 350,00/dia)</span><span id="paint-prof">5 dias = R$ 1.750,00</span></div>
        <div class="labor-row"><span>Ajudante Preparador (R$ 120,00/dia)</span><span id="paint-ajud">5 dias = R$ 600,00</span></div>
        <div class="labor-row"><span>Total Mão de Obra</span><span id="paint-total-mo">R$ 2.350,00</span></div>
    </div>
</div>

<!-- Polimento -->
<div class="section">
    <span class="badge">Tratamento de Superfície</span>
    <h2 contenteditable="true">Polimento Técnico e Correção</h2>
    <div class="item-row" data-service="polish" data-size="P"><div><span contenteditable="true">Polimento Técnico Pequeno (até 6m)</span><button class="btn-toggle" onclick="toggleMaterials(this)">Ver Materiais</button><div class="materials-detail"><strong>Materiais:</strong> Polish corte 1L (R$85), Polish lustro 1L (R$75), Boinas de lã/espuma kit (R$120), Microfibras 10un (R$45), Máscara de proteção</div></div><span class="price-tag">R$ <span class="calc-trigger service-price" contenteditable="true">1.800,00</span></span></div>
    <div class="item-row" data-service="polish" data-size="M"><div><span contenteditable="true">Polimento Técnico Médio (6-10m)</span><button class="btn-toggle" onclick="toggleMaterials(this)">Ver Materiais</button><div class="materials-detail"><strong>Materiais:</strong> Polish corte 3L (R$220), Polish lustro 3L (R$180), Polish finalizador 1L (R$95), Boinas kit profissional (R$280), Microfibras 25un (R$95)</div></div><span class="price-tag">R$ <span class="calc-trigger service-price" contenteditable="true">3.500,00</span></span></div>
    <div class="item-row" data-service="polish" data-size="G"><div><span contenteditable="true">Correção Completa Grande (10-15m)</span><button class="btn-toggle" onclick="toggleMaterials(this)">Ver Materiais</button><div class="materials-detail"><strong>Materiais:</strong> Sistema polish completo 8L (R$650), Boinas profissionais kit grande (R$450), Compostos especiais (R$320), Microfibras 50un (R$180)</div></div><span class="price-tag">R$ <span class="calc-trigger service-price" contenteditable="true">7.200,00</span></span></div>
    <div class="item-row" data-service="polish" data-size="GG"><div><span contenteditable="true">Restauração de Brilho Premium (+15m)</span><button class="btn-toggle" onclick="toggleMaterials(this)">Ver Materiais</button><div class="materials-detail"><strong>Materiais:</strong> Linha premium polish 15L (R$1.200), Boinas especiais importadas (R$850), Ceramic coating 200ml (R$450), Microfibras profissionais 100un (R$320)</div></div><span class="price-tag">R$ <span class="calc-trigger service-price" contenteditable="true">15.000,00</span></span></div>
</div>

<!-- Teca -->
<div class="section">
    <span class="badge badge-secondary">Madeiras</span>
    <h2 contenteditable="true">Restauração de Deck em Teca</h2>
    <div class="item-row" data-service="teak" data-size="P"><div><span contenteditable="true">Deck Pequeno (até 10m²)</span><button class="btn-toggle" onclick="toggleMaterials(this)">Ver Materiais</button><div class="materials-detail"><strong>Materiais:</strong> Deck cleaner 5L (R$120), Teca óleo 5L (R$280), Lixas 60/80/120 (R$45), Escovas de aço, Aplicadores, EPI</div></div><span class="price-tag">R$ <span class="calc-trigger service-price" contenteditable="true">2.200,00</span></span></div>
    <div class="item-row" data-service="teak" data-size="M"><div><span contenteditable="true">Deck Médio (10-25m²)</span><button class="btn-toggle" onclick="toggleMaterials(this)">Ver Materiais</button><div class="materials-detail"><strong>Materiais:</strong> Deck cleaner 10L (R$220), Teca óleo 10L (R$520), Selador deck 5L (R$180), Lixas diversas (R$85), Kit restauração completo</div></div><span class="price-tag">R$ <span class="calc-trigger service-price" contenteditable="true">4.800,00</span></span></div>
    <div class="item-row" data-service="teak" data-size="G"><div><span contenteditable="true">Deck Grande (25-50m²)</span><button class="btn-toggle" onclick="toggleMaterials(this)">Ver Materiais</button><div class="materials-detail"><strong>Materiais:</strong> Deck cleaner 20L (R$400), Teca óleo 20L (R$980), Selador 10L (R$320), Reparador de frestas 5kg (R$280), Lixas industriais (R$150)</div></div><span class="price-tag">R$ <span class="calc-trigger service-price" contenteditable="true">9.500,00</span></span></div>
    <div class="item-row" data-service="teak" data-size="GG"><div><span contenteditable="true">Deck Iate (+50m²)</span><button class="btn-toggle" onclick="toggleMaterials(this)">Ver Materiais</button><div class="materials-detail"><strong>Materiais:</strong> Sistema completo restauração 40L (R$1.800), Reparadores especiais 15kg (R$650), Acabamentos premium (R$450), Equipe 3 profissionais 8 dias</div></div><span class="price-tag">R$ <span class="calc-trigger service-price" contenteditable="true">22.000,00</span></span></div>
</div>

<!-- Anti-incrustante -->
<div class="section">
    <span class="badge badge-danger">Proteção Subaquática</span>
    <h2 contenteditable="true">Anti-Incrustante (Fundo Envenenado)</h2>
    <p style="color:var(--text-muted);font-size:13px;margin-bottom:20px;">Preparação: Lixamento completo do casco, limpeza com solvente, aplicação de primer quando necessário</p>
    <div class="item-row" data-service="antifoul" data-size="P"><div><span contenteditable="true">Fundo Pequeno (até 6m)</span><button class="btn-toggle" onclick="toggleMaterials(this)">Ver Materiais</button><div class="materials-detail"><strong>Preparação:</strong> Lixas 36/60/80 (R$65), Acetona 5L (R$45), Rolos/Trincha (R$35)<br><strong>Tinta:</strong> Anti-incrustante 7,2L (R$1.200), Thinner 9L (R$160), Primer epoxy 3,6L (R$380)</div></div><span class="price-tag">R$ <span class="calc-trigger service-price" contenteditable="true">2.800,00</span></span></div>
    <div class="item-row" data-service="antifoul" data-size="M"><div><span contenteditable="true">Fundo Médio (6-10m)</span><button class="btn-toggle" onclick="toggleMaterials(this)">Ver Materiais</button><div class="materials-detail"><strong>Preparação:</strong> Lixas 36/60/80/120 (R$120), Acetona 10L (R$80), Equipamentos aplicação (R$85)<br><strong>Tinta:</strong> Anti-incrustante 14L (R$2.300), Thinner 18L (R$280), Primer epoxy 7,2L (R$720)</div></div><span class="price-tag">R$ <span class="calc-trigger service-price" contenteditable="true">5.500,00</span></span></div>
    <div class="item-row" data-service="antifoul" data-size="G"><div><span contenteditable="true">Fundo Grande (10-15m)</span><button class="btn-toggle" onclick="toggleMaterials(this)">Ver Materiais</button><div class="materials-detail"><strong>Preparação:</strong> Lixamento industrial (R$280), Acetona 20L (R$140), Equipamentos profissionais (R$150)<br><strong>Tinta:</strong> Anti-incrustante premium 28L (R$4.500), Thinner 36L (R$520), Primer epoxy 14L (R$1.350)</div></div><span class="price-tag">R$ <span class="calc-trigger service-price" contenteditable="true">11.000,00</span></span></div>
    <div class="item-row" data-service="antifoul" data-size="GG"><div><span contenteditable="true">Fundo Iate (+15m)</span><button class="btn-toggle" onclick="toggleMaterials(this)">Ver Materiais</button><div class="materials-detail"><strong>Preparação:</strong> Lixamento industrial pesado (R$550), Solventes 40L (R$280), Equipamentos especializados (R$320)<br><strong>Tinta:</strong> Sistema anti-incrustante 56L (R$8.800), Thinner 72L (R$950), Primers 28L (R$2.600)</div></div><span class="price-tag">R$ <span class="calc-trigger service-price" contenteditable="true">24.000,00</span></span></div>
</div>

<!-- Propspeed -->
<div class="section">
    <span class="badge">Performance</span>
    <h2 contenteditable="true">Aplicação Propspeed (Hélice/Eixo)</h2>
    <p style="color:var(--text-muted);font-size:13px;margin-bottom:20px;">Sistema anti-incrustante de silicone para hélices, eixos e estabilizadores. Aumento de performance e redução de consumo.</p>
    <div class="item-row" data-service="propspeed" data-size="P"><div><span contenteditable="true">Kit Small (Hélice até 18")</span><button class="btn-toggle" onclick="toggleMaterials(this)">Ver Materiais</button><div class="materials-detail"><strong>Kit Propspeed:</strong> Fondant etching 500ml, Primer etching 500ml, Propspeed coating 200ml (Kit R$1.800 importado), Solventes limpeza (R$85)</div></div><span class="price-tag">R$ <span class="calc-trigger service-price" contenteditable="true">2.500,00</span></span></div>
    <div class="item-row" data-service="propspeed" data-size="M"><div><span contenteditable="true">Kit Medium (Hélice 18-24")</span><button class="btn-toggle" onclick="toggleMaterials(this)">Ver Materiais</button><div class="materials-detail"><strong>Kit Propspeed:</strong> Fondant 1L, Primer 1L, Coating 500ml (Kit R$3.200), Solventes (R$120)</div></div><span class="price-tag">R$ <span class="calc-trigger service-price" contenteditable="true">4.200,00</span></span></div>
    <div class="item-row" data-service="propspeed" data-size="G"><div><span contenteditable="true">Kit Large (Hélice 24-32" + Eixo)</span><button class="btn-toggle" onclick="toggleMaterials(this)">Ver Materiais</button><div class="materials-detail"><strong>Kit Propspeed:</strong> Fondant 2L, Primer 2L, Coating 1L (Kit R$5.800), Solventes industriais (R$180)</div></div><span class="price-tag">R$ <span class="calc-trigger service-price" contenteditable="true">7.800,00</span></span></div>
    <div class="item-row" data-service="propspeed" data-size="GG"><div><span contenteditable="true">Kit Extra (Twin Props + Eixos)</span><button class="btn-toggle" onclick="toggleMaterials(this)">Ver Materiais</button><div class="materials-detail"><strong>Kit Propspeed:</strong> Fondant 4L, Primer 4L, Coating 2L (Kit R$11.000), Solventes (R$280)</div></div><span class="price-tag">R$ <span class="calc-trigger service-price" contenteditable="true">15.000,00</span></span></div>
</div>

<!-- Adicionais -->
<div class="section">
    <span class="badge badge-secondary">Serviços Adicionais</span>
    <h2>Personalize seu Orçamento</h2>
    <div class="item-row">
        <label class="checkbox-wrapper"><input type="checkbox" class="upgrade-check" onchange="toggleCheckbox(this)"><span class="custom-checkbox" onclick="toggleCheckbox(this)"></span><span contenteditable="true">Retoques e Ajustes Finais (hora técnica)</span></label>
        <span class="price-tag">R$ <span class="calc-trigger upgrade-val" contenteditable="true">180,00</span>/h</span>
    </div>
    <div class="item-row">
        <label class="checkbox-wrapper"><input type="checkbox" class="upgrade-check" onchange="toggleCheckbox(this)"><span class="custom-checkbox" onclick="toggleCheckbox(this)"></span><span contenteditable="true">Deslocamento e Estadia (fora da base)</span></label>
        <span class="price-tag">R$ <span class="calc-trigger upgrade-val" contenteditable="true">450,00</span>/dia</span>
    </div>
    <div class="item-row">
        <label class="checkbox-wrapper"><input type="checkbox" class="upgrade-check" onchange="toggleCheckbox(this)"><span class="custom-checkbox" onclick="toggleCheckbox(this)"></span><span contenteditable="true">Hospedagem Embarcação (área coberta)</span></label>
        <span class="price-tag">R$ <span class="calc-trigger upgrade-val" contenteditable="true">150,00</span>/dia</span>
    </div>
</div>

<div class="total-container">
    <span class="total-label">Investimento Total Estimado</span>
    <span class="total-value">R$ <span id="finalTotal">0,00</span></span>
    <p class="payment-info" contenteditable="true">💳 Pagamento: 50% entrada + 50% na entrega • Parcelamento em até 3x sem juros • Validade: 30 dias</p>
    <p style="font-size:11px;color:var(--text-muted);margin-top:10px;">* Valores calculados com base em embarcação PEQUENA. Selecione o porte acima para recalcular.</p>
</div>

<div class="footer">
    <div style="display:flex;justify-content:center;gap:30px;margin-bottom:15px;flex-wrap:wrap;">
        <div style="display:flex;align-items:center;gap:8px;"><span style="color:var(--primary)">📱</span><span>(13) 97403-0334</span></div>
        <div style="display:flex;align-items:center;gap:8px;"><span style="color:var(--primary)">⚓</span><span>ONE Nautical Refit</span></div>
        <div style="display:flex;align-items:center;gap:8px;"><span style="color:var(--primary)">📍</span><span>Base Náutica - Guarujá/SP</span></div>
    </div>
    <p style="font-size:12px;color:var(--text-muted);">Especialistas em Restauração e Manutenção Náutica de Alto Padrão</p>
    <p style="margin-top:10px;font-size:11px;opacity:.7;color:var(--text-muted);">"O Rei dos Mares"</p>
    <p style="margin-top:15px;font-size:10px;color:var(--text-muted);">Orçamento técnico baseado em custos reais de materiais e mão de obra especializada. Preços sujeitos à variação de acordo com estado da embarcação e complexidade do serviço.</p>
</div>
```

</div><!-- /doc-wrap-wide -->
</div><!-- /page-orcamento -->

<!-- ══════════════════════════════════════════════
     PAGE 3 — BIOGRAFIA
═══════════════════════════════════════════════ -->

<div id="page-biografia" class="page">
<div class="doc-wrap">

```
<div class="header">
    <div class="logo-container">
        <div class="logo-icon">☠</div>
        <div class="logo-text">
            <div class="logo-title">ONE</div>
            <div class="logo-subtitle">Nautical Refit</div>
        </div>
    </div>
    <div class="tagline">Excelência em Restauração e Manutenção Náutica</div>
</div>

<div class="card">
    <div class="profile-header">
        <div class="profile-avatar">👤</div>
        <div class="profile-info">
            <h2>João Victor</h2>
            <div class="subtitle">Conhecido no setor como Victor Vincy</div>
        </div>
    </div>
    <p class="lead-text" style="color:var(--text);font-size:16px;font-weight:500;line-height:1.8;">
        Atuo desde <strong style="color:var(--primary);">2020</strong> no segmento náutico, com experiência prática em reparo estrutural, laminação e acabamento de embarcações em fibra, desenvolvendo ao longo dos anos domínio completo do processo — da base estrutural ao acabamento final.
    </p>
    <p style="color:var(--text-muted);font-size:15px;margin-top:15px;text-align:justify;">
        Minha formação foi construída diretamente no campo, através de vivência em diferentes operações do setor, o que me proporcionou evolução técnica consistente e contato com ambientes de alto nível de exigência.
    </p>
</div>

<h2 class="section-title anchor-diamond">Experiência em Grandes Referências do Mercado</h2>
<p style="text-align:center;margin-bottom:15px;color:var(--text-muted);font-size:15px;">Ao longo dessa trajetória, atuei em projetos ligados a:</p>

<div class="brands-grid">
    <div class="brand-tag">Azimut Yachts</div>
    <div class="brand-tag">Okean Yachts</div>
    <div class="brand-tag">MCP</div>
    <div class="brand-tag">Ferretti Group</div>
    <div class="brand-tag">Intermarine</div>
    <div class="brand-tag">Carbrasmar</div>
</div>

<div class="card">
    <p style="color:var(--text-muted);font-size:15px;text-align:justify;">
        Também atuei ao lado de equipes especializadas como a <strong style="color:var(--primary);">Marboat</strong>, referência na execução de serviços náuticos no litoral paulista, onde consolidei minha base prática em modelagem, preparação, pintura e acabamento técnico.
    </p>
</div>

<h2 class="section-title anchor-diamond">Domínio Técnico Completo</h2>
<p style="color:var(--text-muted);font-size:15px;">Minha experiência abrange todas as etapas do processo:</p>

<div class="skills-list">
    <div class="skill-item">Preparação de superfície</div>
    <div class="skill-item">Laminação estrutural</div>
    <div class="skill-item">Modelagem estrutural</div>
    <div class="skill-item">Pintura náutica</div>
    <div class="skill-item">Lixamento técnico</div>
    <div class="skill-item">Polimento profissional</div>
</div>

<div class="quote-box">
    "Hoje, meu trabalho é guiado por critério técnico, atenção aos detalhes e compromisso com entrega de alto padrão, aplicando na prática todo o conhecimento adquirido ao longo da minha trajetória no setor."
    <div class="quote-author">— João Victor (Victor Vincy)</div>
</div>

<h2 class="section-title anchor-diamond">A ONE Nautical Refit</h2>

<div class="card card-highlight">
    <p style="text-align:center;font-size:16px;color:var(--text);font-weight:500;line-height:1.8;margin:0;">
        A ONE Nautical Refit nasce a partir de uma visão clara construída ao longo dessa trajetória prática no setor.
    </p>
</div>

<p style="color:var(--text-muted);font-size:15px;text-align:justify;margin-top:20px;">
    Durante minha caminhada, identifiquei padrões recorrentes no mercado que vão contra aquilo que considero essencial: <strong style="color:#fca5a5;">falta de compromisso com qualidade</strong>, <strong style="color:#fca5a5;">desvalorização da mão de obra</strong>, <strong style="color:#fca5a5;">execução sem critério técnico</strong> e <strong style="color:#fca5a5;">foco excessivo apenas em custo</strong>.
</p>

<div class="highlight-box">
    <p style="font-size:20px;color:var(--primary);font-weight:700;margin-bottom:10px;">A ONE surge com o objetivo de ser o oposto disso.</p>
    <p style="font-size:15px;color:var(--text);margin:0;">Mais do que executar serviços, a proposta é atuar com um olhar técnico, criterioso e responsável, elevando o padrão de entrega em cada projeto.</p>
</div>

<h3 style="color:var(--primary);margin:30px 0 20px;font-size:16px;text-align:center;">A empresa se baseia em três pilares fundamentais:</h3>

<div class="pillars-grid">
    <div class="pillar-item"><div class="pillar-number">1</div><div class="pillar-title">Qualidade estrutural e acabamento de alto nível</div></div>
    <div class="pillar-item"><div class="pillar-number">2</div><div class="pillar-title">Transparência e responsabilidade profissional</div></div>
    <div class="pillar-item"><div class="pillar-number">3</div><div class="pillar-title">Evolução contínua e domínio técnico</div></div>
</div>

<div class="card" style="margin-top:30px;">
    <p style="text-align:center;font-size:16px;color:var(--text);margin:0;">
        A ideia é simples: <strong style="color:var(--primary);">absorver os pontos fortes das grandes operações do setor e transformar as falhas observadas em diferenciais.</strong>
    </p>
</div>

<div class="footer">
    <div class="footer-logo">ONE NAUTICAL REFIT</div>
    <div class="footer-tagline">"O Rei dos Mares"</div>
    <div class="footer-slogan">
        A ONE Nautical Refit representa não apenas uma empresa,<br>
        mas um <span style="color:var(--primary);">compromisso com um novo padrão</span> dentro do mercado náutico.
    </div>
    <p class="footer-note">Base Náutica - Guarujá/SP • (13) 97403-0334</p>
</div>
```

</div><!-- /doc-wrap -->
</div><!-- /page-biografia -->

<script>
    // ── TAB SWITCHING ──
    function showTab(name, btn) {
        document.querySelectorAll('.page').forEach(p => p.classList.remove('active'));
        document.querySelectorAll('.tab-btn').forEach(b => b.classList.remove('active'));
        document.getElementById('page-' + name).classList.add('active');
        btn.classList.add('active');
        window.scrollTo({ top: 0, behavior: 'smooth' });
    }

    // ── DATE ──
    document.getElementById('orcDataHoje').textContent =
        new Date().toLocaleDateString('pt-BR');

    // ── BUDGET LOGIC ──
    let currentSize = 'P';

    const laborDays = { P:{prof:2,ajud:2}, M:{prof:5,ajud:5}, G:{prof:10,ajud:10}, GG:{prof:20,ajud:20} };

    const basePrices = {
        lamination: { P:850, M:2800, G:6500, GG:14000 },
        paint:      { P:4200, M:8500, G:18000, GG:38000 },
        polish:     { P:1800, M:3500, G:7200, GG:15000 },
        teak:       { P:2200, M:4800, G:9500, GG:22000 },
        antifoul:   { P:2800, M:5500, G:11000, GG:24000 },
        propspeed:  { P:2500, M:4200, G:7800, GG:15000 }
    };

    function selectSize(size, event) {
        currentSize = size;
        document.querySelectorAll('.size-btn').forEach(btn => btn.classList.remove('active'));
        event.target.closest('.size-btn').classList.add('active');
        updatePrices(); updateLabor(); calcularTotal();
    }

    function updatePrices() {
        document.querySelectorAll('.item-row[data-service]').forEach(row => {
            const svc = row.getAttribute('data-service');
            const priceEl = row.querySelector('.service-price');
            if (basePrices[svc] && basePrices[svc][currentSize]) {
                priceEl.innerText = basePrices[svc][currentSize].toLocaleString('pt-BR', { minimumFractionDigits:2, maximumFractionDigits:2 });
            }
        });
    }

    function updateLabor() {
        const d = laborDays[currentSize];
        const pt = d.prof * 350, at = d.ajud * 120;
        const fmt = v => v.toLocaleString('pt-BR', { minimumFractionDigits:2 });
        document.getElementById('lam-prof').innerText   = d.prof + ' dias = R$ ' + fmt(pt);
        document.getElementById('lam-ajud').innerText   = d.ajud + ' dias = R$ ' + fmt(at);
        document.getElementById('lam-total-mo').innerText = 'R$ ' + fmt(pt+at);
        document.getElementById('paint-prof').innerText   = d.prof + ' dias = R$ ' + fmt(pt);
        document.getElementById('paint-ajud').innerText   = d.ajud + ' dias = R$ ' + fmt(at);
        document.getElementById('paint-total-mo').innerText = 'R$ ' + fmt(pt+at);
    }

    function parsePrice(text) {
        return parseFloat(text.replace(/[^\d.,]/g,'').replace('.','').replace(',','.')) || 0;
    }

    function toggleCheckbox(element) {
        const wrapper = element.closest('.checkbox-wrapper');
        const checkbox = wrapper.querySelector('input[type="checkbox"]');
        const customCb = wrapper.querySelector('.custom-checkbox');
        if (element.type !== 'checkbox') checkbox.checked = !checkbox.checked;
        customCb.classList.toggle('checked', checkbox.checked);
        calcularTotal();
    }

    function toggleMaterials(btn) {
        const detail = btn.nextElementSibling;
        detail.classList.toggle('show');
        btn.innerText = detail.classList.contains('show') ? 'Ocultar Materiais' : 'Ver Materiais';
    }

    function calcularTotal() {
        let total = 0;
        document.querySelectorAll('.item-row[data-service]').forEach(row => {
            if (row.getAttribute('data-size') === currentSize) {
                const el = row.querySelector('.service-price');
                if (el) total += parsePrice(el.innerText);
            }
        });
        document.querySelectorAll('.upgrade-check:checked').forEach(cb => {
            const el = cb.closest('.item-row').querySelector('.upgrade-val');
            if (el) total += parsePrice(el.innerText);
        });
        document.getElementById('finalTotal').innerText =
            total.toLocaleString('pt-BR', { minimumFractionDigits:2, maximumFractionDigits:2 });
    }

    document.addEventListener('input', e => {
        if (e.target.classList.contains('calc-trigger')) calcularTotal();
    });
    document.querySelectorAll('.calc-trigger').forEach(el => {
        el.addEventListener('keydown', e => { if (e.key === 'Enter') { e.preventDefault(); el.blur(); } });
    });

    // Init
    updateLabor();
    calcularTotal();
</script>

</body>
</html>

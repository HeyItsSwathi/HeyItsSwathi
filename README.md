<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Swathi Paramesh — Network Engineer</title>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Syne:wght@400;700;800&family=Barlow:wght@400;500&display=swap');

    * { box-sizing: border-box; margin: 0; padding: 0; }

    body {
      background: #e8eef4;
      display: flex;
      justify-content: center;
      align-items: flex-start;
      min-height: 100vh;
      padding: 40px 16px;
    }

    .card {
      width: 100%;
      max-width: 720px;
      border-radius: 14px;
      overflow: hidden;
      box-shadow: 0 8px 40px rgba(5, 17, 31, 0.18);
    }

    /* ── HEADER ── */
    .header {
      background: #05111f;
      padding: 40px 36px 36px;
      text-align: center;
    }
    .header h1 {
      font-family: 'Syne', sans-serif;
      font-size: 34px;
      font-weight: 800;
      color: #ffffff;
      letter-spacing: -0.5px;
    }
    .header .subtitle {
      font-family: 'Syne', sans-serif;
      font-size: 12px;
      font-weight: 400;
      color: #5b9ec9;
      letter-spacing: 2.5px;
      text-transform: uppercase;
      margin-top: 8px;
    }
    .header .location-pill {
      display: inline-flex;
      align-items: center;
      gap: 5px;
      background: rgba(56, 182, 232, 0.12);
      border: 1px solid rgba(56, 182, 232, 0.3);
      color: #7dd4f0;
      font-family: 'Barlow', sans-serif;
      font-size: 12px;
      padding: 4px 14px;
      border-radius: 20px;
      margin-top: 14px;
    }

    /* ── BODY ── */
    .body {
      background: #ffffff;
      padding: 30px 36px 36px;
      font-family: 'Barlow', sans-serif;
      color: #1a2a38;
    }

    .divider {
      border: none;
      border-top: 1px solid #e8eef4;
      margin: 22px 0;
    }

    .section-title {
      font-family: 'Syne', sans-serif;
      font-size: 11px;
      font-weight: 700;
      letter-spacing: 2px;
      text-transform: uppercase;
      color: #0a6ea0;
      margin-bottom: 14px;
      padding-bottom: 6px;
      border-bottom: 2px solid #e0f0fa;
    }

    .about-text {
      font-size: 14px;
      color: #334e62;
      line-height: 1.8;
    }
    .about-text strong { color: #05111f; }

    .bullet-list { list-style: none; padding: 0; margin-top: 12px; }
    .bullet-list li {
      font-size: 13.5px;
      color: #4a6a80;
      padding: 3px 0 3px 18px;
      position: relative;
    }
    .bullet-list li::before {
      content: '›';
      position: absolute;
      left: 0;
      color: #1a8cc0;
      font-weight: 700;
      font-size: 16px;
      line-height: 1.4;
    }

    .badge-group { margin-bottom: 16px; }
    .badge-group-label {
      font-family: 'Syne', sans-serif;
      font-size: 10.5px;
      font-weight: 700;
      letter-spacing: 1.5px;
      text-transform: uppercase;
      color: #7a9ab0;
      margin-bottom: 8px;
    }
    .badge-row { display: flex; flex-wrap: wrap; gap: 6px; }

    .badge {
      display: inline-flex;
      align-items: center;
      gap: 5px;
      padding: 5px 13px;
      border-radius: 6px;
      font-family: 'Barlow', sans-serif;
      font-size: 12.5px;
      font-weight: 500;
      border: 1px solid transparent;
      white-space: nowrap;
    }

    .b-blue   { background: #e6f4fb; color: #0d5e8a; border-color: #b8ddf0; }
    .b-red    { background: #fdecea; color: #8c2020; border-color: #f5b8b8; }
    .b-navy   { background: #e8f0f8; color: #0c3a6e; border-color: #b0ccec; }
    .b-amber  { background: #fdf4e6; color: #8a4f0a; border-color: #f0d09a; }
    .b-green  { background: #eaf6ee; color: #1a6e36; border-color: #a8dbb8; }
    .b-python { background: #e8f0fa; color: #1a4a8a; border-color: #a8c4e8; }
    .b-azure  { background: #e6eef8; color: #0a3a78; border-color: #a0bce0; }
    .b-cert   { background: #05111f; color: #a0d4f5; border-color: #1a3a58; }

    .social-row { display: flex; flex-wrap: wrap; gap: 10px; margin-top: 4px; }
    .social-btn {
      display: inline-flex;
      align-items: center;
      gap: 8px;
      padding: 8px 18px;
      border-radius: 8px;
      font-family: 'Barlow', sans-serif;
      font-size: 13px;
      font-weight: 500;
      text-decoration: none;
      border: 1px solid transparent;
      transition: opacity 0.15s;
    }
    .social-btn:hover { opacity: 0.75; }
    .s-linkedin  { background: #e8f2fb; color: #0a5a9a; border-color: #a8ccec; }
    .s-instagram { background: #fce8f0; color: #8a1a48; border-color: #f0a8c8; }
    .s-facebook  { background: #e8eef8; color: #0a2e78; border-color: #a8baec; }
  </style>
</head>
<body>
  <div class="card">

    <!-- HEADER -->
    <div class="header">
      <h1>Swathi Paramesh</h1>
      <div class="subtitle">L2 Network Engineer &nbsp;·&nbsp; Enterprise &amp; Hybrid Infrastructure &nbsp;·&nbsp; Network Automation</div>
      <div class="location-pill">📍 Bengaluru, India</div>
    </div>

    <!-- BODY -->
    <div class="body">

      <h2 class="section-title">About Me</h2>
      <p class="about-text">
        Network Engineer with <strong>5+ years</strong> of experience in enterprise and hybrid infrastructure, specializing in <strong>SD-WAN</strong>, routing &amp; switching, network migrations, and automation. I work with technologies like Cisco Catalyst SD-WAN, Meraki, Cisco 9K series, and network monitoring platforms to build reliable and scalable networks.
      </p>
      <ul class="bullet-list">
        <li>Automating repetitive tasks with <strong>Python</strong>, CAC and Hive</li>
        <li>Currently exploring deeper into <strong>network automation</strong> and cloud networking</li>
        <li>Solving complex network problems and building scalable infrastructure</li>
      </ul>

      <hr class="divider" />

      <h2 class="section-title">🛠 Tech Stack</h2>

      <div class="badge-group">
        <div class="badge-group-label">SD-WAN</div>
        <div class="badge-row">
          <span class="badge b-blue">Cisco Catalyst SD-WAN</span>
          <span class="badge b-blue">vManage</span>
          <span class="badge b-blue">Zero-Touch Provisioning</span>
        </div>
      </div>

      <div class="badge-group">
        <div class="badge-group-label">Routing &amp; Switching</div>
        <div class="badge-row">
          <span class="badge b-red">BGP</span>
          <span class="badge b-red">OSPF</span>
          <span class="badge b-red">VLAN</span>
          <span class="badge b-red">STP L2/L3</span>
        </div>
      </div>

      <div class="badge-group">
        <div class="badge-group-label">Cisco Platforms</div>
        <div class="badge-row">
          <span class="badge b-navy">Cisco Catalyst 9K</span>
          <span class="badge b-green">Meraki MS/MR</span>
          <span class="badge b-navy">Cisco WLC</span>
          <span class="badge b-navy">Cisco PnP</span>
        </div>
      </div>

      <div class="badge-group">
        <div class="badge-group-label">Monitoring &amp; Management</div>
        <div class="badge-row">
          <span class="badge b-amber">Catalyst Center (DNAC)</span>
          <span class="badge b-amber">SolarWinds</span>
          <span class="badge b-amber">Infoblox DNS/IPAM</span>
          <span class="badge b-green">ServiceNow</span>
        </div>
      </div>

      <div class="badge-group">
        <div class="badge-group-label">Automation &amp; Cloud</div>
        <div class="badge-row">
          <span class="badge b-python">🐍 Python</span>
          <span class="badge b-azure">☁ Microsoft Azure AZ-900</span>
        </div>
      </div>

      <hr class="divider" />

      <h2 class="section-title">📜 Certifications</h2>
      <div class="badge-row">
        <span class="badge b-cert" style="font-size:13px; padding:7px 16px;">🏅 CCNA — Cisco</span>
        <span class="badge b-cert" style="font-size:13px; padding:7px 16px;">☁ AZ-900 — Microsoft Azure</span>
      </div>

      <hr class="divider" />

      <h2 class="section-title">🔗 Connect With Me</h2>
      <div class="social-row">
        <a class="social-btn s-linkedin" href="https://www.linkedin.com/in/swathiparamesh" target="_blank">
          <svg width="15" height="15" viewBox="0 0 24 24" fill="currentColor"><path d="M20.447 20.452h-3.554v-5.569c0-1.328-.027-3.037-1.852-3.037-1.853 0-2.136 1.445-2.136 2.939v5.667H9.351V9h3.414v1.561h.046c.477-.9 1.637-1.85 3.37-1.85 3.601 0 4.267 2.37 4.267 5.455v6.286zM5.337 7.433a2.062 2.062 0 01-2.063-2.065 2.064 2.064 0 112.063 2.065zm1.782 13.019H3.555V9h3.564v11.452zM22.225 0H1.771C.792 0 0 .774 0 1.729v20.542C0 23.227.792 24 1.771 24h20.451C23.2 24 24 23.227 24 22.271V1.729C24 .774 23.2 0 22.222 0h.003z"/></svg>
          LinkedIn
        </a>
        <a class="social-btn s-instagram" href="https://www.instagram.com/swathi__paramesh?igsh=MXFjYnd5OXpidWdueQ==" target="_blank">
          <svg width="15" height="15" viewBox="0 0 24 24" fill="currentColor"><path d="M12 2.163c3.204 0 3.584.012 4.85.07 3.252.148 4.771 1.691 4.919 4.919.058 1.265.069 1.645.069 4.849 0 3.205-.012 3.584-.069 4.849-.149 3.225-1.664 4.771-4.919 4.919-1.266.058-1.644.07-4.85.07-3.204 0-3.584-.012-4.849-.07-3.26-.149-4.771-1.699-4.919-4.92-.058-1.265-.07-1.644-.07-4.849 0-3.204.013-3.583.07-4.849.149-3.227 1.664-4.771 4.919-4.919 1.266-.057 1.645-.069 4.849-.069zm0-2.163c-3.259 0-3.667.014-4.947.072-4.358.2-6.78 2.618-6.98 6.98-.059 1.281-.073 1.689-.073 4.948 0 3.259.014 3.668.072 4.948.2 4.358 2.618 6.78 6.98 6.98 1.281.058 1.689.072 4.948.072 3.259 0 3.668-.014 4.948-.072 4.354-.2 6.782-2.618 6.979-6.98.059-1.28.073-1.689.073-4.948 0-3.259-.014-3.667-.072-4.947-.196-4.354-2.617-6.78-6.979-6.98-1.281-.059-1.69-.073-4.949-.073zm0 5.838a6.162 6.162 0 100 12.324 6.162 6.162 0 000-12.324zM12 16a4 4 0 110-8 4 4 0 010 8zm6.406-11.845a1.44 1.44 0 100 2.881 1.44 1.44 0 000-2.881z"/></svg>
          Instagram
        </a>
        <a class="social-btn s-facebook" href="#" target="_blank">
          <svg width="15" height="15" viewBox="0 0 24 24" fill="currentColor"><path d="M24 12.073c0-6.627-5.373-12-12-12s-12 5.373-12 12c0 5.99 4.388 10.954 10.125 11.854v-8.385H7.078v-3.47h3.047V9.43c0-3.007 1.792-4.669 4.533-4.669 1.312 0 2.686.235 2.686.235v2.953H15.83c-1.491 0-1.956.925-1.956 1.874v2.25h3.328l-.532 3.47h-2.796v8.385C19.612 23.027 24 18.062 24 12.073z"/></svg>
          Facebook
        </a>
      </div>

    </div>
  </div>
</body>
</html>

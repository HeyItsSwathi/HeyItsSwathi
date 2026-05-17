<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width,initial-scale=1.0"/>
<title>Swathi Paramesh – Network Engineer</title>
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@600;700&family=Inter:wght@300;400;500;600&display=swap" rel="stylesheet"/>
<style>
*,*::before,*::after{box-sizing:border-box;margin:0;padding:0}
:root{
  --midnight:#0B1D3A;
  --navy:#102244;
  --blue:#1D4ED8;
  --blue-light:#3B82F6;
  --teal:#0D9488;
  --white:#FFFFFF;
  --off:#F7F9FF;
  --surface:#EEF3FD;
  --border:#CBD9F2;
  --text:#0B1D3A;
  --body:#2E426B;
  --muted:#6B82A8;
  --display:'Playfair Display',serif;
  --ui:'Inter',sans-serif;
}
html{scroll-behavior:smooth}
body{background:var(--white);color:var(--text);font-family:var(--ui);overflow-x:hidden}

/* ── HERO ── */
.hero{
  background:var(--midnight);
  padding:3.5rem 0 0;
  position:relative;overflow:hidden;
}
.hero::before{
  content:'';position:absolute;inset:0;
  background:
    radial-gradient(ellipse at 15% 50%,rgba(29,78,216,0.18) 0%,transparent 55%),
    radial-gradient(ellipse at 85% 20%,rgba(13,148,136,0.12) 0%,transparent 45%);
}
/* subtle dot grid */
.hero::after{
  content:'';position:absolute;inset:0;
  background-image:radial-gradient(rgba(255,255,255,0.04) 1px,transparent 1px);
  background-size:28px 28px;
}

.container{max-width:860px;margin:0 auto;padding:0 2.5rem}

.hero-inner{
  position:relative;z-index:1;
  display:flex;align-items:flex-end;gap:2.2rem;
  padding-bottom:3rem;
}

/* avatar */
.av-wrap{flex-shrink:0;position:relative}
.av{
  width:100px;height:100px;border-radius:50%;
  background:linear-gradient(145deg,#1D4ED8,#0D9488);
  display:flex;align-items:center;justify-content:center;
  font-family:var(--display);font-size:1.9rem;font-weight:700;color:#fff;
  box-shadow:0 0 0 3px rgba(255,255,255,0.1),0 0 40px rgba(29,78,216,0.35);
  animation:gentle-float 5s ease-in-out infinite;
}
@keyframes gentle-float{0%,100%{transform:translateY(0)}50%{transform:translateY(-6px)}}
.av-ring{
  position:absolute;inset:-7px;border-radius:50%;
  border:1.5px solid rgba(59,130,246,0.3);
  animation:slow-spin 15s linear infinite;
}
@keyframes slow-spin{to{transform:rotate(360deg)}}
.online-dot{
  position:absolute;bottom:4px;right:4px;
  width:16px;height:16px;border-radius:50%;
  background:var(--teal);border:3px solid var(--midnight);
}

/* hero text */
.hero-meta{font-size:.72rem;letter-spacing:3px;text-transform:uppercase;color:rgba(13,148,136,0.9);margin-bottom:.5rem}
.hero-name{font-family:var(--display);font-size:clamp(1.9rem,4vw,2.8rem);color:#fff;line-height:1.1;font-weight:700}
.hero-role{font-size:.92rem;color:rgba(255,255,255,0.45);margin-top:.35rem;font-weight:300;letter-spacing:.3px}
.hero-tags{display:flex;flex-wrap:wrap;gap:7px;margin-top:1rem}
.htag{
  font-size:.7rem;letter-spacing:.4px;
  padding:.28rem .75rem;border-radius:20px;
  border:1px solid rgba(59,130,246,0.3);
  color:rgba(59,130,246,0.85);
  background:rgba(29,78,216,0.1);
}
.htag.t{border-color:rgba(13,148,136,0.3);color:rgba(13,148,136,0.85);background:rgba(13,148,136,0.1)}

/* load anims */
.hero-inner>*{animation:rise .6s ease both}
.hero-inner>*:nth-child(1){animation-delay:.1s}
.hero-inner>*:nth-child(2){animation-delay:.2s}
@keyframes rise{from{opacity:0;transform:translateY(14px)}to{opacity:1;transform:translateY(0)}}

/* white wave divider */
.wave{
  display:block;width:100%;height:50px;
  background:var(--white);
  clip-path:ellipse(55% 100% at 50% 100%);
  margin-top:-1px;
}

/* ── BODY ── */
.page{padding:2.5rem 0 5rem}
.sec{margin-bottom:2.8rem;opacity:0;animation:rise .55s ease both}
.sec:nth-child(1){animation-delay:.25s}
.sec:nth-child(2){animation-delay:.35s}
.sec:nth-child(3){animation-delay:.45s}
.sec:nth-child(4){animation-delay:.55s}
.sec:nth-child(5){animation-delay:.65s}

.sec-head{
  display:flex;align-items:center;gap:.8rem;
  margin-bottom:1.2rem;
}
.sec-title{font-family:var(--display);font-size:1.15rem;font-weight:600;color:var(--midnight)}
.sec-line{flex:1;height:1px;background:linear-gradient(90deg,var(--border),transparent)}

/* about */
.about-p{font-size:.95rem;line-height:1.9;color:var(--body)}
.about-p strong{color:var(--midnight);font-weight:600}

.kv-row{display:flex;flex-wrap:wrap;gap:10px;margin-top:1.2rem}
.kv{
  background:var(--off);border:1px solid var(--border);
  border-radius:10px;padding:.7rem 1.1rem;
  display:flex;flex-direction:column;gap:.15rem;
  transition:border-color .2s,transform .2s;
}
.kv:hover{border-color:var(--blue);transform:translateY(-2px)}
.kv-v{font-family:var(--display);font-size:1.25rem;font-weight:600;color:var(--blue)}
.kv-l{font-size:.7rem;color:var(--muted);letter-spacing:.3px}

/* tech stack */
.chips{display:flex;flex-wrap:wrap;gap:9px}
.chip{
  font-size:.78rem;padding:.48rem 1.05rem;
  border-radius:7px;
  border:1.5px solid var(--border);
  background:var(--white);
  color:var(--navy);
  cursor:pointer;
  font-weight:500;
  position:relative;overflow:hidden;
  transition:border-color .2s,color .2s;
  outline:none;
}
.chip::after{
  content:'';position:absolute;inset:0;
  background:var(--midnight);
  transform:translateY(100%);
  transition:transform .22s cubic-bezier(.4,0,.2,1);
  z-index:0;
}
.chip span{position:relative;z-index:1}
.chip:hover{border-color:var(--midnight);color:var(--white)}
.chip:hover::after{transform:translateY(0)}
.chip.on{background:var(--midnight);color:var(--white);border-color:var(--midnight)}
.chip.on::after{transform:translateY(0)}

/* ripple */
.rpl{
  position:absolute;border-radius:50%;
  background:rgba(255,255,255,0.25);
  transform:scale(0);animation:rpl .5s linear;
  pointer-events:none;z-index:2;
}
@keyframes rpl{to{transform:scale(5);opacity:0}}

/* info drawer */
.drawer{
  display:grid;grid-template-rows:0fr;
  transition:grid-template-rows .32s cubic-bezier(.4,0,.2,1);
  margin-top:0;
}
.drawer.open{grid-template-rows:1fr;margin-top:1rem}
.drawer-inner{overflow:hidden}
.drawer-card{
  background:var(--midnight);border-radius:12px;
  padding:1.3rem 1.5rem;
  transform:translateY(-4px);opacity:0;
  transition:transform .25s .06s ease,opacity .25s .06s ease;
}
.drawer.open .drawer-card{transform:translateY(0);opacity:1}
.dc-name{
  font-family:var(--display);font-size:1rem;font-weight:600;color:#fff;
  margin-bottom:.55rem;display:flex;align-items:center;justify-content:space-between;
}
.dc-close{
  width:22px;height:22px;border-radius:50%;
  background:rgba(255,255,255,0.08);border:none;
  color:rgba(255,255,255,0.4);cursor:pointer;
  font-size:.85rem;line-height:1;
  display:flex;align-items:center;justify-content:center;
  transition:background .2s,color .2s;
}
.dc-close:hover{background:rgba(255,255,255,0.15);color:#fff}
.dc-text{font-size:.85rem;line-height:1.8;color:rgba(255,255,255,0.6)}
.dc-tags{display:flex;flex-wrap:wrap;gap:6px;margin-top:.9rem}
.dc-tag{
  font-size:.68rem;padding:.22rem .6rem;border-radius:4px;
  background:rgba(29,78,216,0.2);color:#93C5FD;
  border:1px solid rgba(59,130,246,0.2);
  animation:tag-pop .2s cubic-bezier(.34,1.56,.64,1) both;
}
.dc-tag:nth-child(2){animation-delay:.03s}
.dc-tag:nth-child(3){animation-delay:.06s}
.dc-tag:nth-child(4){animation-delay:.09s}
.dc-tag:nth-child(5){animation-delay:.12s}
.dc-tag:nth-child(6){animation-delay:.15s}
@keyframes tag-pop{from{transform:scale(.7);opacity:0}to{transform:scale(1);opacity:1}}

/* certs */
.cert-list{display:flex;flex-direction:column;gap:10px}
.cert{
  display:flex;align-items:center;gap:1rem;
  padding:.9rem 1.2rem;
  border:1.5px solid var(--border);border-radius:11px;
  transition:border-color .2s,transform .2s,box-shadow .2s;
}
.cert:hover{border-color:var(--blue);transform:translateX(4px);box-shadow:0 4px 18px rgba(29,78,216,0.08)}
.cert-dot{width:9px;height:9px;border-radius:50%;background:var(--teal);flex-shrink:0}
.cert-name{font-size:.9rem;font-weight:500;color:var(--midnight)}
.cert-sub{font-size:.73rem;color:var(--muted);margin-top:.1rem}
.cert-pill{
  margin-left:auto;font-size:.67rem;padding:.22rem .65rem;border-radius:20px;
  background:var(--surface);color:var(--muted);border:1px solid var(--border);
  white-space:nowrap;
}

/* what you'll find */
.find-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(190px,1fr));gap:10px}
.find-card{
  border:1.5px solid var(--border);border-radius:11px;
  padding:1rem 1.1rem;
  transition:border-color .2s,transform .2s,box-shadow .2s;
}
.find-card:hover{border-color:var(--navy);transform:translateY(-3px);box-shadow:0 6px 22px rgba(11,29,58,0.09)}
.find-icon{font-size:1.2rem;margin-bottom:.45rem}
.find-title{font-weight:600;font-size:.85rem;color:var(--midnight);margin-bottom:.25rem}
.find-desc{font-size:.77rem;color:var(--muted);line-height:1.6}

/* interests */
.int-row{display:flex;flex-wrap:wrap;gap:8px}
.int-tag{
  font-size:.82rem;padding:.38rem .95rem;
  border-radius:20px;border:1.5px solid var(--border);
  color:var(--muted);
  transition:border-color .2s,color .2s,background .2s;
  cursor:default;
}
.int-tag:hover{border-color:var(--midnight);color:var(--midnight);background:var(--off)}

/* ── CODE GUIDE ── */
.code-guide{
  border-top:2px solid var(--midnight);
  padding-top:2.5rem;margin-top:3rem;
}
.cg-head{font-family:var(--display);font-size:1.5rem;font-weight:700;color:var(--midnight);margin-bottom:.35rem}
.cg-sub{font-size:.88rem;color:var(--muted);line-height:1.7;margin-bottom:1.8rem}

.tabs{display:flex;gap:0;border-bottom:2px solid var(--border);margin-bottom:1.5rem}
.tb{
  font-size:.75rem;font-weight:500;letter-spacing:.4px;
  padding:.55rem 1.1rem;border:none;background:none;
  color:var(--muted);cursor:pointer;
  border-bottom:2px solid transparent;margin-bottom:-2px;
  transition:color .2s,border-color .2s;
}
.tb.on{color:var(--midnight);border-bottom-color:var(--midnight)}
.tpanel{display:none}
.tpanel.on{display:block}

.steps{display:flex;flex-direction:column;gap:2rem}
.step{display:flex;gap:1.1rem}
.sn{
  width:32px;height:32px;flex-shrink:0;
  border-radius:50%;background:var(--midnight);color:#fff;
  font-size:.8rem;font-weight:600;
  display:flex;align-items:center;justify-content:center;
  margin-top:.05rem;
}
.sb{}
.st{font-weight:600;font-size:.95rem;color:var(--midnight);margin-bottom:.3rem}
.sd{font-size:.84rem;color:var(--muted);line-height:1.75;margin-bottom:.75rem}
code{background:var(--surface);padding:2px 7px;border-radius:4px;font-size:.82rem;color:var(--navy)}
pre{
  background:var(--midnight);border-radius:10px;
  padding:1.2rem 1.4rem;overflow-x:auto;
  font-family:monospace;font-size:.76rem;line-height:1.8;color:#94BAED;
  position:relative;
}
.pl{
  position:absolute;top:8px;right:12px;
  font-size:.58rem;letter-spacing:2px;text-transform:uppercase;
  color:rgba(255,255,255,0.15);
}
.k{color:#7DD3FC}.s{color:#86EFAC}.c{color:#3E5060;font-style:italic}
.fn{color:#5EEAD4}.t{color:#FCA5A5}

/* footer */
footer{
  text-align:center;margin-top:3.5rem;padding-top:1.5rem;
  border-top:1px solid var(--border);
  font-size:.72rem;color:var(--muted);letter-spacing:.4px;
}
footer strong{color:var(--midnight)}
</style>
</head>
<body>

<!-- HERO -->
<div class="hero">
  <div class="container">
    <div class="hero-inner">
      <div class="av-wrap">
        <div class="av">SP</div>
        <div class="av-ring"></div>
        <div class="online-dot"></div>
      </div>
      <div>
        <p class="hero-meta">Network Engineer · Bengaluru, India</p>
        <h1 class="hero-name">Swathi Paramesh</h1>
        <p class="hero-role">5+ Years · Enterprise & Hybrid Infrastructure</p>
        <div class="hero-tags">
          <span class="htag">SD-WAN</span>
          <span class="htag">Routing & Switching</span>
          <span class="htag">Network Migrations</span>
          <span class="htag t">CCNA</span>
          <span class="htag t">AZ-900</span>
        </div>
      </div>
    </div>
  </div>
  <span class="wave"></span>
</div>

<!-- BODY -->
<div class="container">
<div class="page">

  <!-- ABOUT -->
  <div class="sec">
    <div class="sec-head">
      <h2 class="sec-title">About</h2>
      <span class="sec-line"></span>
    </div>
    <p class="about-p">Enterprise and hybrid infrastructure specialist with <strong>5+ years</strong> of experience in SD-WAN, routing & switching, and network migrations. I build reliable, scalable networks and enjoy solving complex infrastructure problems. Currently exploring deeper into <strong>network security</strong>, <strong>cloud networking</strong>, and <strong>infrastructure technologies</strong>.</p>
    <div class="kv-row">
      <div class="kv"><span class="kv-v">5+</span><span class="kv-l">Years Experience</span></div>
      <div class="kv"><span class="kv-v">SD-WAN</span><span class="kv-l">Primary Specialty</span></div>
      <div class="kv"><span class="kv-v">2</span><span class="kv-l">Certifications</span></div>
      <div class="kv"><span class="kv-v">📍</span><span class="kv-l">Bengaluru, India</span></div>
    </div>
  </div>

  <!-- TECH STACK -->
  <div class="sec">
    <div class="sec-head">
      <h2 class="sec-title">Tech Stack</h2>
      <span class="sec-line"></span>
    </div>
    <p style="font-size:.8rem;color:var(--muted);margin-bottom:.9rem">Click any technology to learn more</p>
    <div class="chips" id="chips"></div>
    <div class="drawer" id="drawer">
      <div class="drawer-inner">
        <div class="drawer-card">
          <div class="dc-name">
            <span id="dc-name">—</span>
            <button class="dc-close" id="dc-close">✕</button>
          </div>
          <p class="dc-text" id="dc-text">—</p>
          <div class="dc-tags" id="dc-tags"></div>
        </div>
      </div>
    </div>
  </div>

  <!-- CERTS -->
  <div class="sec">
    <div class="sec-head">
      <h2 class="sec-title">Certifications</h2>
      <span class="sec-line"></span>
    </div>
    <div class="cert-list">
      <div class="cert">
        <div class="cert-dot"></div>
        <div>
          <div class="cert-name">Cisco Certified Network Associate</div>
          <div class="cert-sub">CCNA · Cisco Systems</div>
        </div>
        <div class="cert-pill">Active</div>
      </div>
      <div class="cert">
        <div class="cert-dot"></div>
        <div>
          <div class="cert-name">Microsoft Azure Fundamentals</div>
          <div class="cert-sub">AZ-900 · Microsoft</div>
        </div>
        <div class="cert-pill">Active</div>
      </div>
    </div>
  </div>

  <!-- WHAT YOU'LL FIND -->
  <div class="sec">
    <div class="sec-head">
      <h2 class="sec-title">What You'll Find Here</h2>
      <span class="sec-line"></span>
    </div>
    <div class="find-grid">
      <div class="find-card"><div class="find-icon">📡</div><div class="find-title">SD-WAN Labs</div><div class="find-desc">Cisco SD-WAN configs and switching lab setups</div></div>
      <div class="find-card"><div class="find-icon">📝</div><div class="find-title">Documentation</div><div class="find-desc">Learning projects with detailed notes and guides</div></div>
      <div class="find-card"><div class="find-icon">🔍</div><div class="find-title">Troubleshooting</div><div class="find-desc">Real-world infrastructure troubleshooting notes</div></div>
      <div class="find-card"><div class="find-icon">☁️</div><div class="find-title">Cloud & Security</div><div class="find-desc">Azure experiments and security research</div></div>
    </div>
  </div>

  <!-- INTERESTS -->
  <div class="sec">
    <div class="sec-head">
      <h2 class="sec-title">Outside Tech</h2>
      <span class="sec-line"></span>
    </div>
    <div class="int-row">
      <span class="int-tag">📖 Reading</span>
      <span class="int-tag">🎵 Music</span>
      <span class="int-tag">🌱 Learning</span>
      <span class="int-tag">🔧 Skill Building</span>
      <span class="int-tag">🌩️ Cloud Exploration</span>
      <span class="int-tag">🔐 Security Research</span>
    </div>
  </div>

  <!-- ── CODE GUIDE ── -->
  <div class="code-guide">
    <h2 class="cg-head">How to Set This Up on GitHub</h2>
    <p class="cg-sub">Two things to set up: your GitHub profile README (shown on your github.com/username page) and this interactive page hosted via GitHub Pages. Both explained below.</p>

    <div class="tabs">
      <button class="tb on" onclick="tab('readme',this)">Profile README</button>
      <button class="tb" onclick="tab('page',this)">Host This Page</button>
      <button class="tb" onclick="tab('stats',this)">Add Live Stats</button>
    </div>

    <!-- README -->
    <div class="tpanel on" id="tp-readme">
      <div class="steps">

        <div class="step">
          <div class="sn">1</div>
          <div class="sb">
            <div class="st">Create your special profile repository</div>
            <p class="sd">Go to GitHub → New Repository. Name it exactly your GitHub username. GitHub will show a special banner — that's how it knows to display the README on your profile.</p>
            <pre><span class="c"># github.com → New Repository</span>
Repository name:  <span class="s">your-github-username</span>
Visibility:       <span class="k">Public</span>
☑  Add a README file  <span class="c"># tick this</span></pre>
          </div>
        </div>

        <div class="step">
          <div class="sn">2</div>
          <div class="sb">
            <div class="st">Header — name, role, and badges</div>
            <p class="sd">Open the README.md file and replace the contents with this. The badges are from shields.io and render automatically in GitHub.</p>
            <pre><span class="pl">README.md</span><span class="k">&lt;div</span> align=<span class="s">"center"</span><span class="k">&gt;</span>

<span class="k">&lt;h1&gt;</span>Hi, I'm Swathi Paramesh 👋<span class="k">&lt;/h1&gt;</span>
<span class="k">&lt;h3&gt;</span>Network Engineer · SD-WAN · Cloud · Security<span class="k">&lt;/h3&gt;</span>

<span class="fn">![Location](https://img.shields.io/badge/📍_Bengaluru-India-0B1D3A?style=flat-square&labelColor=0B1D3A&color=1D4ED8)</span>
<span class="fn">![Experience](https://img.shields.io/badge/Experience-5%2B_Years-0D9488?style=flat-square)</span>
<span class="fn">![CCNA](https://img.shields.io/badge/Certified-CCNA-1D4ED8?style=flat-square&logo=cisco&logoColor=white)</span>
<span class="fn">![AZ900](https://img.shields.io/badge/Certified-AZ--900-0078D4?style=flat-square&logo=microsoftazure&logoColor=white)</span>

<span class="k">&lt;/div&gt;</span></pre>
          </div>
        </div>

        <div class="step">
          <div class="sn">3</div>
          <div class="sb">
            <div class="st">About Me section</div>
            <pre><span class="pl">README.md</span><span class="c">## 👩‍💻 About Me</span>

Enterprise & hybrid infrastructure specialist with **5+ years** of experience.
Specialising in SD-WAN, routing & switching, and network migrations.

- 🌐 Working with: Cisco Catalyst SD-WAN · Meraki · Cisco 9K
- 🔭 Exploring: Network Security · Cloud Networking
- 📍 Based in **Bengaluru, India**</pre>
          </div>
        </div>

        <div class="step">
          <div class="sn">4</div>
          <div class="sb">
            <div class="st">Tech stack badges — each links to official docs</div>
            <p class="sd">These are the GitHub equivalent of the clickable buttons on this page. Each badge is a link to the official documentation.</p>
            <pre><span class="pl">README.md</span><span class="c">## 🛠️ Tech Stack</span>

**Networking**

<span class="fn">[![SD-WAN](https://img.shields.io/badge/Cisco_Catalyst_SD--WAN-1D4ED8?style=for-the-badge&logo=cisco&logoColor=white)](https://www.cisco.com/c/en/us/solutions/enterprise-networks/sd-wan)</span>
<span class="fn">[![Meraki](https://img.shields.io/badge/Cisco_Meraki-0D9488?style=for-the-badge&logo=cisco&logoColor=white)](https://meraki.cisco.com)</span>
<span class="fn">[![Cisco9K](https://img.shields.io/badge/Cisco_9K_Series-0B1D3A?style=for-the-badge&logo=cisco&logoColor=white)](https://www.cisco.com)</span>

**Protocols**

<span class="fn">[![OSPF](https://img.shields.io/badge/OSPF-0B1D3A?style=flat-square)](https://en.wikipedia.org/wiki/OSPF)</span>
<span class="fn">[![BGP](https://img.shields.io/badge/BGP-0B1D3A?style=flat-square)](https://en.wikipedia.org/wiki/BGP)</span>
<span class="fn">[![EIGRP](https://img.shields.io/badge/EIGRP-0B1D3A?style=flat-square)](https://www.cisco.com/c/en/us/tech/ip/enhanced-interior-gateway-routing-protocol-eigrp)</span>

**Cloud & Monitoring**

<span class="fn">[![Azure](https://img.shields.io/badge/Microsoft_Azure-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white)](https://azure.microsoft.com)</span>
<span class="fn">[![PRTG](https://img.shields.io/badge/PRTG_Monitoring-008FD5?style=for-the-badge)](https://www.paessler.com/prtg)</span></pre>
          </div>
        </div>

        <div class="step">
          <div class="sn">5</div>
          <div class="sb">
            <div class="st">Certifications and repo highlights</div>
            <pre><span class="pl">README.md</span><span class="c">## 🏅 Certifications</span>

| Certification | Issuer | Status |
|--------------|--------|--------|
| **CCNA** — Cisco Certified Network Associate | Cisco | ✅ Active |
| **AZ-900** — Microsoft Azure Fundamentals | Microsoft | ✅ Active |

---

<span class="c">## 📂 What You'll Find Here</span>

| | Topic | Description |
|-|-------|-------------|
| 📡 | **SD-WAN Labs** | Cisco SD-WAN configs and switching setups |
| 📝 | **Documentation** | Learning projects with detailed notes |
| 🔍 | **Troubleshooting** | Real-world infra troubleshooting references |
| ☁️ | **Cloud & Security** | Azure and security experiments |</pre>
          </div>
        </div>

      </div>
    </div><!-- /tp-readme -->

    <!-- HOST PAGE -->
    <div class="tpanel" id="tp-page">
      <div class="steps">

        <div class="step">
          <div class="sn">1</div>
          <div class="sb">
            <div class="st">Save this file</div>
            <p class="sd">Download the HTML file you received. Rename it to <code>index.html</code> — this is required for GitHub Pages to serve it correctly.</p>
          </div>
        </div>

        <div class="step">
          <div class="sn">2</div>
          <div class="sb">
            <div class="st">Create a GitHub Pages repository</div>
            <p class="sd">Create a new public repo named exactly <code>yourusername.github.io</code> — GitHub automatically serves it as a website.</p>
            <pre><span class="c"># github.com → New Repository</span>
Name:        <span class="s">swathiparamesh.github.io</span>
Visibility:  <span class="k">Public</span></pre>
          </div>
        </div>

        <div class="step">
          <div class="sn">3</div>
          <div class="sb">
            <div class="st">Push the file via Git</div>
            <pre><span class="fn">git</span> init
<span class="fn">git</span> add index.html
<span class="fn">git</span> commit -m <span class="s">"Add profile page"</span>
<span class="fn">git</span> branch -M main
<span class="fn">git</span> remote add origin https://github.com/<span class="t">USERNAME</span>/<span class="t">USERNAME</span>.github.io.git
<span class="fn">git</span> push -u origin main</pre>
          </div>
        </div>

        <div class="step">
          <div class="sn">4</div>
          <div class="sb">
            <div class="st">Enable GitHub Pages</div>
            <p class="sd">In the repo: Settings → Pages → Source: Deploy from branch → Branch: main → / (root) → Save. Your page goes live at <strong>yourusername.github.io</strong> within a minute or two.</p>
          </div>
        </div>

        <div class="step">
          <div class="sn">5</div>
          <div class="sb">
            <div class="st">Link it from your profile README</div>
            <pre><span class="pl">README.md</span><span class="c">## 🌐 Portfolio</span>

👉 [View my interactive profile](https://swathiparamesh.github.io)</pre>
          </div>
        </div>

      </div>
    </div><!-- /tp-page -->

    <!-- STATS -->
    <div class="tpanel" id="tp-stats">
      <div class="steps">

        <div class="step">
          <div class="sn">1</div>
          <div class="sb">
            <div class="st">GitHub Stats card</div>
            <p class="sd">This auto-updates every day. Replace <code>YOUR_USERNAME</code> with your actual GitHub username.</p>
            <pre><span class="pl">README.md</span><span class="k">&lt;div</span> align=<span class="s">"center"</span><span class="k">&gt;</span>

<span class="fn">![Stats](https://github-readme-stats.vercel.app/api?username=YOUR_USERNAME&show_icons=true&theme=react&hide_border=true&bg_color=0B1D3A&title_color=3B82F6&text_color=94BAED&icon_color=0D9488)</span>

<span class="k">&lt;/div&gt;</span></pre>
          </div>
        </div>

        <div class="step">
          <div class="sn">2</div>
          <div class="sb">
            <div class="st">Streak counter</div>
            <pre><span class="pl">README.md</span><span class="fn">![Streak](https://streak-stats.demolab.com/?user=YOUR_USERNAME&theme=react&hide_border=true&background=0B1D3A&ring=1D4ED8&fire=0D9488&currStreakLabel=94BAED)</span></pre>
          </div>
        </div>

        <div class="step">
          <div class="sn">3</div>
          <div class="sb">
            <div class="st">Visitor badge and LinkedIn</div>
            <pre><span class="pl">README.md</span><span class="k">&lt;div</span> align=<span class="s">"center"</span><span class="k">&gt;</span>

<span class="fn">![Views](https://komarev.com/ghpvc/?username=YOUR_USERNAME&color=1D4ED8&style=flat-square&label=Profile+Views)</span>

<span class="fn">[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/YOUR_PROFILE)</span>

<span class="k">&lt;/div&gt;</span></pre>
          </div>
        </div>

      </div>
    </div><!-- /tp-stats -->

  </div><!-- code-guide -->

</div><!-- page -->
</div><!-- container -->

<footer>
  Built for <strong>Swathi Paramesh</strong> · Network Engineer · Bengaluru
</footer>

<script>
const TECH = [
  {
    label:"Cisco Catalyst SD-WAN",
    name:"Cisco Catalyst SD-WAN",
    text:"Enterprise SD-WAN platform delivering intelligent traffic routing, application-aware policies, and Zero Trust security across hybrid WAN environments. Core platform for enterprise branch connectivity.",
    tags:["vManage","vBond","vSmart","ZTP","App-Aware Routing","Policy Templates"]
  },
  {
    label:"Cisco Meraki",
    name:"Cisco Meraki",
    text:"Cloud-managed networking platform providing centralised visibility and control over switching, wireless, and security across distributed enterprise environments through a unified dashboard.",
    tags:["MX Security","MS Switching","MR Wireless","Dashboard API","Auto-VPN"]
  },
  {
    label:"Cisco 9K Series",
    name:"Cisco 9000 Series",
    text:"High-performance campus and data-centre switching used for enterprise core infrastructure, spine-leaf architectures, and reliable high-density deployments at scale.",
    tags:["Cat 9200","Cat 9300","StackWise","DNA Center","High Availability"]
  },
  {
    label:"Routing & Switching",
    name:"Routing & Switching",
    text:"Deep enterprise experience with routing and switching protocols across large campus and WAN environments, including design, migration, and optimisation.",
    tags:["OSPF","BGP","EIGRP","VLAN/STP","QoS","HSRP/VRRP"]
  },
  {
    label:"Microsoft Azure",
    name:"Microsoft Azure",
    text:"Foundational cloud knowledge (AZ-900 certified) with active exploration of hybrid connectivity patterns including Virtual WAN, ExpressRoute, and Azure network services.",
    tags:["Virtual WAN","ExpressRoute","VNet Peering","Azure Firewall","NSG"]
  },
  {
    label:"Network Monitoring",
    name:"Network Monitoring",
    text:"Enterprise monitoring for performance tracking, anomaly detection, and SLA management across complex hybrid infrastructure environments.",
    tags:["PRTG","Grafana","SNMP","Syslog","NetFlow"]
  },
  {
    label:"Network Security",
    name:"Network Security",
    text:"Actively deepening expertise in Zero Trust architecture, firewall policy design, and threat mitigation in SD-WAN and hybrid cloud environments.",
    tags:["Zero Trust","IPSec VPN","ACLs","Cisco Umbrella","ISE","Firewall Policies"]
  },
];

const grid = document.getElementById('chips');
const drawer = document.getElementById('drawer');
const dcName = document.getElementById('dc-name');
const dcText = document.getElementById('dc-text');
const dcTags = document.getElementById('dc-tags');
const dcClose = document.getElementById('dc-close');
let activeBtn = null, activeIdx = -1;

function close(){
  drawer.classList.remove('open');
  if(activeBtn){activeBtn.classList.remove('on');activeBtn=null;}
  activeIdx=-1;
}

dcClose.addEventListener('click',close);

TECH.forEach((t,i)=>{
  const btn=document.createElement('button');
  btn.className='chip';
  btn.innerHTML=`<span>${t.label}</span>`;

  btn.addEventListener('click',e=>{
    // ripple
    const r=document.createElement('span');
    r.className='rpl';
    const rc=btn.getBoundingClientRect();
    const s=Math.max(rc.width,rc.height);
    r.style.cssText=`width:${s}px;height:${s}px;left:${e.clientX-rc.left-s/2}px;top:${e.clientY-rc.top-s/2}px`;
    btn.appendChild(r);
    setTimeout(()=>r.remove(),500);

    if(activeIdx===i){close();return;}
    if(activeBtn) activeBtn.classList.remove('on');
    btn.classList.add('on');
    activeBtn=btn; activeIdx=i;

    dcName.textContent=t.name;
    dcText.textContent=t.text;
    dcTags.innerHTML=t.tags.map(x=>`<span class="dc-tag">${x}</span>`).join('');
    drawer.classList.remove('open');
    void drawer.offsetWidth;
    drawer.classList.add('open');
    setTimeout(()=>drawer.scrollIntoView({behavior:'smooth',block:'nearest'}),60);
  });

  grid.appendChild(btn);
});

function tab(id,el){
  document.querySelectorAll('.tb').forEach(b=>b.classList.remove('on'));
  document.querySelectorAll('.tpanel').forEach(p=>p.classList.remove('on'));
  el.classList.add('on');
  document.getElementById('tp-'+id).classList.add('on');
}
</script>
</body>
</html>

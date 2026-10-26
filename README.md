# warse172-star.github.io
Official personal portfolio of Arsaney Warsey | Programmer &amp; Web Developer 

<!DOCTYPE html>
<html lang="en" dir="ltr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#080808">
<meta name="description" content="Arsaney Warsey — Programmer and Web Developer. Discover my skills, projects and services.">
<meta name="author" content="Arsaney Warsey">
<title>Arsaney Warsey | Developer Portfolio</title>
<style>
:root {
  --bg:#080808;--surface:#101010;--surface2:#151515;
  --text:#f4f4f4;--muted:#a0a0a0;--accent:#d5b477;
  --border:#272727;--radius:18px;
}
*{box-sizing:border-box;margin:0;padding:0}
html{scroll-behavior:smooth;scroll-padding-top:90px}
body{font-family:Inter,system-ui,-apple-system,Arial,sans-serif;background:var(--bg);color:var(--text);line-height:1.7;overflow-x:hidden}
a{color:inherit;text-decoration:none}
button,input,textarea{font:inherit}
button,a{-webkit-tap-highlight-color:transparent}
button{cursor:pointer}
.container{width:min(1120px,90%);margin:auto}
header{position:sticky;top:0;z-index:100;background:#080808ed;backdrop-filter:blur(18px);border-bottom:1px solid var(--border)}
.nav{min-height:76px;display:flex;align-items:center;justify-content:space-between;gap:18px}
.brand{font-weight:850;font-size:22px;letter-spacing:-1px}
.brand span{color:var(--accent)}
.navlinks{display:flex;align-items:center;gap:22px}
.navlinks a{font-size:13px;color:#c4c4c4;transition:.2s}
.navlinks a:hover,.navlinks a.active{color:var(--accent)}
.navtools{display:flex;align-items:center;gap:10px}
.lang,.menu-btn{background:var(--surface2);border:1px solid var(--border);color:var(--text);padding:8px 12px;border-radius:9px}
.menu-btn{display:none}
.hero{min-height:660px;display:grid;grid-template-columns:1.25fr .75fr;align-items:center;gap:60px;padding-top:75px;padding-bottom:90px}
.eyebrow{display:inline-flex;align-items:center;gap:9px;border:1px solid #343026;color:var(--accent);border-radius:50px;padding:7px 13px;font-size:12px;letter-spacing:1px}
.dot{width:7px;height:7px;border-radius:50%;background:var(--accent);box-shadow:0 0 12px var(--accent)}
h1{font-size:clamp(42px,6.4vw,76px);line-height:1.12;letter-spacing:-2.7px;margin:24px 0}
.gold{color:var(--accent)}
.lead{max-width:590px;color:var(--muted);font-size:17px}
.actions{display:flex;gap:12px;flex-wrap:wrap;margin-top:30px}
.btn{display:inline-flex;justify-content:center;align-items:center;gap:9px;padding:12px 19px;border:1px solid var(--border);border-radius:10px;transition:.25s;font-weight:650;font-size:14px}
.btn:hover{transform:translateY(-3px);border-color:var(--accent)}
.btn.primary{background:var(--accent);color:#100d07;border-color:var(--accent)}
.btn.primary:hover{background:#e7ca91}
.hero-meta{display:flex;gap:25px;margin-top:36px;color:var(--muted);font-size:12px;flex-wrap:wrap}
.hero-meta strong{color:var(--text);display:block;font-size:14px}
.visual{min-height:360px;border:1px solid #29251e;border-radius:28px;background:radial-gradient(ellipse at 50% 40%,#44361c35,transparent 60%),linear-gradient(145deg,#161616,#0b0b0b);display:flex;align-items:center;justify-content:center;position:relative;overflow:hidden}
.visual:before,.visual:after{content:"";position:absolute;border:1px solid #bda16a25;border-radius:50%;width:270px;height:270px;animation:orbit 18s linear infinite}
.visual:after{width:210px;height:210px;animation-direction:reverse;animation-duration:13s}
.monogram{font-size:110px;font-weight:900;letter-spacing:-12px;color:#e0c28a;text-shadow:0 0 55px #c9a56522;z-index:1}
.visual-caption{position:absolute;bottom:24px;text-align:center;font-size:11px;color:var(--muted);letter-spacing:3px}
@keyframes orbit{to{transform:rotate(360deg)}}
.section{padding:95px 0;border-top:1px solid #1c1c1c}
.section-head{display:flex;justify-content:space-between;align-items:end;gap:25px;margin-bottom:36px}
.kicker{font-size:11px;letter-spacing:2px;text-transform:uppercase;color:var(--accent)}
h2{font-size:clamp(30px,4vw,43px);letter-spacing:-1.2px;line-height:1.25;margin-top:7px}
.section-intro{max-width:470px;color:var(--muted);font-size:14px}
.about-grid{display:grid;grid-template-columns:1fr 1fr;gap:25px}
.panel{border:1px solid var(--border);border-radius:var(--radius);background:linear-gradient(140deg,#131313,#0b0b0b);padding:30px}
.panel p{color:var(--muted);font-size:14px;margin-top:12px}
.fact-list{display:grid;grid-template-columns:1fr 1fr;gap:12px;margin-top:20px}
.fact{padding:15px;border-radius:11px;background:#171717}
.fact span{display:block;color:var(--muted);font-size:11px}
.fact strong{font-size:14px}
.skills-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:14px}
.skill{padding:21px;border:1px solid var(--border);border-radius:13px;background:var(--surface);transition:.25s}
.skill:hover{border-color:#806b43;transform:translateY(-4px)}
.skill-top{display:flex;align-items:center;gap:12px}
.skill-icon{width:40px;height:40px;display:grid;place-items:center;border:1px solid #3b3325;background:#201b13;color:var(--accent);border-radius:10px;font-weight:800}
.skill h3{font-size:15px}
.skill p{font-size:12px;color:var(--muted);margin-top:8px}
.project-grid,.service-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:17px}
.project{border:1px solid var(--border);border-radius:16px;overflow:hidden;background:var(--surface);transition:.25s}
.project:hover{transform:translateY(-5px);border-color:#806b43}
.project-art{height:160px;display:grid;place-items:center;background:radial-gradient(ellipse at center,#57432640,transparent 65%),#121212;border-bottom:1px solid var(--border);font-size:42px;color:var(--accent)}
.project-body{padding:22px}
.project h3,.service h3{font-size:17px}
.project p,.service p{font-size:13px;color:var(--muted);margin:9px 0 16px}
.tags{display:flex;gap:7px;flex-wrap:wrap;margin-bottom:17px}
.tags span{font-size:10px;color:#d6c6a4;background:#201c15;padding:4px 8px;border-radius:5px}
.text-link{color:var(--accent);font-size:13px;font-weight:700}
.service{border:1px solid var(--border);border-radius:15px;padding:25px;background:var(--surface);transition:.25s}
.service:hover{border-color:#806b43}
.service-icon{font-size:25px;color:var(--accent);margin-bottom:17px}
.service ul{list-style:none;color:var(--muted);font-size:12px}
.service li{padding:5px 0}
.service li:before{content:"— ";color:var(--accent)}
.contact-grid{display:grid;grid-template-columns:.8fr 1.2fr;gap:25px}
.contact-info{display:flex;flex-direction:column;gap:12px;margin-top:22px}
.contact-item{border:1px solid var(--border);border-radius:10px;padding:14px}
.contact-item small{display:block;color:var(--muted);font-size:11px}
.contact-item strong{font-size:13px;overflow-wrap:anywhere}
form{display:grid;gap:14px}
label{display:block;font-size:12px;color:#ccc;margin-bottom:6px}
input,textarea{width:100%;background:#090909;border:1px solid #303030;color:var(--text);padding:13px;border-radius:9px;outline:none}
input:focus,textarea:focus{border-color:var(--accent)}
textarea{min-height:130px;resize:vertical}
.form-note{font-size:11px;color:var(--muted)}
footer{padding:25px 0;border-top:1px solid var(--border);color:var(--muted);font-size:12px}
.footer-inner{display:flex;justify-content:space-between;align-items:center;gap:16px;flex-wrap:wrap}
.backtop{color:var(--accent)}
.toast{position:fixed;bottom:20px;left:50%;transform:translate(-50%,130px);background:#191919;border:1px solid #51452f;color:var(--text);padding:13px 20px;border-radius:10px;z-index:200;transition:.3s;font-size:13px;max-width:90%;text-align:center}
.toast.show{transform:translate(-50%,0)}
[dir="rtl"] body{text-align:right}
[dir="rtl"] .section-head{flex-direction:row}
[dir="rtl"] .hero{direction:rtl}
[dir="rtl"] .navlinks{direction:rtl}
[dir="rtl"] .text-link{display:inline-block}
@media(max-width:850px){
 .hero{grid-template-columns:1fr;gap:30px;min-height:auto;padding-top:80px}
 .visual{min-height:260px;grid-row:1}
 .monogram{font-size:85px}
 .project-grid,.service-grid{grid-template-columns:repeat(2,1fr)}
 .navlinks{gap:12px}
 .navlinks a{font-size:12px}
}
@media(max-width:600px){
 .nav{min-height:66px;flex-wrap:wrap}
 .menu-btn{display:block}
 .navlinks{display:none;order:3;width:100%;flex-direction:column;align-items:stretch;padding:10px 0 17px}
 .navlinks.open{display:flex}
 .navlinks a{padding:7px 0;font-size:14px}
 .hero{padding-top:55px;padding-bottom:65px}
 h1{letter-spacing:-1.7px}
 .lead{font-size:15px}
 .visual{min-height:230px}
 .section{padding:68px 0}
 .section-head{display:block}
 .section-intro{margin-top:12px}
 .about-grid,.skills-grid,.project-grid,.service-grid,.contact-grid{grid-template-columns:1fr}
 .panel{padding:23px}
 .fact-list{grid-template-columns:1fr 1fr}
 .project-art{height:140px}
 [dir="rtl"] .section-head{display:block}
}
@media(prefers-reduced-motion:reduce){*,*::before,*::after{animation-duration:.01ms!important;transition-duration:.01ms!important;scroll-behavior:auto!important}}
</style>
</head>
<body>
<header>
<div class="container nav">
<a class="brand" href="#home">ARSANEY<span>.</span></a>
<nav class="navlinks" id="navlinks">
<a href="#about" data-i18n="navAbout">About</a>
<a href="#skills" data-i18n="navSkills">Skills</a>
<a href="#projects" data-i18n="navProjects">Projects</a>
<a href="#services" data-i18n="navServices">Services</a>
<a href="#contact" data-i18n="navContact">Contact</a>
</nav>
<div class="navtools">
<button class="lang" id="langBtn" type="button">العربية</button>
<button class="menu-btn" id="menuBtn" type="button" aria-label="Toggle menu">☰</button>
</div>
</div>
</header>

<main>
<section class="container hero" id="home">
<div class="hero-copy">
<div class="eyebrow"><span class="dot"></span><span data-i18n="eyebrow">PERSONAL DEVELOPER PORTFOLIO</span></div>
<h1><span data-i18n="hello">Hello, I'm</span><br><span class="gold">Arsaney Warsey.</span></h1>
<p class="lead" data-i18n="heroText">I build thoughtful digital experiences, modern websites, and clean interfaces with a focus on detail and usability.</p>
<div class="actions">
<a href="#projects" class="btn primary"><span data-i18n="viewWork">Explore My Work</span> ↗</a>
<a href="#contact" class="btn"><span data-i18n="contactMe">Contact Me</span> →</a>
</div>
<div class="hero-meta">
<div><strong>06+</strong><span data-i18n="metaSkills">Technologies</span></div>
<div><strong>Web</strong><span data-i18n="metaFocus">Development Focus</span></div>
<div><strong>∞</strong><span data-i18n="metaIdeas">Ideas to Build</span></div>
</div>
</div>
<div class="visual" aria-label="Arsaney Warsey monogram">
<div class="monogram">AW</div>
<div class="visual-caption">DESIGN · CODE · CREATE</div>
</div>
</section>

<section class="section" id="about">
<div class="container">
<div class="section-head">
<div><div class="kicker" data-i18n="aboutKicker">A LITTLE ABOUT ME</div><h2 data-i18n="aboutTitle">Building with <span class="gold">purpose.</span></h2></div>
<p class="section-intro" data-i18n="aboutIntro">A personal introduction, my approach to development, and what I aim to create.</p>
</div>
<div class="about-grid">
<div class="panel">
<h3 data-i18n="aboutCardTitle">Hi, I'm Arsaney.</h3>
<p data-i18n="aboutText">I'm a programmer interested in web development, technology, and creating useful digital experiences. I enjoy learning, experimenting with code, and turning ideas into clear, responsive interfaces. This portfolio is my home on the web, where I can share my skills and future work.</p>
<p data-i18n="aboutText2">My focus is on continuous learning, clean design, accessibility, and building projects that work well across different screen sizes.</p>
</div>
<div class="panel">
<h3 data-i18n="quickFacts">Quick Overview</h3>
<div class="fact-list">
<div class="fact"><span data-i18n="factRole">Role</span><strong data-i18n="factRoleValue">Programmer</strong></div>
<div class="fact"><span data-i18n="factInterest">Main Interest</span><strong data-i18n="factInterestValue">Web Development</strong></div>
<div class="fact"><span data-i18n="factApproach">Approach</span><strong data-i18n="factApproachValue">Learn & Build</strong></div>
<div class="fact"><span data-i18n="factGoal">Goal</span><strong data-i18n="factGoalValue">Useful Experiences</strong></div>
</div>
</div>
</div>
</div>
</section>

<section class="section" id="skills">
<div class="container">
<div class="section-head">
<div><div class="kicker" data-i18n="skillsKicker">TOOLS OF THE TRADE</div><h2 data-i18n="skillsTitle">Skills & <span class="gold">Technologies.</span></h2></div>
<p class="section-intro" data-i18n="skillsIntro">Technologies I am learning and exploring in my programming journey. Skill levels are not exaggerated.</p>
</div>
<div class="skills-grid">
<div class="skill"><div class="skill-top"><div class="skill-icon">H5</div><h3>HTML</h3></div><p data-i18n="htmlText">Semantic structure for accessible web pages.</p></div>
<div class="skill"><div class="skill-top"><div class="skill-icon">C3</div><h3>CSS</h3></div><p data-i18n="cssText">Layouts, responsive design, and visual styling.</p></div>
<div class="skill"><div class="skill-top"><div class="skill-icon">JS</div><h3>JavaScript</h3></div><p data-i18n="jsText">Interactive behavior and dynamic interfaces.</p></div>
<div class="skill"><div class="skill-top"><div class="skill-icon">Py</div><h3>Python</h3></div><p data-i18n="pythonText">Programming logic and scripting fundamentals.</p></div>
<div class="skill"><div class="skill-top"><div class="skill-icon">PHP</div><h3>PHP</h3></div><p data-i18n="phpText">Server-side development fundamentals.</p></div>
<div class="skill"><div class="skill-top"><div class="skill-icon">R</div><h3>React</h3></div><p data-i18n="reactText">Component-based interface development.</p></div>
</div>
</div>
</section>

<section class="section" id="projects">
<div class="container">
<div class="section-head">
<div><div class="kicker" data-i18n="projectsKicker">SELECTED WORK</div><h2 data-i18n="projectsTitle">Projects & <span class="gold">Experiments.</span></h2></div>
<p class="section-intro" data-i18n="projectsIntro">A few project concepts to explore. Replace these examples with your real projects as you publish them.</p>
</div>
<div class="project-grid">
<article class="project">
<div class="project-art">⌘</div>
<div class="project-body"><h3 data-i18n="project1Title">Personal Portfolio</h3><p data-i18n="project1Text">A responsive personal website with bilingual content, a refined dark theme, and smooth navigation.</p><div class="tags"><span>HTML</span><span>CSS</span><span>JavaScript</span></div><a class="text-link" href="#home" data-i18n="project1Link">Explore this site ↗</a></div>
</article>
<article class="project">
<div class="project-art">◈</div>
<div class="project-body"><h3 data-i18n="project2Title">Business Landing Page</h3><p data-i18n="project2Text">A concept for a clean business website with service details, clear calls to action, and mobile-friendly sections.</p><div class="tags"><span>UI Design</span><span>Responsive</span></div><a class="text-link" href="#contact" data-i18n="project2Link">Discuss a similar idea ↗</a></div>
</article>
<article class="project">
<div class="project-art">⌘</div>
<div class="project-body"><h3 data-i18n="project3Title">Interactive Web Concept</h3><p data-i18n="project3Text">A learning project focused on useful interactions, accessible controls, and thoughtful user experience.</p><div class="tags"><span>JavaScript</span><span>Interaction</span></div><a class="text-link" href="https://github.com/warse172-star" target="_blank" rel="noopener" data-i18n="project3Link">Visit my GitHub ↗</a></div>
</article>
</div>
<p class="form-note" style="margin-top:18px" data-i18n="projectNote">Note: The first card links to this portfolio; the other cards are project concepts, not claims of completed client work.</p>
</div>
</section>

<section class="section" id="services">
<div class="container">
<div class="section-head">
<div><div class="kicker" data-i18n="servicesKicker">HOW I CAN HELP</div><h2 data-i18n="servicesTitle">Services & <span class="gold">Solutions.</span></h2></div>
<p class="section-intro" data-i18n="servicesIntro">Areas I can help with as my skills develop. Contact me to discuss your specific needs.</p>
</div>
<div class="service-grid">
<article class="service"><div class="service-icon">◫</div><h3 data-i18n="service1Title">Website Development</h3><p data-i18n="service1Text">Modern responsive websites designed to work across mobile and desktop screens.</p><ul><li data-i18n="service1a">Landing pages</li><li data-i18n="service1b">Personal portfolios</li><li data-i18n="service1c">Responsive layouts</li></ul></article>
<article class="service"><div class="service-icon">✳</div><h3 data-i18n="service2Title">Website UI & Styling</h3><p data-i18n="service2Text">Clean interfaces with thoughtful typography, layout, and subtle visual details.</p><ul><li data-i18n="service2a">Dark and light themes</li><li data-i18n="service2b">Interactive components</li><li data-i18n="service2c">Mobile-friendly design</li></ul></article>
<article class="service"><div class="service-icon">⌘</div><h3 data-i18n="service3Title">Programming Projects</h3><p data-i18n="service3Text">Small programming tasks and prototypes with a focus on clarity and maintainability.</p><ul><li data-i18n="service3a">Basic scripting</li><li data-i18n="service3b">Website improvements</li><li data-i18n="service3c">Learning prototypes</li></ul></article>
</div>
</div>
</section>

<section class="section" id="contact">
<div class="container">
<div class="section-head">
<div><div class="kicker" data-i18n="contactKicker">START A CONVERSATION</div><h2 data-i18n="contactTitle">Let's build something <span class="gold">good.</span></h2></div>
<p class="section-intro" data-i18n="contactIntro">Have a website idea, a question, or a project to discuss? Use the form to prepare a message.</p>
</div>
<div class="contact-grid">
<div class="panel">
<h3 data-i18n="contactCardTitle">Get in touch</h3>
<p data-i18n="contactCardText">You can also find my public programming profile here.</p>
<div class="contact-info">
<a class="contact-item" href="https://github.com/warse172-star" target="_blank" rel="noopener"><small>GitHub</small><strong>github.com/warse172-star ↗</strong></a>
<div class="contact-item"><small data-i18n="websiteLabel">Website</small><strong>warse172-star.github.io</strong></div>
</div>
</div>
<div class="panel">
<form id="contactForm">
<div><label for="name" data-i18n="nameLabel">Your name</label><input id="name" name="name" required maxlength="100" autocomplete="name" placeholder="Name"></div>
<div><label for="email" data-i18n="emailLabel">Your email (optional)</label><input id="email" name="email" type="email" maxlength="150" autocomplete="email" placeholder="you@example.com"></div>
<div><label for="message" data-i18n="messageLabel">Your message</label><textarea id="message" name="message" required maxlength="3000" placeholder="Tell me about your idea..."></textarea></div>
<button class="btn primary" type="submit"><span data-i18n="sendMessage">Prepare Message</span> ↗</button>
<p class="form-note" data-i18n="formNote">This form opens your email app to send the message. It does not send or store messages by itself.</p>
</form>
</div>
</div>
</div>
</section>
</main>

<footer>
<div class="container footer-inner">
<span>© <span id="year"></span> Arsaney Warsey. <span data-i18n="footerText">Made with care.</span></span>
<a href="#home" class="backtop" data-i18n="backTop">Back to top ↑</a>
</div>
</footer>
<div class="toast" id="toast" role="status" aria-live="polite"></div>

<script>
const translations = {
en:{
navAbout:"About",navSkills:"Skills",navProjects:"Projects",navServices:"Services",navContact:"Contact",
eyebrow:"PERSONAL DEVELOPER PORTFOLIO",hello:"Hello, I'm",heroText:"I build thoughtful digital experiences, modern websites, and clean interfaces with a focus on detail and usability.",
viewWork:"Explore My Work",contactMe:"Contact Me",metaSkills:"Technologies",metaFocus:"Development Focus",metaIdeas:"Ideas to Build",
aboutKicker:"A LITTLE ABOUT ME",aboutTitle:'Building with <span class="gold">purpose.</span>',aboutIntro:"A personal introduction, my approach to development, and what I aim to create.",
aboutCardTitle:"Hi, I'm Arsaney.",aboutText:"I'm a programmer interested in web development, technology, and creating useful digital experiences. I enjoy learning, experimenting with code, and turning ideas into clear, responsive interfaces. This portfolio is my home on the web, where I can share my skills and future work.",aboutText2:"My focus is on continuous learning, clean design, accessibility, and building projects that work well across different screen sizes.",
quickFacts:"Quick Overview",factRole:"Role",factRoleValue:"Programmer",factInterest:"Main Interest",factInterestValue:"Web Development",factApproach:"Approach",factApproachValue:"Learn & Build",factGoal:"Goal",factGoalValue:"Useful Experiences",
skillsKicker:"TOOLS OF THE TRADE",skillsTitle:'Skills & <span class="gold">Technologies.</span>',skillsIntro:"Technologies I am learning and exploring in my programming journey. Skill levels are not exaggerated.",
htmlText:"Semantic structure for accessible web pages.",cssText:"Layouts, responsive design, and visual styling.",jsText:"Interactive behavior and dynamic interfaces.",pythonText:"Programming logic and scripting fundamentals.",phpText:"Server-side development fundamentals.",reactText:"Component-based interface development.",
projectsKicker:"SELECTED WORK",projectsTitle:'Projects & <span class="gold">Experiments.</span>',projectsIntro:"A few project concepts to explore. Replace these examples with your real projects as you publish them.",
project1Title:"Personal Portfolio",project1Text:"A responsive personal website with bilingual content, a refined dark theme, and smooth navigation.",project1Link:"Explore this site ↗",
project2Title:"Business Landing Page",project2Text:"A concept for a clean business website with service details, clear calls to action, and mobile-friendly sections.",project2Link:"Discuss a similar idea ↗",
project3Title:"Interactive Web Concept",project3Text:"A learning project focused on useful interactions, accessible controls, and thoughtful user experience.",project3Link:"Visit my GitHub ↗",
projectNote:"Note: The first card links to this portfolio; the other cards are project concepts, not claims of completed client work.",
servicesKicker:"HOW I CAN HELP",servicesTitle:'Services & <span class="gold">Solutions.</span>',servicesIntro:"Areas I can help with as my skills develop. Contact me to discuss your specific needs.",
service1Title:"Website Development",service1Text:"Modern responsive websites designed to work across mobile and desktop screens.",service1a:"Landing pages",service1b:"Personal portfolios",service1c:"Responsive layouts",
service2Title:"Website UI & Styling",service2Text:"Clean interfaces with thoughtful typography, layout, and subtle visual details.",service2a:"Dark and light themes",service2b:"Interactive components",service2c:"Mobile-friendly design",
service3Title:"Programming Projects",service3Text:"Small programming tasks and prototypes with a focus on clarity and maintainability.",service3a:"Basic scripting",service3b:"Website improvements",service3c:"Learning prototypes",
contactKicker:"START A CONVERSATION",contactTitle:'Let\\'s build something <span class="gold">good.</span>',contactIntro:"Have a website idea, a question, or a project to discuss? Use the form to prepare a message.",
contactCardTitle:"Get in touch",contactCardText:"You can also find my public programming profile here.",websiteLabel:"Website",nameLabel:"Your name",emailLabel:"Your email (optional)",messageLabel:"Your message",sendMessage:"Prepare Message",formNote:"This form opens your email app to send the message. It does not send or store messages by itself.",footerText:"Made with care.",backTop:"Back to top ↑",
namePlaceholder:"Name",emailPlaceholder:"you@example.com",messagePlaceholder:"Tell me about your idea...",missingEmail:"Your email app could not be opened. Please copy your message and contact me through GitHub.",toastReady:"Your message is ready in your email app."
},
ar:{
navAbout:"عني",navSkills:"مهاراتي",navProjects:"مشاريعي",navServices:"خدماتي",navContact:"تواصل معي",
eyebrow:"الموقع الشخصي للمبرمج",hello:"أهلًا، أنا",heroText:"أصمم تجارب رقمية مميزة ومواقع عصرية وواجهات مرتبة، مع الاهتمام بالتفاصيل وسهولة الاستخدام.",
viewWork:"استكشف أعمالي",contactMe:"تواصل معي",metaSkills:"تقنيات",metaFocus:"مجال التطوير",metaIdeas:"أفكار للتنفيذ",
aboutKicker:"نبذة عني",aboutTitle:'أبني بشغف <span class="gold">وهدف.</span>',aboutIntro:"تعرف على طريقتي في البرمجة وما أطمح إلى تنفيذه.",
aboutCardTitle:"أهلًا، أنا أرساني.",aboutText:"أنا مبرمج مهتم بتطوير الويب والتكنولوجيا وإنشاء تجارب رقمية مفيدة. أحب التعلم وتجربة الأكواد وتحويل الأفكار إلى واجهات واضحة ومتجاوبة. هذا الموقع هو مساحتي على الإنترنت لعرض مهاراتي وأعمالي القادمة.",aboutText2:"أهتم بالتعلم المستمر والتصميم البسيط وسهولة الوصول، وإنشاء مواقع تعمل بشكل جيد على مختلف أحجام الشاشات.",
quickFacts:"معلومات سريعة",factRole:"الدور",factRoleValue:"مبرمج",factInterest:"الاهتمام الأساسي",factInterestValue:"تطوير الويب",factApproach:"الأسلوب",factApproachValue:"تعلّم وتنفيذ",factGoal:"الهدف",factGoalValue:"تجارب مفيدة",
skillsKicker:"الأدوات والتقنيات",skillsTitle:'مهاراتي <span class="gold">وتقنياتي.</span>',skillsIntro:"تقنيات أتعلمها وأستكشفها في رحلتي البرمجية، دون المبالغة في مستوى المهارات.",
htmlText:"بناء هيكل صفحات الويب بطريقة منظمة.",cssText:"تنسيق الصفحات والتصميم المتجاوب.",jsText:"إضافة التفاعل والحركة إلى المواقع.",pythonText:"أساسيات المنطق البرمجي وكتابة السكريبتات.",phpText:"أساسيات البرمجة من جهة الخادم.",reactText:"إنشاء الواجهات باستخدام المكونات.",
projectsKicker:"نماذج وأفكار",projectsTitle:'مشاريع <span class="gold">وتجارب.</span>',projectsIntro:"بعض نماذج المشاريع والأفكار. استبدلها بمشاريعك الحقيقية عند نشرها.",
project1Title:"الموقع الشخصي",project1Text:"موقع شخصي متجاوب بلغتين، بتصميم داكن أنيق وتنقل سلس.",project1Link:"استكشف الموقع ↗",
project2Title:"واجهة موقع تجاري",project2Text:"تصور لموقع تجاري منظم يعرض الخدمات وأزرار التواصل ويتناسب مع الموبايل.",project2Link:"ناقش فكرة مشابهة ↗",
project3Title:"تجربة ويب تفاعلية",project3Text:"مشروع تعليمي يركز على التفاعل وسهولة الاستخدام وتجربة الزائر.",project3Link:"زر حسابي على GitHub ↗",
projectNote:"ملحوظة: البطاقة الأولى تفتح هذا الموقع، أما البطاقتان الأخريان فهما أفكار تجريبية وليستا أعمالًا تجارية مكتملة.",
servicesKicker:"كيف يمكنني المساعدة",servicesTitle:'خدمات <span class="gold">وحلول.</span>',servicesIntro:"مجالات أعمل على تطوير مهاراتي فيها. تواصل معي لمناقشة احتياجاتك.",
service1Title:"تطوير المواقع",service1Text:"مواقع عصرية متجاوبة تعمل على الموبايل والكمبيوتر.",service1a:"صفحات تعريفية",service1b:"مواقع شخصية",service1c:"تصميم متجاوب",
service2Title:"تصميم واجهات المواقع",service2Text:"واجهات مرتبة مع خطوط مناسبة وتنسيق وتفاصيل بصرية بسيطة.",service2a:"أنماط داكنة وفاتحة",service2b:"عناصر تفاعلية",service2c:"تصميم مناسب للموبايل",
service3Title:"مشاريع برمجية",service3Text:"مهام ونماذج برمجية صغيرة مع الاهتمام بوضوح الكود وسهولة تطويره.",service3a:"سكريبتات بسيطة",service3b:"تحسين المواقع",service3c:"مشاريع للتعلم",
contactKicker:"ابدأ محادثة",contactTitle:'لنبنِ شيئًا <span class="gold">مميزًا.</span>',contactIntro:"عندك فكرة موقع أو سؤال أو مشروع؟ استخدم النموذج لتجهيز رسالة.",
contactCardTitle:"تواصل معي",contactCardText:"يمكنك أيضًا زيارة حسابي البرمجي العام هنا.",websiteLabel:"الموقع",nameLabel:"اسمك",emailLabel:"بريدك الإلكتروني (اختياري)",messageLabel:"رسالتك",sendMessage:"تجهيز الرسالة",formNote:"النموذج يفتح تطبيق البريد لإرسال الرسالة، ولا يرسل أو يخزن الرسائل بنفسه.",footerText:"صُنع بعناية.",backTop:"العودة للأعلى ↑",
namePlaceholder:"اكتب اسمك",emailPlaceholder:"you@example.com",messagePlaceholder:"اكتب فكرتك هنا...",missingEmail:"تعذر فتح تطبيق البريد. انسخ رسالتك وتواصل معي عبر GitHub.",toastReady:"تم تجهيز رسالتك في تطبيق البريد."
}
};
let currentLang="en";
const langBtn=document.getElementById("langBtn");
const navlinks=document.getElementById("navlinks");
function setLanguage(lang){
 currentLang=lang;
 const dict=translations[lang];
 document.documentElement.lang=lang;
 document.documentElement.dir=lang==="ar"?"rtl":"ltr";
 document.querySelectorAll("[data-i18n]").forEach(el=>{
  const key=el.dataset.i18n;
  if(dict[key]!==undefined)el.innerHTML=dict[key];
 });
 document.getElementById("name").placeholder=dict.namePlaceholder;
 document.getElementById("email").placeholder=dict.emailPlaceholder;
 document.getElementById("message").placeholder=dict.messagePlaceholder;
 langBtn.textContent=lang==="en"?"العربية":"English";
 document.title=lang==="ar"?"أرساني ورسي | الموقع الشخصي":"Arsaney Warsey | Developer Portfolio";
 try{localStorage.setItem("arsaney-language",lang)}catch(e){}
}
langBtn.addEventListener("click",()=>setLanguage(currentLang==="en"?"ar":"en"));
document.getElementById("menuBtn").addEventListener("click",()=>navlinks.classList.toggle("open"));
navlinks.querySelectorAll("a").forEach(a=>a.addEventListener("click",()=>navlinks.classList.remove("open")));
document.getElementById("year").textContent=new Date().getFullYear();
const toast=document.getElementById("toast");
function showToast(msg){toast.textContent=msg;toast.classList.add("show");setTimeout(()=>toast.classList.remove("show"),4500)}
document.getElementById("contactForm").addEventListener("submit",function(e){
 e.preventDefault();
 const dict=translations[currentLang];
 const name=document.getElementById("name").value.trim();
 const email=document.getElementById("email").value.trim();
 const message=document.getElementById("message").value.trim();
 if(!name||!message)return;
 const subject=encodeURIComponent("Portfolio contact from "+name);
 const body=encodeURIComponent(message+"\n\nFrom: "+name+(email?"\nEmail: "+email:""));
 const mailto="mailto:?subject="+subject+"&body="+body;
 window.location.href=mailto;
 showToast(dict.toastReady);
});
try{
 const saved=localStorage.getItem("arsaney-language");
 if(saved==="ar")setLanguage("ar");
}catch(e){}
</script>
</body>
</html>

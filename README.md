* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

:root {
  --bg: #050505;
  --panel: #0b0b0b;
  --text: #f4f4f4;
  --muted: #8d8d8d;
  --line: #242424;
  --accent: #ffffff;
  --accent-dark: #151515;
}

html {
  scroll-behavior: smooth;
}

body {
  background: var(--bg);
  color: var(--text);
  font-family: "Inter", sans-serif;
  line-height: 1.6;
}

a {
  color: inherit;
  text-decoration: none;
}

.sidebar {
  position: fixed;
  inset: 0 auto 0 0;
  width: 245px;
  background: #080808;
  border-right: 1px solid var(--line);
  padding: 34px 25px;
  display: flex;
  flex-direction: column;
  z-index: 100;
}

.brand {
  display: flex;
  align-items: center;
  gap: 11px;
  font-size: 20px;
  font-weight: 900;
  letter-spacing: 2px;
}

.brand span:last-child span,
.footer-brand span {
  color: #777;
}

.brand-mark {
  border: 1px solid #fff;
  padding: 5px 8px;
  font-size: 13px;
}

.nav-menu {
  display: flex;
  flex-direction: column;
  gap: 7px;
  margin-top: 75px;
}

.nav-menu a {
  padding: 14px 13px;
  color: #777;
  border-left: 2px solid transparent;
  transition: .25s;
}

.nav-menu a:hover,
.nav-menu a.active {
  color: #fff;
  border-left-color: #fff;
  background: #111;
}

.nav-menu a span {
  margin-left: 12px;
}

.sidebar-bottom {
  margin-top: auto;
  color: #777;
  font-size: 13px;
}

.sidebar-bottom strong {
  color: #fff;
}

.side-whatsapp {
  display: block;
  margin-top: 17px;
  border: 1px solid #444;
  padding: 11px 12px;
  text-align: center;
  transition: .25s;
}

.side-whatsapp:hover {
  background: #fff;
  color: #000;
}

main {
  margin-left: 245px;
}

.section {
  min-height: 100vh;
  padding: 110px 8%;
  border-bottom: 1px solid var(--line);
  position: relative;
  overflow: hidden;
}

.hero {
  min-height: 100vh;
  display: flex;
  align-items: center;
}

.code-bg {
  position: absolute;
  inset: 0 0 auto auto;
  width: 53%;
  height: 100%;
  opacity: .13;
  pointer-events: none;
  overflow: hidden;
}

.code-bg pre {
  font: 14px/2 monospace;
  padding: 80px 40px;
  transform: rotate(-3deg);
}

.hero-content {
  max-width: 800px;
  position: relative;
  z-index: 2;
}

.eyebrow,
.section-label {
  color: #777;
  font-size: 11px;
  font-weight: 700;
  letter-spacing: 3px;
}

.hero h1 {
  font-size: clamp(55px, 8vw, 115px);
  line-height: .92;
  letter-spacing: -6px;
  margin: 25px 0;
}

.hero h1 span,
h2 span {
  color: #777;
}

.hero-text {
  color: #aaa;
  max-width: 620px;
  font-size: 17px;
}

.hero-text strong {
  color: #fff;
}

.hero-buttons {
  display: flex;
  gap: 12px;
  margin-top: 35px;
  flex-wrap: wrap;
}

.btn {
  padding: 14px 20px;
  border: 1px solid #444;
  font-weight: 700;
}

.btn.primary {
  background: #fff;
  color: #000;
}

.btn.ghost:hover {
  background: #fff;
  color: #000;
}

.world-grid {
  position: absolute;
  right: 7%;
  bottom: 35px;
  color: #333;
  font: 11px monospace;
  letter-spacing: 3px;
}

h2 {
  font-size: clamp(42px, 6vw, 78px);
  line-height: 1;
  letter-spacing: -3px;
  margin: 25px 0 55px;
}

.two-column,
.skills-layout {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 80px;
  align-items: start;
}

.large-text {
  font-size: 27px;
  line-height: 1.35;
  margin-bottom: 25px;
}

.two-column p:not(.large-text) {
  color: var(--muted);
  max-width: 600px;
}

.service-grid {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 14px;
}

.card {
  border: 1px solid var(--line);
  padding: 25px;
  min-height: 310px;
  background: linear-gradient(145deg, #0d0d0d, #060606);
  transition: .3s;
}

.card:hover {
  transform: translateY(-7px);
  border-color: #666;
}

.card-number {
  color: #555;
  font: 12px monospace;
}

.icon {
  font-size: 38px;
  margin: 55px 0 20px;
}

.card h3 {
  font-size: 20px;
  margin-bottom: 10px;
}

.card p {
  color: var(--muted);
  font-size: 14px;
}

.skill-list > div {
  display: flex;
  justify-content: space-between;
  padding: 19px 0;
  border-bottom: 1px solid var(--line);
  font-weight: 700;
}

.skill-list b {
  color: #555;
  font: 12px monospace;
}

.work-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 15px;
}

.work-card {
  min-height: 350px;
  padding: 25px;
  border: 1px solid var(--line);
  display: flex;
  flex-direction: column;
  justify-content: flex-end;
  background:
    linear-gradient(145deg, transparent 35%, #111 100%);
}

.work-card span {
  color: #555;
  font: 12px monospace;
  margin-bottom: auto;
}

.work-card h3 {
  font-size: 25px;
}

.work-card p {
  color: #777;
}

.contact {
  min-height: 75vh;
}

.contact > p {
  max-width: 600px;
  color: #888;
  margin-top: -25px;
}

.contact-whatsapp {
  margin-top: 35px;
  width: min(620px, 100%);
  padding: 22px;
  border: 1px solid #444;
  display: flex;
  justify-content: space-between;
  gap: 15px;
  align-items: center;
}

.contact-whatsapp:hover {
  background: #fff;
  color: #000;
}

footer {
  padding: 50px 8%;
  display: grid;
  grid-template-columns: 1.4fr 1fr 1fr;
  gap: 30px;
  color: #777;
}

.footer-brand {
  font-size: 23px;
  color: #fff;
  font-weight: 900;
  letter-spacing: 3px;
}

.socials {
  display: flex;
  flex-direction: column;
  gap: 7px;
}

.socials a:hover,
.footer-user strong {
  color: #fff;
}

.footer-user {
  display: flex;
  flex-direction: column;
}

.footer-user small {
  font-size: 9px;
  letter-spacing: 2px;
}

.copyright {
  grid-column: 1 / -1;
  border-top: 1px solid var(--line);
  padding-top: 20px;
  font-size: 12px;
}

/* Mobile */
@media (max-width: 900px) {
  .sidebar {
    width: 100%;
    height: 70px;
    padding: 12px 18px;
    flex-direction: row;
    align-items: center;
    border-right: 0;
    border-bottom: 1px solid var(--line);
  }

  .nav-menu {
    flex-direction: row;
    margin: 0 0 0 auto;
    gap: 2px;
  }

  .nav-menu a {
    padding: 9px;
    border-left: 0;
  }

  .nav-menu a span,
  .sidebar-bottom {
    display: none;
  }

  main {
    margin-left: 0;
    padding-top: 70px;
  }

  .section {
    padding: 80px 6%;
  }

  .service-grid {
    grid-template-columns: 1fr 1fr;
  }

  .work-grid {
    grid-template-columns: 1fr;
  }

  footer {
    grid-template-columns: 1fr 1fr;
  }
}

@media (max-width: 600px) {
  .brand {
    font-size: 16px;
  }

  .nav-menu a {
    font-size: 12px;
  }

  .hero h1 {
    letter-spacing: -3px;
  }

  .two-column,
  .skills-layout,
  .service-grid {
    grid-template-columns: 1fr;
    gap: 35px;
  }

  .large-text {
    font-size: 22px;
  }

  .contact-whatsapp {
    flex-direction: column;
    align-items: flex-start;
  }

  footer {
    grid-template-columns: 1fr;
  }
}

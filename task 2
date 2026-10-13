<!doctype html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width,initial-scale=1">
<meta name="theme-color" content="#f4f2ed">
<title>Tracko — Mobile App Prototype</title>
<style>
@import url('https://fonts.googleapis.com/css2?family=DM+Mono:wght@400;500&family=Space+Grotesk:wght@400;500;600;700&display=swap');

:root {
  --ink: #11110f;
  --paper: #f4f2ed;
  --white: #fffefa;
  --purple: #9673ff;
  --yellow: #e8f833;
  --muted: #77756e;
  --line: #dedbd3;
}

* { box-sizing: border-box; }
body {
  margin: 0;
  background: var(--paper);
  color: var(--ink);
  font-family: 'Space Grotesk', Arial, sans-serif;
}
.top {
  max-width: 1200px;
  margin: auto;
  padding: 22px 28px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  border-bottom: 1px solid var(--line);
}
.brand {
  font-weight: 700;
  font-size: 21px;
  letter-spacing: -1.4px;
  display: flex;
  align-items: center;
  gap: 10px;
}
.mark {
  width: 32px;
  height: 32px;
  display: grid;
  place-items: center;
  background: var(--yellow);
  border: 1.5px solid var(--ink);
  box-shadow: 3px 3px var(--ink);
  font-size: 19px;
}
.top small, .mono {
  font-family: 'DM Mono', monospace;
  font-size: 11px;
  letter-spacing: .04em;
  text-transform: uppercase;
  color: var(--muted);
}
.layout {
  max-width: 1200px;
  margin: 0 auto;
  padding: 54px 28px 70px;
  display: grid;
  grid-template-columns: .9fr 1.1fr;
  gap: 60px;
  align-items: center;
}
.intro { max-width: 440px; }
.tag {
  display: inline-block;
  padding: 7px 9px;
  background: var(--purple);
  border: 1.5px solid var(--ink);
  box-shadow: 3px 3px var(--ink);
  font: 10px 'DM Mono', monospace;
  text-transform: uppercase;
  letter-spacing: .05em;
}
.intro h1 {
  font-size: clamp(45px, 6.5vw, 78px);
  line-height: .92;
  letter-spacing: -.075em;
  margin: 24px 0 18px;
}
.intro h1 em {
  font-style: normal;
  background: var(--yellow);
  padding: 0 .04em;
}
.intro p {
  color: #5e5c55;
  font-size: 16px;
  line-height: 1.7;
  margin: 0 0 23px;
}
.bullets {
  display: grid;
  gap: 10px;
  margin-top: 29px;
}
.bullet {
  display: flex;
  align-items: center;
  gap: 12px;
  font-size: 13px;
}
.bullet b {
  display: grid;
  place-items: center;
  width: 25px;
  height: 25px;
  background: var(--white);
  border: 1px solid var(--ink);
  font-size: 12px;
}
.device-stage {
  position: relative;
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 14px;
  padding: 23px 16px 30px;
  overflow: hidden;
}
.device-stage::before {
  content: '';
  position: absolute;
  inset: 4% 6%;
  background: var(--yellow);
  border: 1px solid var(--ink);
  transform: rotate(-2deg);
}
.phone {
  position: relative;
  width: 220px;
  height: 452px;
  background: var(--white);
  border: 2px solid var(--ink);
  border-radius: 27px;
  box-shadow: 4px 5px 0 var(--ink);
  padding: 13px 12px 12px;
  overflow: hidden;
  display: flex;
  flex-direction: column;
  transition: transform .2s;
}
.phone:nth-child(1), .phone:nth-child(3) {
  transform: translateY(12px) scale(.91);
}
.phone:nth-child(2) { z-index: 2; }
.phone:hover { transform: translateY(-5px) scale(1); }
.notch {
  position: absolute;
  top: 6px;
  left: 50%;
  transform: translateX(-50%);
  width: 43px;
  height: 11px;
  border-radius: 0 0 9px 9px;
  background: var(--ink);
}
.screen-head {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-top: 9px;
  margin-bottom: 18px;
  font-size: 13px;
  font-weight: 700;
}
.screen-head .back {
  font-size: 20px;
  line-height: 1;
  display: grid;
  place-items: center;
  width: 22px;
  height: 22px;
  background: var(--yellow);
  border: 1px solid var(--ink);
}
.screen-head .dots { font-size: 18px; }
.sub {
  font-size: 9px;
  color: var(--muted);
  margin-top: -16px;
  margin-bottom: 13px;
}
.filters {
  display: flex;
  gap: 5px;
  margin-bottom: 12px;
}
.pill {
  font-size: 8px;
  padding: 5px 6px;
  border: 1px solid var(--ink);
  background: var(--white);
}
.pill.active { background: var(--purple); font-weight: 700; }
.task {
  border: 1px solid var(--ink);
  padding: 10px 8px;
  display: flex;
  align-items: center;
  gap: 8px;
  margin-bottom: 7px;
  font-size: 9px;
}
.check {
  flex: none;
  width: 13px;
  height: 13px;
  border: 1px solid var(--ink);
  display: grid;
  place-items: center;
  background: var(--yellow);
  font-size: 9px;
}
.task small {
  display: block;
  color: var(--muted);
  font-size: 7px;
  margin-top: 3px;
}
.date {
  font: 7px 'DM Mono', monospace;
  margin-left: auto;
  padding: 4px;
  background: #eee9ff;
}
.chart {
  height: 104px;
  background: var(--purple);
  border: 1px solid var(--ink);
  padding: 10px;
  margin-bottom: 10px;
  display: flex;
  align-items: end;
  justify-content: space-around;
  gap: 6px;
}
.bar {
  width: 22px;
  background: var(--yellow);
  border: 1px solid var(--ink);
}
.bar:nth-child(1) { height: 30%; }
.bar:nth-child(2) { height: 55%; }
.bar:nth-child(3) { height: 42%; }
.bar:nth-child(4) { height: 78%; }
.bar:nth-child(5) { height: 100%; }
.statrow {
  padding: 9px;
  border: 1px solid var(--ink);
  font-size: 8px;
  display: flex;
  justify-content: space-between;
  margin-bottom: 7px;
}
.ring {
  width: 43px;
  height: 43px;
  border-radius: 50%;
  border: 5px solid var(--yellow);
  border-right-color: var(--ink);
  display: grid;
  place-items: center;
  font-size: 10px;
  font-weight: 700;
}
.mood {
  background: #f8f6ee;
  border: 1px solid var(--ink);
  padding: 9px;
  font-size: 8px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.mood b { font-size: 18px; }
.phone-nav {
  display: flex;
  justify-content: space-around;
  align-items: center;
  margin-top: auto;
  padding-top: 9px;
  border-top: 1px solid var(--line);
  font-size: 13px;
}
.phone-nav span {
  width: 24px;
  height: 24px;
  display: grid;
  place-items: center;
}
.phone-nav .selected {
  background: var(--purple);
  border: 1px solid var(--ink);
}
.screenlabel {
  position: absolute;
  top: 0;
  left: 50%;
  transform: translateX(-50%);
  z-index: 3;
  background: var(--ink);
  color: var(--white);
  font: 9px 'DM Mono', monospace;
  letter-spacing: .1em;
  padding: 7px 10px;
  text-transform: uppercase;
}
.footer {
  max-width: 1200px;
  margin: auto;
  padding: 18px 28px;
  border-top: 1px solid var(--line);
  display: flex;
  justify-content: space-between;
  color: var(--muted);
  font: 10px 'DM Mono', monospace;
}
.prototype {
  max-width: 1200px;
  margin: -16px auto 42px;
  padding: 0 28px;
}
.prototype button {
  border: 1px solid var(--ink);
  background: var(--yellow);
  padding: 10px 14px;
  font: 11px 'DM Mono', monospace;
  text-transform: uppercase;
  cursor: pointer;
}
.prototype-note {
  font-size: 12px;
  color: var(--muted);
  margin-left: 12px;
}
.toast {
  position: fixed;
  bottom: 22px;
  left: 50%;
  transform: translate(-50%, 15px);
  opacity: 0;
  transition: .2s;
  background: var(--ink);
  color: white;
  padding: 12px 16px;
  font-size: 12px;
  pointer-events: none;
}
.toast.show {
  opacity: 1;
  transform: translate(-50%, 0);
}

@media (max-width: 960px) {
  .layout { grid-template-columns: 1fr; gap: 30px; padding-top: 40px; }
  .intro { max-width: 630px; }
  .device-stage { max-width: 680px; width: 100%; margin: auto; }
  .phone { width: min(29vw, 220px); }
  .phone:nth-child(1), .phone:nth-child(3) {
    transform: translateY(12px) scale(.95);
  }
}
@media (max-width: 580px) {
  .top { padding: 16px; }
  .top small { font-size: 9px; }
  .layout { padding: 30px 16px 45px; }
  .intro h1 { font-size: 54px; }
  .intro p { font-size: 14px; }
  .device-stage { gap: 7px; padding: 24px 0 25px; }
  .phone {
    width: 31vw;
    height: 390px;
    padding: 12px 8px 9px;
    border-radius: 21px;
  }
  .phone:nth-child(1), .phone:nth-child(3) {
    transform: translateY(10px) scale(.95);
  }
  .screen-head { font-size: 10px; margin-bottom: 14px; }
  .task { padding: 7px 5px; font-size: 7px; gap: 5px; }
  .task small { font-size: 6px; }
  .date { font-size: 6px; padding: 3px; }
  .chart { height: 86px; padding: 7px; }
  .bar { width: 15px; }
  .statrow, .mood { font-size: 7px; padding: 6px; }
  .ring { width: 34px; height: 34px; font-size: 8px; }
  .phone-nav { font-size: 11px; }
  .phone-nav span { width: 20px; height: 20px; }
  .prototype { padding: 0 16px; }
  .prototype-note { display: block; margin: 10px 0 0; }
  .footer { padding: 15px 16px; gap: 10px; flex-wrap: wrap; }
  .screenlabel { font-size: 8px; }
}
</style>
</head>
<body>
<header class="top">
  <a class="brand" href="#"><span class="mark">✳</span> tracko</a>
  <small>Mobile app concept · task management</small>
</header>

<main class="layout">
  <section class="intro">
    <span class="tag">UI / UX design · concept 01</span>
    <h1>Make time for <em>what matters.</em></h1>
    <p>
      Tracko turns your to-do list into a calm, clear plan. Organize your work,
      see your progress, and keep moving at your own pace.
    </p>
    <div class="bullets">
      <div class="bullet"><b>✓</b><span>Know what to focus on next</span></div>
      <div class="bullet"><b>▥</b><span>See progress without the noise</span></div>
      <div class="bullet"><b>✳</b><span>Build a routine that works for you</span></div>
    </div>
  </section>

  <section class="device-stage" aria-label="Three mobile app screens">
    <span class="screenlabel">A little more organized</span>

    <div class="phone">
      <span class="notch"></span>
      <div class="screen-head">Hello, Alex! <span class="back">♧</span></div>
      <div class="sub">What would you like to do today?</div>
      <div class="task" style="background:var(--yellow)">
        <span class="check">✓</span>
        <span><b>My Tasks</b><small>2 tasks due today</small></span>
        <span style="margin-left:auto">→</span>
      </div>
      <div class="task" style="background:var(--purple)">
        <span>▦</span>
        <span><b>Calendar</b><small>Plan your schedule</small></span>
        <span style="margin-left:auto">→</span>
      </div>
      <div class="task">
        <span>▥</span>
        <span><b>Statistics</b><small>Track your progress</small></span>
        <span style="margin-left:auto">→</span>
      </div>
      <div class="task">
        <span>⚙</span>
        <span><b>Settings</b><small>Manage preferences</small></span>
        <span style="margin-left:auto">→</span>
      </div>
      <div class="phone-nav">
        <span class="selected">⌂</span><span>▥</span><span>＋</span><span>✉</span><span>♙</span>
      </div>
    </div>

    <div class="phone">
      <span class="notch"></span>
      <div class="screen-head">
        <span style="display:flex;gap:7px;align-items:center">
          <span class="back">←</span> My Tasks
        </span>
        <span class="dots">⋮</span>
      </div>
      <div class="filters">
        <span class="pill">All</span><span class="pill active">In Progress</span><span class="pill">Completed</span>
      </div>
      <div class="task">
        <span class="check">✓</span><span><b>UX Research</b><small>Study interviews and insights</small></span>
        <span class="date">May 20</span>
      </div>
      <div class="task">
        <span class="check"></span><span><b>Wireframe</b><small>Create flow for dashboard</small></span>
        <span class="date">May 22</span>
      </div>
      <div class="task">
        <span class="check"></span><span><b>UI Design</b><small>High-fidelity screens in Figma</small></span>
        <span class="date">May 24</span>
      </div>
      <div class="task">
        <span class="check"></span><span><b>Prototype</b><small>Interactive review</small></span>
        <span class="date">May 26</span>
      </div>
      <div class="phone-nav">
        <span>⌂</span><span>▥</span><span class="selected">＋</span><span>✉</span><span>♙</span>
      </div>
    </div>

    <div class="phone">
      <span class="notch"></span>
      <div class="screen-head">
        <span style="display:flex;gap:7px;align-items:center">
          <span class="back">←</span> Statistics
        </span>
        <span class="dots">⋮</span>
      </div>
      <div class="filters">
        <span class="pill" style="width:100%;display:flex;justify-content:space-between">
          This week <b>⌄</b>
        </span>
      </div>
      <div class="chart">
        <i class="bar"></i><i class="bar"></i><i class="bar"></i><i class="bar"></i><i class="bar"></i>
      </div>
      <div class="statrow"><span>Tasks completed</span><b>18</b></div>
      <div class="statrow" style="align-items:center">
        <span>Task progress</span><span class="ring">75%</span>
      </div>
      <div class="mood">
        <span><b>Productivity</b><br><small>Good work this week!</small></span><b>☺</b>
      </div>
      <div class="phone-nav">
        <span>⌂</span><span class="selected">▥</span><span>＋</span><span>✉</span><span>♙</span>
      </div>
    </div>
  </section>
</main>

<div class="prototype">
  <button id="flow">Preview interaction flow ↗</button>
  <span class="prototype-note">Tap to cycle through Home → Tasks → Statistics.</span>
</div>

<footer class="footer">
  <span>TRACKO · CONCEPT DESIGN</span>
  <span>Simple plans. Steady progress.</span>
</footer>
<div class="toast" role="status" aria-live="polite"></div>

<script>
  const flow = document.querySelector('#flow');
  const phones = [...document.querySelectorAll('.phone')];
  const toast = document.querySelector('.toast');
  let step = 0;

  flow.addEventListener('click', () => {
    step = (step + 1) % 3;
    phones.forEach((phone, index) => {
      phone.style.outline = index === step ? '3px solid var(--yellow)' : 'none';
    });
    toast.textContent = [
      'Home screen selected',
      'Task list selected',
      'Statistics screen selected'
    ][step];
    toast.classList.add('show');
    clearTimeout(window.toastTimer);
    window.toastTimer = setTimeout(() => toast.classList.remove('show'), 1400);
  });
</script>
</body>
</html>

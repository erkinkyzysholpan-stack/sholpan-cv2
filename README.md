<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Sholpan Shabdenbek, CV</title>
  <meta name="description" content="CV of Sholpan Shabdenbek: geography student at Eurasian National University, English tutor and volunteer from Astana, Kazakhstan.">
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Big+Shoulders+Display:wght@700;900&family=Figtree:wght@400;500;600&display=swap" rel="stylesheet">
  <style>
    :root {
      --white: #eef3ee;     /* soft sage mist */
      --black: #23393a;     /* deep slate teal instead of black */
      --blue: #3f6f73;      /* calm muted teal accent */
      --grey: #dbe7de;      /* pale sage */
      --sand: #e9dcc3;      /* warm sand */
      --muted: #5a6e6c;
      --display: "Big Shoulders Display", "Arial Narrow", Impact, sans-serif;
      --body: "Figtree", "Segoe UI", Helvetica, Arial, sans-serif;
    }
    * { box-sizing: border-box; margin: 0; padding: 0; }
    html { scroll-behavior: smooth; }
    body { font-family: var(--body); background: var(--white); color: var(--black); line-height: 1.65; font-size: 1.05rem; overflow-x: hidden; }
    a { color: inherit; }
    :focus-visible { outline: 3px solid var(--blue); outline-offset: 3px; }
    .wrap { max-width: 1120px; margin: 0 auto; padding: 0 24px; }

    /* ---------- First page ---------- */
    .hero { position: relative; padding-bottom: 56px; }
    .topbar { display: flex; justify-content: space-between; align-items: center; gap: 20px; padding-top: 24px; padding-bottom: 8px; }
    .topbar .mark { font-family: var(--display); font-weight: 900; font-size: 1.5rem; text-decoration: none; letter-spacing: .01em; white-space: nowrap; flex: none; }
    .topbar nav { display: flex; gap: 22px; overflow-x: auto; scrollbar-width: none; min-width: 0; }
    .topbar nav::-webkit-scrollbar { display: none; }
    .topbar nav a { text-decoration: none; font-size: .95rem; font-weight: 500; white-space: nowrap; border-bottom: 2px solid transparent; padding: 3px 0; }
    .topbar nav a:hover { border-bottom-color: var(--blue); }

    .hero h1 { font-family: var(--display); font-weight: 900; font-size: clamp(5.2rem, 24vw, 17rem); line-height: .8; letter-spacing: -.01em; margin-top: 28px; }
    .hero h1 span { display: block; }
    .hero h1 span + span { color: var(--blue); }
    .sticker { position: absolute; right: max(24px, calc((100vw - 1120px) / 2 + 24px)); top: 150px; background: var(--sand); color: var(--black); padding: 14px 20px; transform: rotate(7deg); font-family: var(--display); font-weight: 900; font-size: clamp(1.1rem, 3vw, 1.8rem); line-height: 1.05; text-align: center; border-radius: 6px; }

    .hero-low { display: grid; grid-template-columns: 1fr auto; align-items: end; gap: 32px; margin-top: 40px; }
    .hero .lede { max-width: 30rem; font-size: 1.25rem; font-weight: 500; }
    .facts { display: flex; flex-wrap: wrap; gap: 10px; margin-top: 22px; }
    .facts span { border: 2px solid var(--black); border-radius: 999px; padding: 4px 16px; font-size: .95rem; font-weight: 500; }
    .btn { display: inline-block; margin-top: 26px; background: var(--black); color: #fff; font-weight: 600; text-decoration: none; padding: 14px 28px; border-radius: 999px; transition: background .2s ease; }
    .btn:hover { background: var(--blue); }
    .photo { width: 210px; aspect-ratio: 4 / 5; background: var(--grey); border-radius: 6px; overflow: hidden; transform: rotate(-3deg); border: 3px solid var(--black); }
    .photo img { width: 100%; height: 100%; object-fit: cover; display: block; }

    /* skills marquee */
    .marquee { background: var(--black); color: #fff; overflow: hidden; padding: 16px 0; }
    .track { display: flex; width: max-content; animation: slide 32s linear infinite; }
    .track span { font-family: var(--display); font-weight: 900; font-size: clamp(1.6rem, 4vw, 2.4rem); padding: 0 22px; white-space: nowrap; }
    .track span.sep { color: var(--sand); padding: 0; }
    @keyframes slide { to { transform: translateX(-50%); } }

    /* ---------- Sections ---------- */
    section { padding: 88px 0 0; }
    .row { display: grid; grid-template-columns: 220px 1fr; gap: 14px 40px; }
    .row > h2 { font-family: var(--display); font-weight: 900; font-size: 2.6rem; line-height: .95; position: sticky; top: 24px; align-self: start; }
    .row > h2::after { content: ""; display: block; width: 52px; height: 8px; background: var(--blue); margin-top: 12px; }

    .about { font-size: clamp(1.5rem, 3.4vw, 2.2rem); font-weight: 600; line-height: 1.3; max-width: 36rem; letter-spacing: -.01em; }
    .about mark { background: var(--blue); color: #fff; padding: 0 .25em; }

    .entry { display: grid; grid-template-columns: 130px 1fr; gap: 4px 24px; padding: 24px 16px; margin: 0 -16px; border-top: 2px solid var(--black); transition: background .2s ease, color .2s ease; }
    .entry:last-child { border-bottom: 2px solid var(--black); }
    .entry:hover { background: var(--blue); color: #fff; }
    .entry .when { font-size: .95rem; font-weight: 500; padding-top: 6px; }
    .entry h3 { font-family: var(--display); font-weight: 900; font-size: 1.9rem; line-height: 1.05; }
    .entry .where { font-weight: 600; color: var(--blue); margin: 4px 0 8px; transition: color .2s ease; }
    .entry:hover .where { color: #fff; }
    .entry p, .entry li { max-width: 34rem; }
    .entry ul { padding-left: 1.1rem; }

    .big-skills { list-style: none; }
    .big-skills li { font-family: var(--display); font-weight: 900; font-size: clamp(2.8rem, 9vw, 6rem); line-height: .95; transition: color .2s ease; }
    .big-skills li:hover { color: var(--blue); }
    .chips { display: flex; flex-wrap: wrap; gap: 10px; margin-top: 28px; list-style: none; }
    .chips li { background: var(--grey); padding: 6px 16px; border-radius: 999px; font-weight: 500; }

    .langs { display: grid; grid-template-columns: repeat(auto-fit, minmax(160px, 1fr)); gap: 18px; }
    .lang { border-top: 8px solid var(--black); padding-top: 12px; }
    .lang:nth-child(3) { border-top-color: var(--blue); }
    .lang b { display: block; font-family: var(--display); font-weight: 900; font-size: 2.4rem; line-height: 1; }
    .lang span { color: var(--muted); }

    /* ---------- Contact ---------- */
    .contact { background: var(--black); color: var(--white); margin-top: 110px; padding: 90px 0 36px; }
    .contact h2 { font-family: var(--display); font-weight: 900; font-size: clamp(4rem, 17vw, 11rem); line-height: .85; }
    .contact a.mail { display: inline-block; margin-top: 28px; background: var(--sand); color: var(--black); font-weight: 600; font-size: clamp(1rem, 3.4vw, 1.5rem); padding: 14px 26px; border-radius: 999px; text-decoration: none; word-break: break-all; transition: background .2s ease, color .2s ease; }
    .contact a.mail:hover { background: var(--blue); color: #fff; }
    .contact small { display: block; margin-top: 70px; opacity: .8; font-size: .9rem; }

    @media (max-width: 800px) {
      .sticker { top: 120px; }
      .hero-low { grid-template-columns: 1fr; }
      .photo { width: 150px; order: -1; }
      .row { grid-template-columns: 1fr; }
      .row > h2 { position: static; margin-bottom: 8px; }
      .entry { grid-template-columns: 1fr; }
      .topbar nav a:nth-child(n+4) { display: none; }
    }
    @media (prefers-reduced-motion: reduce) {
      html { scroll-behavior: auto; }
      .track { animation: none; }
      .entry, .btn, .contact a.mail, .big-skills li { transition: none; }
    }
  </style>
</head>
<body>

  <header class="hero">
    <div class="wrap">
      <div class="topbar">
        <a class="mark" href="#top">SHOLPAN S.</a>
        <nav aria-label="Sections">
          <a href="#about">About</a>
          <a href="#education">Education</a>
          <a href="#experience">Experience</a>
          <a href="#volunteering">Volunteering</a>
          <a href="#skills">Skills</a>
          <a href="#languages">Languages</a>
        </nav>
      </div>

      <h1 id="top"><span>Sholpan</span><span>Shabdenbek</span></h1>
      <div class="sticker" aria-hidden="true">Age <span id="age">20</span><br>Astana, KZ</div>

      <div class="hero-low">
        <div>
          <p class="lede">Geography student, English tutor and volunteer. I learn fast and I take responsibility for my work.</p>
          <div class="facts">
            <span>Eurasian National University</span>
            <span>4th year</span>
            <span>Kazakh, Russian, English</span>
          </div>
          <a class="btn" href="mailto:erkinkyzy.sholpan@gmail.com">Email me</a>
        </div>
        <!-- To show your photo: save it as photo.jpg next to this file. Without it, this block disappears. -->
        <div class="photo"><img src="photo.jpg" alt="Portrait of Sholpan Shabdenbek" onerror="this.parentNode.remove()"></div>
      </div>
    </div>
  </header>

  <div class="marquee" aria-hidden="true">
    <div class="track" id="track">
      <span>Responsibility</span><span class="sep">&#10022;</span>
      <span>Fast learner</span><span class="sep">&#10022;</span>
      <span>Adaptability</span><span class="sep">&#10022;</span>
      <span>Communication</span><span class="sep">&#10022;</span>
      <span>Teamwork</span><span class="sep">&#10022;</span>
      <span>Teaching</span><span class="sep">&#10022;</span>
    </div>
  </div>

  <main class="wrap">

    <section id="about" class="row">
      <h2>About me</h2>
      <p class="about">I study <mark>scientific geography</mark> and enjoy understanding how places, people and systems fit together. Outside lectures I teach English online and volunteer at education events.</p>
    </section>

    <section id="education" class="row">
      <h2>Education</h2>
      <div>
        <div class="entry">
          <div class="when">Now, 4th year</div>
          <div>
            <h3>L.N. Gumilyov Eurasian National University</h3>
            <div class="where">Astana, Kazakhstan</div>
            <p>Bachelor's studies, major in scientific geography.</p>
          </div>
        </div>
      </div>
    </section>

    <section id="experience" class="row">
      <h2>Work experience</h2>
      <div>
        <div class="entry">
          <div class="when">5 months</div>
          <div>
            <h3>Online English tutor</h3>
            <div class="where">Remote</div>
            <ul>
              <li>Taught English to students one-on-one online.</li>
              <li>Planned lessons around each student's level and goals.</li>
            </ul>
          </div>
        </div>
        <div class="entry">
          <div class="when">Retail</div>
          <div>
            <h3>Sales consultant</h3>
            <div class="where">Astana, Kazakhstan</div>
            <ul>
              <li>Advised customers and helped them choose the right product.</li>
              <li>Worked in a fast-paced team.</li>
            </ul>
          </div>
        </div>
      </div>
    </section>

    <section id="volunteering" class="row">
      <h2>Volunteering</h2>
      <div>
        <div class="entry">
          <div class="when">Volunteer</div>
          <div>
            <h3>International Education Fair (IEF)</h3>
            <div class="where">Bolashaq Development Fund</div>
            <p>Helped run the fair, supporting the organizers and guiding visitors to the information they needed.</p>
          </div>
        </div>
      </div>
    </section>

    <section id="skills" class="row">
      <h2>Skills</h2>
      <div>
        <ul class="big-skills">
          <li>Responsibility</li>
          <li>Fast learner</li>
          <li>Adaptability</li>
        </ul>
        <ul class="chips">
          <li>Communication</li>
          <li>Teamwork</li>
          <li>Teaching and explaining</li>
          <li>Customer service</li>
          <li>Time management</li>
        </ul>
      </div>
    </section>

    <section id="languages" class="row">
      <h2>Languages</h2>
      <div class="langs">
        <div class="lang"><b>Kazakh</b><span>Native</span></div>
        <div class="lang"><b>Russian</b><span>Fluent</span></div>
        <div class="lang"><b>English</b><span>B2, upper-intermediate</span></div>
      </div>
    </section>

  </main>

  <footer class="contact" id="contact">
    <div class="wrap">
      <h2>Let's talk.</h2>
      <a class="mail" href="mailto:erkinkyzy.sholpan@gmail.com">erkinkyzy.sholpan@gmail.com</a>
      <small>&copy; <span id="year">2026</span> Sholpan Shabdenbek</small>
    </div>
  </footer>

  <script>
    // Age is worked out from the date of birth (3 July 2006), so it stays correct.
    (function () {
      var b = new Date(2006, 6, 3), n = new Date();
      var a = n.getFullYear() - b.getFullYear();
      var m = n.getMonth() - b.getMonth();
      if (m < 0 || (m === 0 && n.getDate() < b.getDate())) a--;
      document.getElementById("age").textContent = a;
      document.getElementById("year").textContent = n.getFullYear();
    })();
    // Repeat the marquee content so it loops without a gap.
    (function () {
      var t = document.getElementById("track");
      t.innerHTML = t.innerHTML + t.innerHTML;
    })();
  </script>
</body>
</html>

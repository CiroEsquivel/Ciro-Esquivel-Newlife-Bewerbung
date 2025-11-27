# Ciro-Esquivel-Newlife-Bewerbung
<!DOCTYPE html>
<html lang="de">
<head>
<meta charset="UTF-8" />
<title>Ciro Esquivel – NewLife Roleplay Bewerbung</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<!-- Google Fonts -->
<link href="https://fonts.googleapis.com/css2?family=Cinzel:wght@400;600;700&family=Poppins:wght@300;400;500;600&display=swap" rel="stylesheet" />
<style>
:root {
--bg-main: #120b08;
--bg-alt: #1b120e;
--coffee: #6b3e2e;
--sand: #d6b98c;
--sunset: #b14527;
--gold: #e5cb76;
--ink: #f5ede2;
--muted: #b3a692;
--accent: #ff4b3a;
}

* {
box-sizing: border-box;
margin: 0;
padding: 0;
}

html {
scroll-behavior: smooth;
}

body {
font-family: "Poppins", sans-serif;
background: radial-gradient(circle at top, #2a1a12 0%, var(--bg-main) 45%, #050302 100%);
color: var(--ink);
line-height: 1.6;
}

/* NAVBAR */

header {
position: fixed;
top: 0;
left: 0;
right: 0;
z-index: 100;
background: linear-gradient(to right, rgba(11,7,5,0.98), rgba(37,20,15,0.96));
border-bottom: 1px solid rgba(229,203,118,0.22);
backdrop-filter: blur(8px);
}

.nav-container {
max-width: 1100px;
margin: 0 auto;
display: flex;
align-items: center;
justify-content: space-between;
padding: 0.7rem 1.5rem;
}

.logo {
font-family: "Cinzel", serif;
letter-spacing: 0.15em;
font-size: 0.9rem;
text-transform: uppercase;
color: var(--gold);
}

nav ul {
list-style: none;
display: flex;
gap: 1rem;
font-size: 0.9rem;
}

nav a {
text-decoration: none;
color: var(--sand);
text-transform: uppercase;
letter-spacing: 0.1em;
font-size: 0.75rem;
position: relative;
padding-bottom: 0.15rem;
}

nav a::after {
content: "";
position: absolute;
left: 0;
bottom: 0;
width: 0;
height: 1px;
background: var(--accent);
transition: width 0.25s ease;
}

nav a:hover::after {
width: 100%;
}

/* HERO */

.hero {
min-height: 100vh;
display: flex;
align-items: center;
justify-content: center;
padding: 6rem 1.5rem 3rem;
position: relative;
overflow: hidden;
color: var(--ink);
}

/* Hero Background: Stadt + Farbverlauf */
.hero::before {
content: "";
position: absolute;
inset: 0;
background:
linear-gradient(to bottom, rgba(0,0,0,0.55), rgba(0,0,0,0.9)),
url("img/hero-city.jpg") center center / cover no-repeat;
z-index: -2;
filter: grayscale(10%) saturate(120%);
}

.hero::after {
content: "";
position: absolute;
inset: 0;
background: radial-gradient(circle at top left, rgba(177,69,39,0.35), transparent 55%);
mix-blend-mode: soft-light;
z-index: -1;
}

.hero-inner {
max-width: 1100px;
margin: 0 auto;
display: grid;
grid-template-columns: 3fr 2fr;
gap: 3rem;
align-items: center;
}

.hero-title {
font-family: "Cinzel", serif;
font-size: 2.5rem;
text-transform: uppercase;
letter-spacing: 0.25em;
color: var(--gold);
margin-bottom: 1rem;
}

.hero-sub {
font-size: 1.05rem;
color: var(--sand);
margin-bottom: 1.5rem;
max-width: 520px;
text-shadow: 0 2px 8px rgba(0,0,0,0.7);
}

.hero-tagline {
font-style: italic;
color: var(--muted);
border-left: 3px solid var(--sunset);
padding-left: 0.75rem;
margin-top: 1rem;
text-shadow: 0 2px 6px rgba(0,0,0,0.7);
background: rgba(0,0,0,0.35);
border-radius: 4px;
padding-top: 0.4rem;
padding-bottom: 0.4rem;
}

.hero-meta {
display: flex;
flex-wrap: wrap;
gap: 1rem;
margin-top: 1.5rem;
font-size: 0.9rem;
color: var(--muted);
}

.meta-pill {
border-radius: 999px;
border: 1px solid rgba(229,203,118,0.5);
padding: 0.3rem 0.9rem;
background: rgba(12,6,4,0.7);
backdrop-filter: blur(3px);
box-shadow: 0 4px 12px rgba(0,0,0,0.6);
}

.badge {
display: inline-flex;
align-items: center;
gap: 0.4rem;
font-size: 0.8rem;
text-transform: uppercase;
letter-spacing: 0.09em;
background: rgba(177,69,39,0.25);
border: 1px solid rgba(255,75,58,0.5);
padding: 0.35rem 0.75rem;
border-radius: 999px;
color: #ffe9c8;
margin-top: 0.75rem;
box-shadow: 0 4px 14px rgba(0,0,0,0.7);
}

.badge span {
font-size: 0.7rem;
font-weight: 600;
color: var(--accent);
}

/* Right hero column card */

.hero-card {
border-radius: 18px;
border: 1px solid rgba(213,190,120,0.8);
background:
radial-gradient(circle at top, rgba(225,174,102,0.2), rgba(22,11,7,0.95)),
url("img/crime-texture.jpg") center/cover no-repeat;
background-blend-mode: overlay;
padding: 1.75rem 1.5rem;
box-shadow: 0 18px 45px rgba(0,0,0,0.85);
}

.hero-card-title {
font-family: "Cinzel", serif;
font-size: 1.1rem;
letter-spacing: 0.16em;
text-transform: uppercase;
color: var(--gold);
margin-bottom: 1rem;
}

.hero-card-line {
font-size: 0.9rem;
color: var(--sand);
margin-bottom: 0.35rem;
text-shadow: 0 1px 4px rgba(0,0,0,0.7);
}

.hero-card-foot {
margin-top: 1.25rem;
font-size: 0.8rem;
color: var(--muted);
border-top: 1px solid rgba(213,190,120,0.35);
padding-top: 0.85rem;
text-shadow: 0 1px 4px rgba(0,0,0,0.7);
}

/* SECTIONS */

section {
padding: 3.5rem 1.5rem;
}

.section-inner {
max-width: 1100px;
margin: 0 auto;
}

.section-title {
font-family: "Cinzel", serif;
text-transform: uppercase;
letter-spacing: 0.25em;
font-size: 1rem;
color: var(--gold);
margin-bottom: 0.75rem;
}

.section-heading {
font-size: 1.6rem;
color: var(--sand);
margin-bottom: 1.5rem;
}

.section-grid {
display: grid;
grid-template-columns: 1.4fr 1.6fr;
gap: 2.5rem;
}

/* Background band / image strip for certain sections */

.band {
background:
linear-gradient(to right, rgba(12,7,4,0.96), rgba(30,18,11,0.96)),
url("img/colombia-mountains.jpg") center/cover no-repeat fixed;
background-blend-mode: soft-light;
border-top: 1px solid rgba(213,190,120,0.35);
border-bottom: 1px solid rgba(213,190,120,0.35);
}

/* History table */

.history-table {
width: 100%;
border-collapse: collapse;
font-size: 0.9rem;
margin-top: 0.5rem;
background: rgba(19,10,7,0.9);
border-radius: 10px;
overflow: hidden;
box-shadow: 0 12px 30px rgba(0,0,0,0.5);
}

.history-table thead {
background: linear-gradient(to right, var(--coffee), var(--sunset));
}

.history-table th,
.history-table td {
padding: 0.65rem 0.8rem;
text-align: left;
}

.history-table th {
font-weight: 600;
color: #f9f3de;
text-transform: uppercase;
letter-spacing: 0.08em;
font-size: 0.72rem;
}

.history-table tbody tr:nth-child(odd) {
background: rgba(32,18,13,0.96);
}

.history-table tbody tr:nth-child(even) {
background: rgba(23,13,9,0.96);
}

.history-table td {
border-top: 1px solid rgba(140,94,65,0.45);
color: var(--muted);
}

.history-table td:first-child {
color: var(--sand);
font-weight: 500;
}

/* Roles list */

.pill-list {
display: flex;
flex-direction: column;
gap: 0.7rem;
margin-top: 0.5rem;
}

.pill-item {
padding: 0.6rem 0.9rem;
border-radius: 12px;
background: rgba(26,14,10,0.95);
border: 1px solid rgba(209,176,111,0.4);
font-size: 0.9rem;
}

.pill-label {
font-weight: 600;
color: var(--sand);
}

.pill-desc {
color: var(--muted);
font-size: 0.85rem;
}

/* Highlight block */

.highlight {
margin-top: 1.25rem;
padding: 0.9rem 1rem;
border-left: 3px solid var(--sunset);
background: radial-gradient(circle at left, rgba(177,69,39,0.24), rgba(15,9,6,0.95));
font-size: 0.9rem;
color: var(--muted);
}

.quote-big {
font-style: italic;
color: var(--sand);
margin-top: 1rem;
}

/* Character section */

.char-meta {
display: grid;
grid-template-columns: repeat(auto-fit,minmax(160px,1fr));
gap: 1rem;
margin-bottom: 1.5rem;
}

.char-meta-item {
background: rgba(25,14,10,0.95);
border-radius: 10px;
border: 1px solid rgba(213,190,120,0.4);
padding: 0.7rem 0.9rem;
font-size: 0.9rem;
color: var(--muted);
}

.char-meta-item span {
display: block;
font-size: 0.75rem;
text-transform: uppercase;
letter-spacing: 0.12em;
color: var(--gold);
margin-bottom: 0.3rem;
}

/* Checklist */

.check-list {
list-style: none;
margin: 0.5rem 0 1.5rem;
padding: 0;
font-size: 0.92rem;
}

.check-list li {
margin-bottom: 0.35rem;
}

.check-icon {
color: var(--accent);
margin-right: 0.35rem;
}

/* Trailer section */

.script-block {
border-radius: 14px;
border: 1px solid rgba(222,184,135,0.5);
padding: 1.1rem 1.2rem;
background:
radial-gradient(circle at top left, rgba(214,185,140,0.13), rgba(12,7,5,0.98)),
url("img/crime-texture.jpg") center/cover no-repeat;
background-blend-mode: soft-light;
font-size: 0.9rem;
color: var(--muted);
box-shadow: 0 10px 30px rgba(0,0,0,0.7);
}

.script-label {
font-size: 0.8rem;
text-transform: uppercase;
letter-spacing: 0.15em;
color: var(--gold);
margin-bottom: 0.25rem;
display: inline-block;
}

/* Footer */

footer {
border-top: 1px solid rgba(229,203,118,0.25);
padding: 1.5rem;
text-align: center;
font-size: 0.8rem;
color: var(--muted);
background: rgba(7,4,3,0.95);
margin-top: 2rem;
}

footer span {
color: var(--gold);
text-transform: uppercase;
letter-spacing: 0.2em;
font-size: 0.7rem;
}

/* Responsive */

@media (max-width: 880px) {
.hero-inner {
grid-template-columns: 1fr;
}
.hero-card {
order: -1;
}
.section-grid {
grid-template-columns: 1fr;
}
header {
position: static;
}
.hero {
padding-top: 3.5rem;
min-height: 80vh;
}
}

@media (max-width: 600px) {
.hero-title {
font-size: 1.9rem;
letter-spacing: 0.18em;
}
nav ul {
flex-wrap: wrap;
justify-content: flex-end;
}
section {
padding-inline: 1.1rem;
}
}
</style>
</head>
<body>

<!-- NAVBAR -->
<header>
<div class="nav-container">
<div class="logo">CIRO ESQUIVEL</div>
<nav>
<ul>
<li><a href="#about">Über mich</a></li>
<li><a href="#history">RP-Historie</a></li>
<li><a href="#roles">Rollen</a></li>
<li><a href="#character">Charakter</a></li>
<li><a href="#why">Warum NewLife</a></li>
<li><a href="#trailer">Trailer</a></li>
</ul>
</nav>
</div>
</header>

<!-- HERO -->
<section class="hero" id="top">
<div class="hero-inner">
<div>
<h1 class="hero-title">NEWLIFE ROLEPLAY</h1>
<p class="hero-sub">
Bewerbung &amp; Charakterdossier von <strong>Ciro Esquivel</strong> –
geboren in Cali, geformt von Hitze, Staub und Kartellschatten.
Hier endet seine Vergangenheit – und NewLife beginnt.
</p>
<div class="hero-tagline">
„GTA-Roleplay ist für mich kein Spiel – es ist ein Medium, durch das ich Geschichten forme,
Erlebnisse erschaffe und Charaktere mit psychologischer Tiefe lebendig mache.“
</div>
<div class="hero-meta">
<div class="meta-pill">Daniel · 22 Jahre</div>
<div class="meta-pill">4+ Jahre GTA-RP Erfahrung</div>
<div class="meta-pill">Aktiver Charakter: Ciro Esquivel</div>
</div>
<div class="badge">
<span>NEWLIFE</span> Kino-RP statt Routine
</div>
</div>

<aside class="hero-card">
<div class="hero-card-title">Kurzprofil</div>
<p class="hero-card-line"><strong>Origin:</strong> Cali, Kolumbien</p>
<p class="hero-card-line"><strong>Sprachen:</strong> Spanisch · Englisch · gebrochenes Deutsch</p>
<p class="hero-card-line"><strong>Stärken:</strong> Tiefes RP, Lore-Aufbau, Konfliktführung</p>
<p class="hero-card-line"><strong>Rollen:</strong> Badfaction · PD · Militär · Unicorn-Leitung</p>
<p class="hero-card-foot">
„Ich spiele RP nicht nebenbei – ich spiele es bewusst, ernst und langfristig.“
</p>
</aside>
</div>
</section>

<!-- ABOUT & HISTORY (mit Colombia-Band) -->
<section id="about" class="band">
<div class="section-inner">
<div class="section-grid">
<div>
<div class="section-title">About</div>
<h2 class="section-heading">Über mich</h2>
<p>
Ich spiele GTA-Roleplay seit meinem 18. Lebensjahr und habe seitdem mehr als vier Jahre
auf unterschiedlichen Hardcore-Servern verbracht. Für mich ist RP kein schneller
Zeitvertreib – sondern eine Mischung aus Film, Theater und Charakterstudie.
</p>
<p class="quote-big">
Ich will keine Szenen farmen – ich will Geschichten schreiben.
</p>
</div>
<div id="history">
<div class="section-title">History</div>
<h2 class="section-heading">RP-Historie – Stationen &amp; Entwicklung</h2>
<table class="history-table">
<thead>
<tr>
<th>Server</th>
<th>Schwerpunkt &amp; Wert</th>
</tr>
</thead>
<tbody>
<tr>
<td>Dirty Gaming</td>
<td>PD &amp; Unterwelt · Hardcore Konflikt-RP · Transporte · Deals</td>
</tr>
<tr>
<td>Diamond Life</td>
<td>Organisierte Gangs · Bad Fraktionen · Straßenpolitik</td>
</tr>
<tr>
<td>Fast Life</td>
<td>Schnelle Konflikte · Risiko-RP · Bad-Fraktion</td>
</tr>
<tr>
<td>Next Roleplay</td>
<td>Zivilist &amp; Firmenkontakte · soziales Langzeit-RP</td>
</tr>
<tr>
<td>Identity Valley</td>
<td>Deep Charakter-Progression · Lore-Aufbau</td>
</tr>
<tr>
<td>GVMP</td>
<td>Organisierte Gangs · Hardcore Konflikt-RP</td>
</tr>
<tr>
<td>Narco City</td>
<td>Kartell-Szenarien · Schmuggelnetze</td>
</tr>
<tr>
<td>Corleone (Hauptspielzeit)</td>
<td>Langzeituntergrund · tiefe Strukturen · Gang Dynamics</td>
</tr>
</tbody>
</table>
<div class="highlight">
Ich habe am längsten auf <strong>Corleone</strong> gespielt – tief im RP, über Jahre.
Doch dort verlor das RP an Tiefe und Entwicklung. Ich suche einen Server,
der Charaktere nicht verwaltet, sondern wachsen lässt. <br />
<strong>→ Deshalb NewLife. Kino-RP statt Routine.</strong>
</div>
</div>
</div>
</div>
</section>

<!-- ROLES -->
<section id="roles">
<div class="section-inner">
<div class="section-title">Experience</div>
<h2 class="section-heading">Gespielte Rollen – Vielseitigkeit</h2>
<div class="section-grid">
<div>
<div class="pill-list">
<div class="pill-item">
<div class="pill-label">Gang / Badfrags</div>
<div class="pill-desc">
Territorien · Straßenpolitik · Diplomatie · Eskalation – Konflikte nicht nur schießen,
sondern aufbauen, verhandeln und mit Konsequenz zu Ende spielen.
</div>
</div>
<div class="pill-item">
<div class="pill-label">PD</div>
<div class="pill-desc">
Funkprotokolle · Festnahmen · Einsatzberichte – sauberes Arbeiten,
Perspektivwechsel zur Staatsseite, Verständnis für Strukturen und Regeln.
</div>
</div>
<div class="pill-item">
<div class="pill-label">Militär</div>
<div class="pill-desc">
Strategie · Teamführung · Missionsdisziplin – koordiniertes Vorgehen,
taktische Planung und klares Rollenverständnis im Team.
</div>
</div>
<div class="pill-item">
<div class="pill-label">Unicorn-Leitung</div>
<div class="pill-desc">
Personalführung · Events · Finanzen – soziales RP, Verantwortung,
Organisation und Nightlife-Atmosphäre sinnvoll verbunden.
</div>
</div>
</div>
</div>
<div>
<p>
Diese Mischung aus illegalen und staatlichen Rollen hat mir eine Perspektive gegeben,
die viele Spieler nicht haben: Ich kenne das Chaos der Straße und die Ordnung des Gesetzes.
</p>
<p class="quote-big">
Ich kenne Gesetz <strong>und</strong> Straße.
Ich spiele beides konsequent und filmreif aus.
</p>
</div>
</div>
</div>
</section>

<!-- CHARACTER -->
<section id="character" class="band">
<div class="section-inner">
<div class="section-title">Character</div>
<h2 class="section-heading">Charakterdossier – Ciro Esquivel</h2>

<div class="char-meta">
<div class="char-meta-item">
<span>Geburtsort</span>
Cali, Kolumbien
</div>
<div class="char-meta-item">
<span>Alter</span>
26 Jahre
</div>
<div class="char-meta-item">
<span>Sprachen</span>
Spanisch · Englisch · gebrochenes Deutsch
</div>
</div>

<h3 style="margin-bottom:0.5rem;color:var(--sand);">Herkunft</h3>
<p>
Geboren zwischen Kaffee und Kartellstahl. Eine Familie ohne Telefonnummer,
aber mit Reputation im Untergrund. Schweigen war Pflicht, Vertrauen ein Luxus.
</p>
<p class="quote-big">
„In Kolumbien bedeutet ein Fehler kein Ärger – sondern ein Grab.“
</p>

<h3 style="margin-top:1.8rem;margin-bottom:0.5rem;color:var(--sand);">Neuanfang in NewLife</h3>
<p>
Er kommt nicht als Kartellsoldat. Er kommt, um zu leben, statt nur zu überleben.
NewLife ist für Ciro keine Flucht, sondern eine bewusste Entscheidung:
Weg von blinder Loyalität – hin zu eigener Identität.
</p>

<h3 style="margin-top:1.6rem;margin-bottom:0.5rem;color:var(--sand);">Ziele in NewLife</h3>
<ul class="check-list">
<li><span class="check-icon">✔</span> legales Business gründen</li>
<li><span class="check-icon">✔</span> soziales Netzwerk ohne Pulver &amp; Blut aufbauen</li>
<li><span class="check-icon">✔</span> perspektivisch ein Wechsel ins PD als Richtungsänderung</li>
<li><span class="check-icon">✔</span> Wachstum statt Gewaltspirale – Charakterentwicklung mit Tiefgang</li>
</ul>
</div>
</section>

<!-- WHY NEWLIFE -->
<section id="why">
<div class="section-inner">
<div class="section-title">Reason</div>
<h2 class="section-heading">Warum ich zu NewLife passe</h2>
<div class="section-grid">
<div>
<ul class="check-list">
<li><span class="check-icon">✔</span> tiefes RP – keine Oberflächen-Action</li>
<li><span class="check-icon">✔</span> Charakterentwicklung statt Abkürzungen</li>
<li><span class="check-icon">✔</span> Konfliktaufbau – kein Schnellschuss</li>
<li><span class="check-icon">✔</span> langfristige Storyline – keine Kurzzeit-Idee</li>
<li><span class="check-icon">✔</span> reif – kein PowerRP / kein FailRP</li>
<li><span class="check-icon">✔</span> passend für Qualität, Anspruch &amp; Lorepflege</li>
</ul>
</div>
<div>
<p>
Ich will nicht nur einen Slot auf einem Server – ich will Teil einer lebenden Stadt werden,
in der Entscheidungen Gewicht haben und Charaktere Spuren hinterlassen.
</p>
<p class="quote-big">
Ich will nicht mitlaufen – ich will <strong>beitragen</strong>.
</p>
</div>
</div>

<h3 style="margin-top:2rem;margin-bottom:0.4rem;color:var(--sand);">Schlusswort</h3>
<p>
Ich bewerbe mich nicht um Zugang – ich bewerbe mich um eine Bühne.
Wenn ihr mir die Chance gebt, bekommt ihr einen Charakter mit Vergangenheit,
Vision, Zukunft und Gewicht. Er wird NewLife nicht konsumieren – er wird es prägen.
</p>
<p class="quote-big">
Ich bin bereit. Wenn ihr es seid – öffnet die Tür.
<strong>CIRO ESQUIVEL – EIN NEUES LEBEN BEGINNT.</strong>
</p>
</div>
</section>

<!-- TRAILER -->
<section id="trailer">
<div class="section-inner">
<div class="section-title">Trailer</div>
<h2 class="section-heading">Cinematic Voiceover – RP Trailer</h2>
<div class="script-block">
<div class="script-label">Voiceover Script</div>
<p>
(Dunkler Atem – Wind – ein Zug an einer Zigarette.)<br><br>
<strong>VOICE:</strong><br>
Cali hat mich geboren… aber die Welt hat mich geformt.<br>
Ich bin kein Engel. Kein Teufel. Nur ein Mann, der überlebt hat.<br><br>
Blut auf Asphalt. Namen in der Erde. Loyalität – teuer bezahlt.<br>
Doch ich bin hier – nicht, um zu sterben.<br>
Sondern um neu zu leben.<br><br>
Beat droppt langsam. Schwarzblende. Schritte auf nassem Boden.<br><br>
<strong>VOICE:</strong><br>
NewLife… hört genau zu.<br>
Ich bin Ciro Esquivel. Ich komme nicht für Krieg.<br>
Ich komme für Geschichte.
</p>
</div>
</div>
</section>

<footer>
<span>CIRO ESQUIVEL</span><br />
Bewerbung für NewLife Roleplay · erstellt als Onepager
</footer>

</body>
</html>

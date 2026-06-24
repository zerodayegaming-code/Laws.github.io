[613-laws-hebrew-israelite.5.html](https://github.com/user-attachments/files/29272836/613-laws-hebrew-israelite.5.html)

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>The 613 Laws of the Most High</title>
<style>
*{box-sizing:border-box;margin:0;padding:0}
body{background:#0a0a0a;font-family:-apple-system,BlinkMacSystemFont,'Segoe UI',Roboto,sans-serif;color:#f3f4f6;min-height:100vh;padding:16px}
h1,h2,h3{font-weight:700}
button{cursor:pointer;font-family:inherit}
input{font-family:inherit}
::-webkit-scrollbar{width:4px}
::-webkit-scrollbar-track{background:#1a1a1a}
::-webkit-scrollbar-thumb{background:#444;border-radius:2px}
@keyframes spin{to{transform:rotate(360deg)}}
.spin{display:inline-block;animation:spin 1s linear infinite}
#app{max-width:640px;margin:0 auto}

/* Header */
.header{text-align:center;margin-bottom:20px}
.header .star{font-size:40px;display:block;margin-bottom:8px}
.header h1{color:#fbbf24;font-size:22px;margin-bottom:4px}
.header .sub{color:#6b7280;font-size:13px}
.header .verse{color:#78350f;font-size:11px;margin-top:4px;font-style:italic}
.cache-info{color:#374151;font-size:10px;margin-top:6px}

/* Stat cards */
.stat-grid{display:grid;grid-template-columns:repeat(4,1fr);gap:8px;margin-bottom:16px}
.stat-card{border-radius:10px;padding:8px;text-align:center}
.stat-card .num{font-size:18px;font-weight:700}
.stat-card .lbl{font-size:11px;opacity:.7}

/* Nav */
.nav{display:flex;gap:6px;margin-bottom:16px;overflow-x:auto;padding-bottom:4px}
.nav button{padding:6px 10px;border-radius:10px;font-size:12px;font-weight:500;white-space:nowrap;flex-shrink:0;transition:all .15s;border:1px solid #374151;background:#111827;color:#d1d5db}
.nav button.active{background:#eab308;color:#000;border-color:#eab308}

/* Panels */
.panel{border-radius:16px;padding:16px;background:#0a0a0a}
.panel h2{color:#fbbf24;margin-bottom:4px}
.panel .panel-sub{color:#6b7280;font-size:12px;margin-bottom:12px}

/* Filters */
.filter-group{margin-bottom:10px}
.filter-label{color:#6b7280;font-size:10px;text-transform:uppercase;letter-spacing:.1em;margin-bottom:6px;display:block}
.filter-btns{display:flex;flex-wrap:wrap;gap:6px}
.filter-btn{padding:4px 10px;border-radius:999px;font-size:12px;white-space:nowrap;flex-shrink:0;transition:all .15s;border:1px solid #374151;background:#1f2937;color:#9ca3af}
.filter-btn.active{background:#eab308;color:#000;border-color:#eab308}
.filter-cats{display:flex;flex-wrap:wrap;gap:6px;max-height:96px;overflow-y:auto}

/* Search */
.search-input{width:100%;padding:8px 12px;border-radius:8px;border:1px solid #374151;background:#1f2937;color:#fff;font-size:13px;margin-bottom:12px;outline:none}
.search-input:focus{border-color:#eab308}

/* Active chips */
.chips-bar{display:flex;flex-wrap:wrap;gap:6px;margin-bottom:12px;padding:8px;background:#1f2937;border-radius:8px;border:1px solid #374151;align-items:center}
.chip-label{color:#6b7280;font-size:11px}
.chip{background:#78350f;color:#fde68a;font-size:11px;font-weight:600;padding:2px 8px;border-radius:999px;display:inline-flex;align-items:center;gap:4px}
.chip button{background:none;border:none;color:#fde68a;font-weight:700;font-size:13px;line-height:1;cursor:pointer;padding:0}
.clear-all{background:none;border:none;color:#6b7280;font-size:11px;cursor:pointer}

/* Toggle */
.toggle-btn{width:100%;margin-bottom:12px;padding:8px 12px;border-radius:8px;font-size:13px;font-weight:500;display:flex;justify-content:space-between;align-items:center;transition:all .15s;border:1px solid #374151;background:#1f2937;color:#d1d5db;text-align:left}
.toggle-btn.on{border-color:#ca8a04;background:#1c1400;color:#fde68a}
.toggle-hint{font-size:11px;color:#6b7280;margin-left:8px;flex-shrink:0}

/* Count bar */
.count-bar{display:flex;align-items:center;justify-content:space-between;padding:8px 12px;border-radius:8px;margin-bottom:12px;border:1px solid #374151;background:#1f2937}
.count-bar.filtered{border-color:#92400e;background:#1c1400}
.count-num{font-size:20px;font-weight:700;color:#fff}
.count-bar.filtered .count-num{color:#fbbf24}
.count-text{font-size:12px;color:#9ca3af;margin-left:8px}
.count-text .total{color:#e5e7eb;font-weight:600}
.count-text .out{color:#d97706;margin-left:6px}
.count-text .shared{color:#4b5563;margin-left:6px}
.progress-wrap{display:flex;align-items:center;gap:6px}
.progress-bar{width:60px;height:4px;background:#374151;border-radius:2px;overflow:hidden}
.progress-fill{height:100%;background:#eab308;border-radius:2px;transition:width .3s}
.progress-pct{color:#d97706;font-size:11px;font-family:monospace}

/* Section divider */
.section-div{display:flex;align-items:center;gap:8px;margin:12px 0 8px}
.section-div span{font-size:11px;font-weight:700;text-transform:uppercase;letter-spacing:.08em;white-space:nowrap}
.section-div .s-count{color:#4b5563;text-transform:none;font-weight:normal}
.section-div hr{flex:1;border:none;border-top:1px solid #1f2937}

/* Law cards */
.results{max-height:520px;overflow-y:auto;padding-right:4px}
.law-card{border:1px solid #374151;border-radius:10px;padding:12px;background:#111827;margin-bottom:8px;cursor:pointer;transition:background .15s}
.law-card:hover{background:#1f2937}
.law-card-top{display:flex;justify-content:space-between;align-items:flex-start;margin-bottom:6px;flex-wrap:wrap;gap:4px}
.law-id{color:#6b7280;font-size:11px;font-family:monospace}
.badges{display:flex;gap:4px;flex-wrap:wrap;justify-content:flex-end}
.badge{font-size:11px;font-weight:600;padding:2px 8px;border-radius:999px;white-space:nowrap}
.law-text{color:#f3f4f6;font-size:13px;font-weight:500;line-height:1.55;margin-bottom:6px}
.law-ref{background:none;border:none;padding:0;color:#d97706;font-size:12px;font-style:italic;cursor:pointer;text-decoration:underline;text-underline-offset:2px;text-align:left}
.law-note{margin-top:10px;padding-top:10px;border-top:1px solid #374151;color:#fef08a;font-size:12px;line-height:1.65}
.law-toggle{color:#374151;font-size:11px;margin-top:6px}

/* Empty state */
.empty{text-align:center;padding:32px}
.empty p{color:#6b7280;font-size:13px;font-style:italic;margin-bottom:8px}
.empty button{background:none;border:none;color:#d97706;font-size:12px;cursor:pointer;text-decoration:underline}

/* Scripture modal */
.modal-overlay{position:fixed;inset:0;background:rgba(0,0,0,.9);z-index:1000;display:flex;align-items:center;justify-content:center;padding:16px}
.modal-box{background:#111;border:1px solid #92400e;border-radius:16px;padding:20px;max-width:440px;width:100%;box-shadow:0 25px 50px rgba(0,0,0,.8)}
.modal-head{display:flex;justify-content:space-between;align-items:center;margin-bottom:12px}
.modal-ref{color:#fbbf24;font-weight:700;font-size:14px}
.modal-close{background:none;border:none;color:#6b7280;font-size:22px;font-weight:700;line-height:1;padding:0 4px;cursor:pointer}
.modal-loading{text-align:center;color:#9ca3af;padding:24px;font-size:13px}
.modal-verse{border-left:3px solid #92400e;padding-left:12px;margin-bottom:12px}
.modal-verse p{color:#fef3c7;font-size:13px;line-height:1.75;font-style:italic}
.modal-cite{color:#4b5563;font-size:11px;text-align:right}
.modal-hint{color:#374151;font-size:10px;margin-top:12px;text-align:center}

/* Overview */
.overview-framework{background:#111;border:1px solid #92400e;border-radius:16px;padding:16px;margin-bottom:12px}
.overview-framework h2{color:#fbbf24;margin-bottom:10px}
.fw-row{display:flex;gap:6px;margin-bottom:8px;align-items:flex-start}
.fw-bullet{color:#d97706;flex-shrink:0}
.fw-text{color:#d1d5db;font-size:13px;line-height:1.6}
.fw-text strong{color:#fff}
.status-key{background:#111;border:1px solid #374151;border-radius:16px;padding:16px;margin-bottom:12px}
.status-key h2{color:#fbbf24;margin-bottom:10px}
.sk-row{display:flex;gap:8px;margin-bottom:8px;align-items:flex-start}
.sk-dot{width:10px;height:10px;border-radius:50%;flex-shrink:0;margin-top:3px;display:inline-block}
.sk-text{font-size:13px;color:#9ca3af}
.sk-text strong{color:#fff}
.overview-cards{display:grid;grid-template-columns:repeat(2,1fr);gap:8px}
.ov-card{text-align:left;border-radius:10px;padding:12px;background:#111;cursor:pointer;transition:background .15s;border:1px solid #374151}
.ov-card:hover{background:#1f2937}
.ov-card .ov-label{font-weight:600;font-size:13px}
.ov-card .ov-count{font-size:20px;font-weight:700;margin-top:4px}
.ov-card .ov-arrow{font-size:11px;font-weight:normal;opacity:.5}

/* Agri split */
.agri-tabs{display:flex;gap:8px;flex-wrap:wrap;margin-bottom:16px}
.agri-tab{padding:6px 14px;border-radius:10px;font-size:13px;font-weight:500;cursor:pointer;transition:all .15s}

/* Footer */
.footer{color:#1f2937;font-size:11px;text-align:center;margin-top:16px}
</style>
</head>
<body>
<div id="app">
  <div class="header">
    <span class="star">✡️</span>
    <h1>The 613 Laws of the Most High</h1>
    <p class="sub">For the Children of Israel · KJV 1611 · All Laws Remain · Torah-Only</p>
    <p class="verse">"Think not that I am come to destroy the law, or the prophets: I am not come to destroy, but to fulfil." — Matthew 5:17</p>
    <p class="cache-info" id="cache-info">📖 Tap any scripture reference to load KJV verse · Cached after first load</p>
  </div>
  <div class="stat-grid" id="stat-grid"></div>
  <div class="nav" id="nav"></div>
  <div id="main-content"></div>
  <p class="footer">613 Commandments of the Most High · King James Version 1611 · Given to the children of Israel at Mount Sinai</p>
</div>

<div id="modal" style="display:none" class="modal-overlay">
  <div class="modal-box">
    <div class="modal-head">
      <span class="modal-ref" id="modal-ref"></span>
      <button class="modal-close" onclick="closeModal()">×</button>
    </div>
    <div id="modal-body"></div>
  </div>
</div>

<script>
// ── DATA ─────────────────────────────────────────────────────────────────────
const ALL_LAWS_RAW=[[1,'Know there is a God (the Most High, Ahayah)','Exodus 20:2','Belief & Knowledge','Both','binding','Foundation of all truth — the first commandment given to Israel.'],
  [2,'Have no other gods before Him','Exodus 20:3','Belief & Knowledge','Both','binding','No worship of any deity, image, or idol whatsoever.'],
  [3,'Know that He is one','Deuteronomy 6:4','Belief & Knowledge','Both','binding','Hear, O Israel: The LORD our God is one LORD (Deuteronomy 6:4) — the foundation of all Israelite faith.'],
  [4,'Love Him with all your heart, soul, and might','Deuteronomy 6:5','Belief & Knowledge','Both','binding','And thou shalt love the LORD thy God with all thine heart, and with all thy soul, and with all thy might (Deuteronomy 6:5). Yeshua confirmed this as the first and greatest commandment (Matthew 22:37).'],
  [5,'Fear the Most High','Deuteronomy 10:20','Belief & Knowledge','Both','binding','The fear of the LORD is the beginning of wisdom (Proverbs 9:10). This is not terror, but deep reverence and awe before the Most High.'],
  [6,'Sanctify His Name','Leviticus 22:32','Belief & Knowledge','Both','binding','Use the proper names — Ahayah, Yeshua — not substitutes like God or Lord.'],
  [7,'Do not profane His Name','Leviticus 22:32','Belief & Knowledge','Both','binding','Do not misuse or replace His sacred name.'],
  [8,'Worship Him as He has ordered; do not destroy holy objects','Deuteronomy 12:4','Belief & Knowledge','Both','binding','Worship according to Torah, not man-made tradition.'],
  [9,'Listen to the true prophet','Deuteronomy 18:15','Belief & Knowledge','Both','binding','Yeshua was the prophet Moses foretold. His words are Torah-aligned (John 5:46).'],
  [10,'Do not test the Most High','Deuteronomy 6:16','Belief & Knowledge','Both','binding','Do not put conditions on obedience.'],
  [11,'Emulate His ways','Deuteronomy 28:9','Belief & Knowledge','Both','binding','Walk in righteousness as defined by Torah, not man\'s tradition.'],
  [12,'Be with those who only worship Him','Deuteronomy 10:20','Belief & Knowledge','Both','binding','Guard your associations — surround yourself with those who keep the commandments.'],
  [13,'Love your neighbor as yourself','Leviticus 19:18','Social Laws','Both','binding','Thou shalt love thy neighbour as thyself (Leviticus 19:18). Yeshua confirmed this as the second great commandment (Matthew 22:39).'],
  [14,'Love converts and returning brethren','Deuteronomy 10:19','Social Laws','Both','binding','Show love to your brethren who are awakening to their identity.'],
  [15,'Do not hate your brother in your heart','Leviticus 19:17','Social Laws','Both','binding','Hatred between Israelites is forbidden.'],
  [16,'Reprove your brother when necessary','Leviticus 19:17','Social Laws','Both','binding','Correction in love — warn your brother of his sin (Ezekiel 3:18).'],
  [17,'Do not embarrass others publicly','Leviticus 19:17','Social Laws','Both','binding','Shaming a person in public is likened to shedding blood.'],
  [18,'Do not oppress the weak','Exodus 22:21','Social Laws','Both','binding','The stranger, widow, and orphan are under the Most High\'s protection.'],
  [19,'Do not slander','Leviticus 19:16','Social Laws','Both','binding','Do not spread false reports or go as a talebearer among the people.'],
  [20,'Do not take revenge','Leviticus 19:18','Social Laws','Both','binding','Vengeance belongs to the Most High (Romans 12:19, Deuteronomy 32:35).'],
  [21,'Do not bear a grudge','Leviticus 19:18','Social Laws','Both','binding','Let go of offenses — unforgiveness is sin.'],
  [22,'Teach Torah to your children','Deuteronomy 6:7','Social Laws','Both','binding','The responsibility of parents to raise children in the law — diligently.'],
  [23,'Respect and defer to the elders','Leviticus 19:32','Social Laws','Both','binding','Rise before the aged and honor the face of the old man.'],
  [24,'Do not turn to the ways of idol worship','Leviticus 19:4','Social Laws','Both','binding','Reject all Gentile religious customs and holidays.'],
  [25,'Let the fringes on your clothes remind you to keep all the commandments','Numbers 15:39','Social Laws','Both','binding','Tzitzit trigger mindfulness of all 613 commandments at all times.'],
  [26,'Do not blaspheme or curse a judge','Exodus 22:27','Idolatry & False Worship','Both','binding','Honor those in righteous authority; do not speak against them.'],
  [27,'Do not worship idols','Exodus 20:5','Idolatry & False Worship','Both','binding','Includes crosses, statues, and images of a white Jesus.'],
  [28,'Do not bow down to idols','Exodus 20:5','Idolatry & False Worship','Both','binding','Physical prostration to any image is forbidden.'],
  [29,'Do not make an idol','Exodus 20:4','Idolatry & False Worship','Both','binding','Do not craft or commission idolatrous images of any kind.'],
  [30,'Do not make or cast an image for worship','Leviticus 19:4','Idolatry & False Worship','Both','binding','Includes religious statues, paintings of the divine, etc.'],
  [31,'Thou shalt not make with me gods of silver, neither shall ye make unto you gods of gold','Exodus 20:20','Idolatry & False Worship','Both','binding','Material wealth must never become an object of devotion.'],
  [32,'Do not turn a people to idolatry','Exodus 23:13','Idolatry & False Worship','Both','binding','Do not lead others into false worship.'],
  [33,'Destroy a city that has turned to idol worship','Deuteronomy 13:17','Idolatry & False Worship','Both','suspended','Requires functioning Israelite national authority.'],
  [34,'Do not rebuild a city turned to idol worship','Deuteronomy 13:17','Idolatry & False Worship','Both','suspended','Awaits Israelite national governance.'],
  [35,'Do not retain any benefit from that city','Deuteronomy 13:18','Idolatry & False Worship','Both','suspended','No profit from a city given over to idolatry.'],
  [36,'Do not missionize a person to idol worship','Deuteronomy 13:12','Idolatry & False Worship','Both','binding','Never lead anyone toward false worship — a capital sin.'],
  [37,'Do not love the idolatrous missionary','Deuteronomy 13:9','Idolatry & False Worship','Both','binding','Have no affection for those who draw people away from Torah.'],
  [38,'Do not stop hating false doctrine','Deuteronomy 13:9','Idolatry & False Worship','Both','binding','Righteous hatred of false doctrine — not personal vengeance.'],
  [39,'Do not save the idolatrous missionary','Deuteronomy 13:9','Idolatry & False Worship','Both','binding','Do not protect or defend those who teach idolatry.'],
  [40,'Do not speak in defense of the idolatrous missionary','Deuteronomy 13:9','Idolatry & False Worship','Both','binding','No defense of false prophets or idol worshippers.'],
  [41,'Do not refrain from incriminating the idolatrous missionary','Deuteronomy 13:9','Idolatry & False Worship','Both','binding','Testify against those who lead Israel into idolatry.'],
  [42,'Do not prophesy in idolatry','Deuteronomy 18:20','Idolatry & False Worship','Both','binding','No one may speak in the name of the Most High while teaching false doctrine.'],
  [43,'Not to hearken unto the false prophet','Deuteronomy 13:4','Idolatry & False Worship','Both','binding','Test all prophets by their obedience to Torah (Deuteronomy 13:1-4).'],
  [44,'Do not prophesy falsely in the Most High\'s name','Deuteronomy 18:20','Idolatry & False Worship','Both','binding','Any prophecy that contradicts Torah is false — period.'],
  [45,'Do not fear killing a false prophet','Deuteronomy 18:22','Idolatry & False Worship','Both','suspended','Capital punishment requires a functioning Israelite court.'],
  [46,'Never swear in the name of an idol','Exodus 23:13','Idolatry & False Worship','Both','binding','All oaths and promises must be in the Most High\'s name only.'],
  [47,'Do not channel or acknowledge spirits','Leviticus 19:31','Idolatry & False Worship','Both','binding','Regard not them that have familiar spirits, neither seek after wizards, to be defiled by them (Leviticus 19:31).'],
  [48,'Do not consult fortunetellers','Leviticus 19:31','Idolatry & False Worship','Both','binding','There shall not be found among you a consulter with familiar spirits, or a wizard, or a necromancer (Deuteronomy 18:11).'],
  [49,'Do not burn children as sacrifice to Molech','Leviticus 18:21','Idolatry & False Worship','Both','binding','Includes any sacrifice of children to false gods.'],
  [50,'Do not erect a stone pillar in public worship','Deuteronomy 16:22','Idolatry & False Worship','Both','binding','No obelisks, monuments, or pillars for religious veneration.'],
  [51,'Do not erect an idol or bow on a smooth stone for worship','Leviticus 26:1','Idolatry & False Worship','Both','binding','No shrines or altars not ordained by Torah.'],
  [52,'Thou shalt not plant thee a grove of any trees near unto the altar of the LORD thy God','Deuteronomy 16:21','Idolatry & False Worship','Both','binding','For the customs of the people are vain: for one cutteth a tree out of the forest, the work of the hands of the workman (Jeremiah 10:3). This includeth the setting up of trees as sacred objects.'],
  [53,'Destroy idols and the places where they were worshipped','Deuteronomy 12:2','Idolatry & False Worship','Both','binding','Israelites are to have no part in maintaining idol worship.'],
  [54,'Do not derive benefit from idols or bring abominations home','Deuteronomy 7:26','Idolatry & False Worship','Both','binding','Do not decorate your home with pagan symbols.'],
  [55,'Do not derive benefit from the accessories of idols','Deuteronomy 7:25','Idolatry & False Worship','Both','binding','No profit from anything associated with idol worship.'],
  [56,'Make no covenant with Canaanites or their gods','Deuteronomy 7:2','Idolatry & False Worship','Both','binding','No spiritual or covenantal agreements with Gentile religious systems.'],
  [57,'Show them no favor','Deuteronomy 7:2','Idolatry & False Worship','Both','identity','Do not uplift Gentile systems, culture, or religion above Torah.'],
  [58,'Do not let them dwell in your land','Exodus 23:33','Idolatry & False Worship','Both','identity','Covenant community boundaries — for national restoration context.'],
  [59,'Do not imitate Gentile customs and clothing','Leviticus 20:23','Idolatry & False Worship','Both','binding','Reject all Gentile holidays, fashions, and religious traditions.'],
  [60,'Do not be superstitious','Leviticus 19:26','Idolatry & False Worship','Both','binding','Reject omens, lucky charms, and superstitious practices.'],
  [61,'Do not self-induce trances or tolerate soothsayers','Deuteronomy 18:10','Idolatry & False Worship','Both','binding','Thou shalt not suffer a witch to live (Exodus 22:18). Reject all soothsayers and enchanters.'],
  [62,'Do not engage in astrology','Leviticus 19:26','Idolatry & False Worship','Both','binding','Thou shalt not observe times nor engage in astrology — these are abominations before the LORD.'],
  [63,'Do not say incantations or cast spells','Deuteronomy 18:11','Idolatry & False Worship','Both','binding','Neither shall ye use enchantment, nor observe times (Leviticus 19:26).'],
  [64,'Do not attempt to contact the dead','Deuteronomy 18:11','Idolatry & False Worship','Both','binding','There shall not be found among you one that consulteth with the dead — it is abomination (Deuteronomy 18:11).'],
  [65,'Do not consult with mediums','Deuteronomy 18:11','Idolatry & False Worship','Both','binding','A man also or woman that hath a familiar spirit, or that is a wizard, shall surely be put to death (Leviticus 20:27).'],
  [66,'Do not converse with wizards','Deuteronomy 18:11','Idolatry & False Worship','Both','binding','Do not seek after them that have familiar spirits nor after wizards — do not go a whoring after them (Leviticus 19:31).'],
  [67,'Do not do witchcraft','Deuteronomy 18:10','Idolatry & False Worship','Both','binding','Magic, witchcraft, and witchcraft are strictly forbidden.'],
  [68,'Men must not cut the hair at the temples','Leviticus 19:27','Clothing & Appearance','Men','binding','Ye shall not round the corners of your heads (Leviticus 19:27). This is a custom of the heathen nations.'],
  [69,'Men must not shave the beard','Leviticus 19:27','Clothing & Appearance','Men','binding','Ye shall not mar the corners of your beard (Leviticus 19:27).'],
  [70,'Men must not wear women\'s clothes','Deuteronomy 22:5','Clothing & Appearance','Men','binding','The woman shall not wear that which pertaineth unto a man, neither shall a man put on a woman\'s garment: for all that do so are abomination unto the LORD thy God (Deuteronomy 22:5).'],
  [71,'Women must not wear men\'s clothes','Deuteronomy 22:5','Clothing & Appearance','Women','binding','The woman shall not wear that which pertaineth unto a man: for all that do so are abomination unto the LORD thy God (Deuteronomy 22:5).'],
  [72,'Ye shall not print any marks upon your skin','Leviticus 19:28','Clothing & Appearance','Both','binding','Ye shall not make any cuttings in your flesh for the dead, nor print any marks upon you: I am the LORD (Leviticus 19:28).'],
  [73,'Do not tear your skin for mourning','Deuteronomy 14:1','Clothing & Appearance','Both','binding','Cutting yourself in mourning is a Gentile practice — forbidden.'],
  [74,'Do not shave your head in mourning','Deuteronomy 14:1','Clothing & Appearance','Both','binding','Do not mourn as the heathen do.'],
  [75,'Confess and correct your ways before the Most High','Numbers 5:7','Prayer & Study','Both','binding','Repentance is active — turning from sin and returning to the law.'],
  [76,'Recite central prayers and study Torah daily','Deuteronomy 6:7','Prayer & Study','Both','binding','Morning and evening prayers; constant study of scripture.'],
  [77,'Serve the Most High with prayer','Exodus 23:25','Prayer & Study','Both','binding','And ye shall serve the LORD your God (Exodus 23:25) — service includeth prayer, praise, and supplication.'],
  [78,'The priests must bless the nation (Aaronic blessing)','Numbers 6:23','Prayer & Study','Priests','suspended','They shall be holy unto their God, and not profane the name of their God (Leviticus 21:6).'],
  [79,'Wear phylacteries on the forehead','Deuteronomy 6:8','Prayer & Study','Men','binding','The law shall be a sign on your forehead — constant reminder of Torah.'],
  [80,'Bind phylacteries on the arm','Deuteronomy 6:8','Prayer & Study','Men','binding','The law shall be a sign on your hand — governing all actions.'],
  [81,'Put up a Mezuzah on the doorposts','Deuteronomy 6:9','Prayer & Study','Both','binding','The law written on the doorposts of your house and gates.'],
  [82,'Each male must write or obtain a Torah scroll','Deuteronomy 31:19','Prayer & Study','Men','binding','Every Israelite man should have the Torah accessible and study it.'],
  [83,'The king must write a second Torah scroll for himself','Deuteronomy 17:18','Prayer & Study','Men','suspended','Awaits restoration of Israelite kingship.'],
  [84,'Have fringes (tzitzit) on the corners of your garments','Numbers 15:38','Prayer & Study','Both','binding','A reminder to keep all the commandments — wear tzitzit daily.'],
  [85,'Bless the Most High after meals','Deuteronomy 8:10','Prayer & Study','Both','binding','Give thanks after eating — recognize He provides all things.'],
  [86,'Circumcise every male on the eighth day','Leviticus 12:3','Circumcision','Men','binding','And ye shall circumcise the flesh of your foreskin; and it shall be a token of the covenant betwixt me and you (Genesis 17:11). This covenant is everlasting — it was never abolished.'],
  [87,'Rest on the seventh day — the Sabbath','Exodus 23:12','Sabbath','Both','binding','Remember the sabbath day, to keep it holy (Exodus 20:8). From even unto even shall ye celebrate your sabbath (Leviticus 23:32). The seventh day is the sabbath — never changed by any commandment of the Most High.'],
  [88,'Do no prohibited work on the seventh day','Exodus 20:10','Sabbath','Both','binding','No labor, commerce, or servile work on the Sabbath.'],
  [89,'The court must not inflict punishment on the Sabbath','Exodus 35:3','Sabbath','Both','suspended','Requires a functioning Israelite court system.'],
  [90,'Stay near home and within city bounds on the Sabbath','Exodus 16:29','Sabbath','Both','binding','Do not travel long distances — remain within your community.'],
  [91,'Remember and sanctify the Sabbath','Exodus 20:8','Sabbath','Both','binding','Keep it holy — set apart from all other days with blessing and rest.'],
  [92,'Perform self-denial and rest on Yom Kippur','Leviticus 23:32','Feast Days','Both','binding','Day of Atonement — fasting and affliction of soul required.'],
  [93,'Do no prohibited labor on Yom Kippur','Leviticus 23:32','Feast Days','Both','binding','The holiest day of the year — complete rest.'],
  [94,'Afflict yourself on Yom Kippur','Leviticus 16:29','Feast Days','Both','binding','Fast and humble yourself before the Most High.'],
  [95,'Do not eat or drink on Yom Kippur','Leviticus 23:29','Feast Days','Both','binding','A 24-hour fast from sundown to sundown.'],
  [96,'Rest on the first day of Passover','Leviticus 23:7','Feast Days','Both','binding','Passover (Pesach) — 14th of Abib. A holy convocation.'],
  [97,'Do no work on the first day of Passover','Leviticus 23:7','Feast Days','Both','binding','First day of Unleavened Bread is a high Sabbath.'],
  [98,'Rest on the seventh day of Passover','Leviticus 23:8','Feast Days','Both','binding','The last day of Unleavened Bread is also a high Sabbath.'],
  [99,'Do no work on the seventh day of Passover','Leviticus 23:8','Feast Days','Both','binding','High Sabbath — no servile work.'],
  [100,'Rest on the first day of Pentecost (Shavuot)','Leviticus 23:21','Feast Days','Both','binding','Feast of Weeks — 50 days after First Fruits. A high Sabbath.'],
  [101,'Do no work on the first day of Pentecost','Leviticus 23:21','Feast Days','Both','binding','Holy convocation — no servile work on Shavuot.'],
  [102,'Rest on Rosh Hashana — the Feast of Trumpets','Leviticus 23:24','Feast Days','Both','binding','1st of Tishri — a memorial of blowing of trumpets.'],
  [103,'Do no work on Rosh Hashana','Leviticus 23:25','Feast Days','Both','binding','A high Sabbath — no servile work.'],
  [104,'Rest on the first day of Sukkot — Feast of Tabernacles','Leviticus 23:35','Feast Days','Both','binding','15th of Tishri — a high Sabbath.'],
  [105,'Do no work on the first day of Sukkot','Leviticus 23:35','Feast Days','Both','binding','Holy convocation — the Feast of Tabernacles begins.'],
  [106,'Rest on the eighth day of Sukkot — Shmini Atzeret','Leviticus 23:36','Feast Days','Both','binding','The closing assembly — a high Sabbath.'],
  [107,'Do no work on the eighth day of Sukkot','Leviticus 23:36','Feast Days','Both','binding','No servile work on the last great day.'],
  [108,'Do not eat leaven past noon on Passover','Deuteronomy 16:3','Feast Days','Both','binding','Remove all leaven before the feast begins.'],
  [109,'Destroy all leaven on Passover','Exodus 12:15','Feast Days','Both','binding','Thoroughly search and remove all leavened bread from your home.'],
  [110,'Do not eat leaven all seven days of Passover','Exodus 13:3','Feast Days','Both','binding','Unleavened bread only for the full seven days.'],
  [111,'Do not eat anything containing leaven during Passover','Exodus 12:20','Feast Days','Both','binding','Check all food labels — leaven includes yeast in all forms.'],
  [112,'No leaven shall be found in your domain during Passover','Exodus 13:7','Feast Days','Both','binding','Your entire property must be free of leaven.'],
  [113,'Do not find leaven in your house all seven days of Passover','Exodus 12:19','Feast Days','Both','binding','Search the house completely before Passover begins.'],
  [114,'Eat matzoh on the first night of Passover','Exodus 12:18','Feast Days','Both','binding','Unleavened bread must be eaten on the night of Passover.'],
  [115,'On that night explain the meaning of Passover to your children','Exodus 13:8','Feast Days','Both','binding','And thou shalt shew thy son in that day, saying, This is done because of that which the LORD did unto me when I came forth out of Egypt (Exodus 13:8).'],
  [116,'Hear the Shofar on the Feast of Trumpets','Numbers 29:1','Feast Days','Both','binding','The ram\'s horn is blown on the 1st of Tishri.'],
  [117,'Dwell in a Sukkah for seven days during Sukkot','Leviticus 23:42','Feast Days','Both','binding','Build and dwell in a temporary shelter for the feast.'],
  [118,'Take up a Lulav and Etrog during Sukkot','Leviticus 23:40','Feast Days','Both','binding','The four species — palm, myrtle, willow, and citron.'],
  [119,'Families shall pay an annual half-shekel temple tax','Exodus 30:13','Feast Days','Both','suspended','Requires the Temple and its treasury.'],
  [120,'The courts must calculate the new month','Exodus 12:2','Feast Days','Both','suspended','Requires a functioning council of elders and judges of Israel to determine the new moon calendar.'],
  [121,'Cry out and blow trumpets before the Most High in times of catastrophe','Numbers 10:9','Feast Days','Both','binding','Sound the alarm and pray in times of national crisis.'],
  [122,'A man must contractually marry a woman before living with her','Deuteronomy 24:1','Marriage & Family','Men','binding','Thou shalt not commit fornication — a man must take a wife before he lie with her.'],
  [123,'There shall be no whore of the daughters of Israel, nor a sodomite of the sons of Israel','Deuteronomy 23:18','Marriage & Family','Both','binding','The hire of a whore and the price of a dog shall not come into the house of the LORD thy God (Deuteronomy 23:18).'],
  [124,'Do not withhold food, clothing, and relations from your wife','Exodus 21:10','Marriage & Family','Men','binding','Husbands have three covenant obligations to their wives.'],
  [125,'Be fruitful and multiply','Genesis 1:28','Marriage & Family','Men','binding','The first commandment ever given — have children.'],
  [126,'A divorced wife must receive a written bill of divorce','Deuteronomy 24:1','Marriage & Family','Men','binding','Divorce requires a formal written document — a Get.'],
  [127,'A man cannot remarry his divorced wife after she has remarried','Deuteronomy 24:4','Marriage & Family','Men','binding','An abomination after the wife has been with another man.'],
  [128,'Marry a childless brother\'s widow (levirate marriage)','Deuteronomy 25:5','Marriage & Family','Men','binding','To raise up the name of the deceased brother in Israel.'],
  [129,'Free a childless widow from levirate obligation if she requests','Deuteronomy 25:9','Marriage & Family','Women','binding','The Chalitza ceremony — releasing the widow if the brother refuses.'],
  [130,'A widow must not remarry until released from levirate obligation','Deuteronomy 25:5','Marriage & Family','Women','binding','She must wait for the brother-in-law to fulfill or release the obligation.'],
  [131,'If a man entice a maid that is not betrothed and lie with her, he shall surely endow her to be his wife','Exodus 22:16-17','Marriage & Family','Men','suspended','And if a man entice a maide that is not betrothed, and lie with her, he shall surely endow her to be his wife. If her father utterly refuse to give her unto him, he shall pay money according to the dowry of virgins (Exodus 22:16-17). This concerneth enticement — not compulsion — of an unbetrothed maid.'],
  [132,'He that humbleth a virgin and lieth with her must take her to wife','Deuteronomy 22:29','Marriage & Family','Men','suspended','Requires a functioning Israelite court.'],
  [133,'He must not divorce her','Deuteronomy 22:29','Marriage & Family','Men','suspended','Tied to the court ruling in law 132 — he may not put her away all his days.'],
  [134,'The slanderer must remain married to his wife','Deuteronomy 22:19','Marriage & Family','Men','suspended','Requires a functioning Israelite court.'],
  [135,'He must not divorce her','Deuteronomy 22:19','Marriage & Family','Men','suspended','Tied to the court ruling in law 134.'],
  [136,'Take procedures against a suspected adulteress (Sotah)','Numbers 5:30','Marriage & Family','Men','suspended','The Sotah procedure requires the Temple and functioning priesthood.'],
  [137,'A jealous husband must take his wife to the priests','Numbers 5:15','Marriage & Family','Men','suspended','Requires the Temple and Levitical priesthood.'],
  [138,'The suspected wife\'s offering must contain no oil or frankincense','Numbers 5:15','Marriage & Family','Women','suspended','Requires the Temple — the Sotah meal offering.'],
  [139,'Do not have relations with your mother','Leviticus 18:7','Sexual Laws','Men','binding','None of you shall approach to any that is near of kin to him, to uncover their nakedness: I am the LORD (Leviticus 18:6).'],
  [140,'Do not have relations with your father\'s wife','Leviticus 18:8','Sexual Laws','Men','binding','Including stepmother — forbidden.'],
  [141,'Do not have relations with your sister','Leviticus 18:9','Sexual Laws','Men','binding','Full or half sister — both forbidden.'],
  [142,'Do not have relations with your father\'s wife\'s daughter','Leviticus 18:11','Sexual Laws','Men','binding','Stepsister — forbidden.'],
  [143,'Do not have relations with your son\'s daughter','Leviticus 18:10','Sexual Laws','Men','binding','Granddaughter — an abomination.'],
  [144,'Do not have relations with your daughter','Leviticus 18:10','Sexual Laws','Men','binding','It is wickedness — they shall be cut off in the sight of their people.'],
  [145,'Do not have relations with your daughter\'s daughter','Leviticus 18:10','Sexual Laws','Men','binding','Granddaughter — forbidden.'],
  [146,'Do not marry a woman and her daughter','Leviticus 18:17','Sexual Laws','Men','binding','Wickedness — cannot marry mother and daughter.'],
  [147,'Do not marry a woman and her son\'s daughter','Leviticus 18:17','Sexual Laws','Men','binding','Forbidden — thou shalt not uncover his nakedness.'],
  [148,'Do not marry a woman and her daughter\'s daughter','Leviticus 18:17','Sexual Laws','Men','binding','Forbidden — thou shalt not uncover his nakedness.'],
  [149,'Do not have relations with your father\'s sister','Leviticus 18:12','Sexual Laws','Men','binding','Aunt on father\'s side — forbidden.'],
  [150,'Do not have relations with your mother\'s sister','Leviticus 18:13','Sexual Laws','Men','binding','Aunt on mother\'s side — forbidden.'],
  [151,'Do not have relations with your father\'s brother\'s wife','Leviticus 18:14','Sexual Laws','Men','binding','Uncle\'s wife — forbidden.'],
  [152,'Do not have relations with your son\'s wife','Leviticus 18:15','Sexual Laws','Men','binding','Daughter-in-law — forbidden.'],
  [153,'Do not have relations with your brother\'s wife','Leviticus 18:16','Sexual Laws','Men','binding','Exception for levirate marriage duty only.'],
  [154,'Do not have relations with your wife\'s sister while your wife lives','Leviticus 18:18','Sexual Laws','Men','binding','Forbidden while the wife is alive.'],
  [155,'Neither shalt thou lie with any beast — it is confusion','Leviticus 18:23','Sexual Laws','Men','binding','Whosoever lieth with a beast shall surely be put to death (Exodus 22:19).'],
  [156,'Neither shall any woman stand before a beast to lie down thereto','Leviticus 18:23','Sexual Laws','Women','binding','Whosoever lieth with a beast shall surely be put to death (Exodus 22:19).'],
  [157,'Thou shalt not lie with mankind as with womankind — it is abomination','Leviticus 18:22','Sexual Laws','Men','binding','Thou shalt not lie with mankind, as with womankind: it is abomination (Leviticus 18:22). Never repealed by any scripture.'],
  [158,'Thou shalt not lie with mankind as with womankind — it is abomination with your father','Leviticus 18:7','Sexual Laws','Men','binding','The nakedness of thy father shalt thou not uncover — doubly forbidden.'],
  [159,'Thou shalt not lie with mankind as with womankind — it is abomination with your father\'s brother','Leviticus 18:14','Sexual Laws','Men','binding','Forbidden — thou shalt not uncover his nakedness.'],
  [160,'Do not have relations with a married woman','Leviticus 18:20','Sexual Laws','Men','binding','Thou shalt not commit adultery — the seventh commandment (Exodus 20:14). Both shall be put to death (Leviticus 20:10).'],
  [161,'Do not have relations with a menstrually unclean woman','Leviticus 18:19','Sexual Laws','Men','binding','During the woman\'s period — strictly forbidden.'],
  [162,'Do not marry Gentiles','Deuteronomy 7:3','Marriage & Family','Both','binding','Intermarriage with the nations is forbidden — it leads to idol worship.'],
  [163,'Moabite and Ammonite males may not marry into Israel','Deuteronomy 23:4','Marriage & Family','Both','binding','Certain nations are permanently excluded from the congregation of Israel.'],
  [164,'Do not prevent third-generation Edomite converts from marrying into Israel','Deuteronomy 23:8-9','Marriage & Family','Both','binding','Third-generation Edomite converts may be permitted.'],
  [165,'Do not prevent third-generation Egyptian converts from marrying into Israel','Deuteronomy 23:8-9','Marriage & Family','Both','binding','Third-generation Egyptian converts may enter the congregation.'],
  [166,'A mamzer (child of forbidden union) cannot enter the congregation of Israel','Deuteronomy 23:3','Marriage & Family','Both','binding','Children born of certain forbidden unions cannot marry into Israel.'],
  [167,'A eunuch or sexually mutilated man may not enter the community','Deuteronomy 23:2','Marriage & Family','Men','binding','Sexual integrity required for full membership in the congregation.'],
  [168,'Thou shalt not offer unto the LORD that which is bruised, or crushed, or broken, or cut — neither make eunuchs of man nor beast','Leviticus 22:24','Sexual Laws','Men','binding','He that is wounded in the stones, or hath his privy member cut off, shall not enter into the congregation of the LORD (Deuteronomy 23:1).'],
  [169,'The High Priest must not marry a widow','Leviticus 21:14','Priestly Laws','Men','suspended','Requires a functioning High Priest and Levitical order.'],
  [170,'The High Priest must not have relations with a widow','Leviticus 21:15','Priestly Laws','Men','suspended','Requires a functioning High Priest.'],
  [171,'The High Priest must marry a virgin','Leviticus 21:13','Priestly Laws','Men','suspended','The High Priest\'s wife must be a virgin from Israel.'],
  [172,'A priest must not marry a divorcee','Leviticus 21:7','Priestly Laws','Men','suspended','They shall be holy unto their God, and not profane the name of their God (Leviticus 21:6).'],
  [173,'A priest may not take a wife that is a whore or profane','Leviticus 21:7','Priestly Laws','Men','suspended','They shall be holy unto their God, and not profane the name of their God (Leviticus 21:6).'],
  [174,'A priest must not marry a defiled woman','Leviticus 21:7','Priestly Laws','Men','suspended','They shall be holy unto their God, and not profane the name of their God (Leviticus 21:6).'],
  [175,'Do not have pleasurable physical contact with any forbidden woman','Leviticus 18:6','Sexual Laws','Men','binding','Includes all forms of sexual contact with forbidden relations.'],
  [176,'Examine animals to determine which are permitted as food','Leviticus 11:2','Dietary Laws','Both','binding','Animals must chew the cud AND have split hooves to be clean.'],
  [177,'Eat only clean birds','Deuteronomy 14:11','Dietary Laws','Both','binding','The list of forbidden birds includes eagles, owls, vultures, etc.'],
  [178,'Distinguish which sea creatures are fit to eat','Leviticus 11:9','Dietary Laws','Both','binding','Only fish with fins AND scales are clean — no shrimp, crab, or lobster.'],
  [179,'Distinguish which winged insects may be eaten','Leviticus 11:21','Dietary Laws','Both','binding','Certain locusts are permitted (Leviticus 11:21-22).'],
  [180,'Do not eat unclean animals — pig, camel, rabbit, etc.','Leviticus 11:4','Dietary Laws','Both','binding','They that sanctify themselves, and eat swine\'s flesh, and the abomination, shall be consumed together, saith the LORD (Isaiah 66:17). Swine\'s flesh is an abomination — it was never made clean.'],
  [181,'Do not eat forbidden birds','Leviticus 11:13','Dietary Laws','Both','binding','Eagles, vultures, owls, ravens, and others are forbidden.'],
  [182,'Do not eat sea creatures without fins and scales','Leviticus 11:11','Dietary Laws','Both','binding','Whatsoever hath no fins nor scales in the waters, that shall be an abomination unto you (Leviticus 11:12). This includeth shrimp, crab, lobster, catfish, and clams.'],
  [183,'Do not eat unclean flying insects','Deuteronomy 14:19','Dietary Laws','Both','binding','Most insects are forbidden as food.'],
  [184,'Do not eat swarming insects or unclean crawling creatures','Leviticus 11:41','Dietary Laws','Both','binding','Rodents, lizards, and crawling things are all forbidden.'],
  [185,'Do not eat maggots','Leviticus 11:44','Dietary Laws','Both','binding','Do not defile your body with unclean creatures.'],
  [186,'Do not eat snakes, scorpions, and worms found on the ground','Leviticus 11:42','Dietary Laws','Both','binding','Ground-crawling creatures are forbidden.'],
  [187,'Do not eat creatures that live in water other than clean fish','Leviticus 11:43','Dietary Laws','Both','binding','Only fish with fins and scales are permitted.'],
  [188,'Do not eat an animal that died without proper slaughter','Deuteronomy 14:21','Dietary Laws','Both','binding','That which dieth of itself, or that which is torn with beasts, ye shall not eat (Deuteronomy 14:21).'],
  [189,'Do not eat an ox that was condemned to be stoned','Exodus 21:28','Dietary Laws','Both','binding','And the ox shall be stoned... but his flesh shall not be eaten (Exodus 21:28).'],
  [190,'Do not eat meat of a mortally wounded animal','Exodus 22:30','Dietary Laws','Both','binding','Ye shall not eat any flesh that is torn of beasts in the field; ye shall cast it to the dogs (Exodus 22:31).'],
  [191,'Do not eat a limb torn off from a living creature','Deuteronomy 12:23','Dietary Laws','Both','binding','The blood is the life — respect for the animal.'],
  [192,'Do not eat blood','Leviticus 3:17','Dietary Laws','Both','binding','Ye shall eat the blood of no manner of flesh: for the life of all flesh is the blood thereof (Leviticus 17:14). All blood must be drained.'],
  [193,'Do not eat the forbidden fat of clean animals','Leviticus 3:17','Dietary Laws','Both','binding','Certain fat portions were reserved as offerings — not to be eaten.'],
  [194,'Do not eat the thigh muscle — the sciatic nerve','Genesis 32:33','Dietary Laws','Both','binding','A perpetual law from Jacob\'s wrestling with the angel.'],
  [195,'Do not eat milk and meat cooked together','Exodus 23:19','Dietary Laws','Both','binding','Do not boil a kid in its mother\'s milk — no cheeseburgers.'],
  [196,'Do not cook milk and meat together','Exodus 34:26','Dietary Laws','Both','binding','Repeated three times in Torah — this law is serious.'],
  [197,'Do not eat bread from the new grain harvest before the Temple offering','Leviticus 23:14','Dietary Laws','Both','suspended','The wave sheaf offering must come first — requires Temple.'],
  [198,'Roasted grains must be offered before being eaten from new harvest','Leviticus 23:14','Dietary Laws','Both','suspended','Requires the Temple wave offering at First Fruits.'],
  [199,'Do not eat ripe grains from the new harvest before the Temple offering','Leviticus 23:14','Dietary Laws','Both','suspended','Requires the First Fruits offering at the Temple.'],
  [200,'Do not eat the fruit of a tree for the first three years','Leviticus 19:23','Dietary Laws','Both','binding','The fruit is called uncircumcised for three years — forbidden.'],
  [201,'Do not eat diverse seeds planted in a vineyard','Deuteronomy 22:9','Dietary Laws','Both','binding','Mixed plantings in a vineyard make the produce forbidden.'],
  [202,'Do not eat untithed produce','Leviticus 22:15','Dietary Laws','Both','binding','Produce must be properly tithed before it can be eaten.'],
  [203,'Do not eat or drink anything offered as sacrifice to an idol','Deuteronomy 32:38','Dietary Laws','Both','binding','Food sacrificed to idols is forbidden — no exceptions.'],
  [204,'Ritually slaughter an animal properly before eating it','Deuteronomy 12:21','Dietary Laws','Both','binding','Animals must be properly slaughtered — not strangled or electrocuted.'],
  [205,'Do not slaughter an animal and its offspring on the same day','Leviticus 22:28','Dietary Laws','Both','binding','Compassion for mother and young — do not slaughter both in one day.'],
  [206,'Cover the blood of a slaughtered wild animal with dirt','Leviticus 17:13','Dietary Laws','Both','binding','The blood must be covered — it represents the life of the animal.'],
  [207,'Do not take a nesting mother bird with her eggs','Deuteronomy 22:6','Dietary Laws','Both','binding','Send away the mother — do not take her with her young.'],
  [208,'Release the mother bird before taking her eggs','Deuteronomy 22:7','Dietary Laws','Both','binding','This law carries the same reward as honoring parents — long life.'],
  [209,'Do not swear falsely in the Most High\'s Name','Leviticus 19:12','Oaths & Vows','Both','binding','Oaths made in His name must be kept without exception.'],
  [210,'Do not take His Name in vain','Exodus 20:7','Oaths & Vows','Both','binding','No false oaths, no empty use of His name.'],
  [211,'Thou shalt not deny possession of that which was entrusted or delivered unto thee','Leviticus 19:11','Oaths & Vows','Both','binding','Truth is foundational to Torah — all lying is forbidden.'],
  [212,'Neither swear falsely in denial of a monetary claim or possession','Leviticus 19:11','Oaths & Vows','Both','binding','False swearing is a sin against the Most High and your neighbor.'],
  [213,'Swear only in His Name to confirm truth when required','Deuteronomy 10:20','Oaths & Vows','Both','binding','When an oath is necessary, it must be in the Most High\'s name only.'],
  [214,'Keep your promises and vows to the Most High','Deuteronomy 23:24','Oaths & Vows','Both','binding','If you vow to the Most High, fulfill it without delay.'],
  [215,'Do not break oaths or vows','Numbers 30:3','Oaths & Vows','Both','binding','Your word is your bond — breaking a vow is sin.'],
  [216,'Have vows and oaths annulled according to law when necessary','Numbers 30:3','Oaths & Vows','Both','binding','A vow can be lawfully annulled under specific Torah conditions.'],
  [217,'The Nazirite must let his hair grow','Numbers 6:5','Vow of Separation','Men','binding','A voluntary vow of separation unto the Most High — the hair is the sign.'],
  [218,'The Nazirite must not cut his hair','Numbers 6:5','Vow of Separation','Men','binding','The uncut hair is the visible sign of the vow of separation.'],
  [219,'The Nazirite must not drink wine or wine mixtures','Numbers 6:3','Vow of Separation','Men','binding','Complete abstinence from all gthe humbling of a virgin products while under the vow.'],
  [220,'The Nazirite must not eat fresh gthe humbling of a virgins','Numbers 6:3','Vow of Separation','Men','binding','Nothing from the vine during the Nazirite period.'],
  [221,'The Nazirite must not eat raisins or drink gthe humbling of a virgin-steeped liquids','Numbers 6:3','Vow of Separation','Men','binding','All gthe humbling of a virgin-derived food and drink is forbidden under the vow.'],
  [222,'The Nazirite must not eat gthe humbling of a virgin seeds','Numbers 6:4','Vow of Separation','Men','binding','Even the seeds of the gthe humbling of a virgin are forbidden.'],
  [223,'The Nazirite must not eat gthe humbling of a virgin skins','Numbers 6:4','Vow of Separation','Men','binding','Every part of the gthe humbling of a virgin is forbidden — even the skin.'],
  [224,'A Nazirite may not enter where there is a dead person','Numbers 6:6','Vow of Separation','Men','binding','Nazirites maintain a higher level of ritual purity.'],
  [225,'A Nazirite must not come in contact with the dead','Numbers 6:7','Vow of Separation','Men','binding','Not even for a parent — the vow takes priority.'],
  [226,'A Nazirite must shave his head after completing his vowed service','Numbers 6:18','Vow of Separation','Men','suspended','The completion offering requires the Temple.'],
  [227,'Estimate the value of persons for whom offerings are paid','Leviticus 27:2','Vows & Valuations','Both','suspended','Requires the Temple and functioning priesthood for valuation offerings.'],
  [228,'Priests estimate the value of animal offerings','Leviticus 27:12-13','Vows & Valuations','Priests','suspended','Requires functioning Levitical priesthood.'],
  [229,'Priests estimate the value of consecrated houses','Leviticus 27:14','Vows & Valuations','Priests','suspended','Requires the Temple system.'],
  [230,'Determine the redemption value of a vowed field','Leviticus 27:16','Vows & Valuations','Both','suspended','Requires the Temple and Jubilee system.'],
  [231,'Fulfill the procedures of vowed possessions','Leviticus 27:28','Vows & Valuations','Both','suspended','Requires the Temple system for cherem (devoted things).'],
  [232,'Do not sell vowed possessions','Leviticus 27:28','Vows & Valuations','Both','suspended','Devoted things belong to the Most High — cannot be sold.'],
  [233,'Do not redeem vowed possessions','Leviticus 27:28','Vows & Valuations','Both','suspended','Devoted things cannot be bought back.'],
  [234,'Do not plant diverse seeds together (Kilayim)','Leviticus 19:19','Agriculture','Both','binding','No mixing of seed kinds in the same field.'],
  [235,'Do not plant grains or greens in a vineyard','Deuteronomy 22:9','Agriculture','Both','binding','Mixing crops in a vineyard is forbidden — makes all forfeit.'],
  [236,'Do not crossbreed animals','Leviticus 19:19','Agriculture','Both','binding','No hybrid breeding of different animal kinds.'],
  [237,'Do not work different kinds of animals together','Deuteronomy 22:10','Agriculture','Both','binding','Do not yoke an ox and donkey together.'],
  [238,'Do not wear cloth woven of both wool and linen (Shatnez)','Deuteronomy 22:11','Agriculture','Both','binding','Mixed fabric garments are forbidden by Torah.'],
  [239,'Leave the corners of the field (Peah) for the poor','Leviticus 19:10','Agriculture','Both','binding','The corners of your field belong to the poor and stranger.'],
  [240,'Leave fruit and grain for the poor — do not reap the corners','Leviticus 19:9','Agriculture','Both','binding','The poor have a right to the corners — do not take them.'],
  [241,'Leave gleanings from the harvest for the poor','Leviticus 19:9','Agriculture','Both','binding','What falls during harvesting belongs to the poor.'],
  [242,'Do not gather the gleanings — leave them for the poor','Leviticus 19:9','Agriculture','Both','binding','Do not go back to pick up what fell — leave it for the poor.'],
  [243,'Do not pick your vineyard bare','Leviticus 19:10','Agriculture','Both','binding','Leave some fruit for the poor and stranger.'],
  [244,'Do not gather the gleanings of a vineyard','Leviticus 19:10','Agriculture','Both','binding','Leave fallen gthe humbling of a virgins for the poor.'],
  [245,'Do not gather the fallen fruit of the vineyard','Leviticus 19:10','Agriculture','Both','binding','Fallen gthe humbling of a virgins belong to the poor — do not collect them.'],
  [246,'Do not pick unformed clusters of gthe humbling of a virgins','Leviticus 19:10','Agriculture','Both','binding','Unformed gthe humbling of a virgin clusters belong to the poor.'],
  [247,'Leave forgotten sheaves in the field for the poor','Deuteronomy 24:19','Agriculture','Both','binding','Do not go back for forgotten sheaves — leave them.'],
  [248,'Leave forgotten sheaves for the widow, alien, and orphan','Deuteronomy 24:19','Agriculture','Both','binding','The forgotten sheaf is the property of the vulnerable.'],
  [249,'Separate the tithe for the poor (Maaser Ani)','Deuteronomy 14:28','Agriculture','Both','binding','The poor tithe — given in the 3rd and 6th years of the Shemitah cycle.'],
  [250,'Give charity to those in need','Deuteronomy 15:8','Agriculture','Both','binding','For the poor shall never cease out of the land: therefore I command thee, saying, Thou shalt open thine hand wide unto thy brother (Deuteronomy 15:11).'],
  [251,'Do not withhold charity from those in need','Deuteronomy 15:7','Agriculture','Both','binding','Thou shalt surely give him, and thine heart shall not be grieved when thou givest unto him (Deuteronomy 15:10).'],
  [252,'Set aside a tithe for the priesthood from agricultural produce','Deuteronomy 18:4','Agriculture','Both','binding','Give the Terumah — the first portion — to the priests.'],
  [253,'The Levite must tithe on his tithe','Numbers 18:26','Agriculture','Priests','binding','Even the Levites must tithe on what they receive.'],
  [254,'Do not delay your agricultural offerings','Exodus 22:28','Agriculture','Both','binding','Bring your offerings on time — do not delay the first fruits.'],
  [255,'A layperson may not eat from a sacred donation (Terumah)','Leviticus 22:10','Agriculture','Both','suspended','Sacred donations are for the priesthood — requires Temple.'],
  [256,'A servant of a priest may not eat from a sacred donation','Leviticus 22:10','Agriculture','Both','suspended','Requires the Temple and active Levitical priesthood.'],
  [257,'An uncircumcised priest may not eat from a sacred donation','Exodus 12:48','Agriculture','Men','suspended','Requires the active Levitical priesthood.'],
  [258,'A priest in a state of impurity may not eat from a sacred donation','Leviticus 22:4','Agriculture','Priests','suspended','Requires the active Levitical priesthood and Temple system.'],
  [259,'A priest\'s daughter married to a layman may not eat from a sacred donation','Leviticus 22:12','Agriculture','Women','suspended','Requires the active Levitical priesthood.'],
  [260,'Levites are to receive earmarked tithes each planting year','Numbers 18:24','Agriculture','Both','binding','The Levitical tithe (Maaser Rishon) — 10% given to the Levites.'],
  [261,'Set aside the Second Tithe (Maaser Sheni)','Deuteronomy 14:22','Agriculture','Both','binding','A second 10% set aside — to be taken to Jerusalem or redeemed.'],
  [262,'Do not spend the Second Tithe on anything except food, drink, or ointment','Deuteronomy 26:14','Agriculture','Both','suspended','The Second Tithe was to be eaten in Jerusalem — requires Temple.'],
  [263,'Do not eat from the Second Tithe while unclean','Deuteronomy 26:14','Agriculture','Both','suspended','Requires the Temple system.'],
  [264,'A mourner must not eat the Second Tithe on the first day of mourning','Deuteronomy 26:14','Agriculture','Both','suspended','Requires the Temple system.'],
  [265,'Do not eat Second-Tithe grain outside Jerusalem','Deuteronomy 12:17','Agriculture','Both','suspended','Requires Jerusalem and the Temple.'],
  [266,'Do not consume Second-Tithe wine outside Jerusalem','Deuteronomy 12:17','Agriculture','Both','suspended','Requires Jerusalem and the Temple.'],
  [267,'Do not consume Second-Tithe oil outside Jerusalem','Deuteronomy 12:17','Agriculture','Both','suspended','Requires Jerusalem and the Temple.'],
  [268,'The fourth-year crops must be totally for holy purposes','Leviticus 19:24','Agriculture','Both','suspended','Fourth-year fruit was to be brought to Jerusalem — requires Temple.'],
  [269,'Read the confession of tithes every fourth and seventh year','Deuteronomy 26:13','Agriculture','Both','binding','The Vidui Maaser — a declaration of proper tithing.'],
  [270,'Bring the first fruits (Bikkurim) into the Temple','Exodus 23:19','Agriculture','Both','suspended','Requires the Temple and the Bikkurim offering.'],
  [271,'Priests must not eat the first fruits outside Jerusalem','Deuteronomy 12:17','Agriculture','Priests','suspended','Requires the Temple.'],
  [272,'Read the Torah portion when presenting first fruits','Deuteronomy 26:5','Agriculture','Both','suspended','The Bikkurim declaration — requires the Temple.'],
  [273,'When baking, set aside some dough for the priesthood (Challah)','Numbers 15:20','Agriculture','Both','binding','The dough offering — still practiced today.'],
  [274,'Give the shoulder, two cheeks, and stomach of a slaughtered animal to the priesthood','Deuteronomy 18:3','Agriculture','Both','suspended','The priestly portions — requires functioning Levitical priesthood.'],
  [275,'Give the first shearing of sheep to the priesthood','Deuteronomy 18:4','Agriculture','Both','suspended','Reishit HaGez — requires functioning Levitical priesthood.'],
  [276,'A father must redeem the firstborn son and give the money to the priesthood','Numbers 18:15','Agriculture','Men','binding','Pidyon Haben — redeeming the firstborn son is still practiced.'],
  [277,'Redeem each firstborn donkey with a lamb for the priesthood','Exodus 13:13','Agriculture','Both','binding','The firstborn donkey must be redeemed — still applicable.'],
  [278,'Break the neck of the firstborn donkey if the owner does not redeem it','Exodus 13:13','Agriculture','Both','binding','If not redeemed it must be destroyed — not used for personal gain.'],
  [279,'Rest the land during the seventh year (Shemitah)','Exodus 34:21','Agriculture','Both','binding','Every 7th year the land gets a Sabbath — no planting or harvesting.'],
  [280,'Do not work the land during the seventh year','Leviticus 25:4','Agriculture','Both','binding','No plowing, sowing, or pruning in the Shemitah year.'],
  [281,'Do not work with trees to produce fruit during the seventh year','Leviticus 25:4','Agriculture','Both','binding','Trees are also rested in the Shemitah year.'],
  [282,'Do not harvest wild crops in the seventh year','Leviticus 25:5','Agriculture','Both','binding','Even wild growth is not to be harvested commercially in Shemitah.'],
  [283,'Do not systematically pick fruit in the seventh year','Leviticus 25:5','Agriculture','Both','binding','Fruit of the Shemitah year belongs to all — not to be farmed commercially.'],
  [284,'Leave all Shemitah produce untouched for all to access','Exodus 23:11','Agriculture','Both','binding','The land\'s produce in the 7th year is ownerless and open to all.'],
  [285,'Relax all loans in the seventh year (Shemitah)','Deuteronomy 15:2','Agriculture','Both','binding','All debts between Israelites are cancelled every 7 years.'],
  [286,'Do not pressure the debtor in the seventh year','Deuteronomy 15:2','Agriculture','Both','binding','Do not demand payment when the Shemitah cancels the debt.'],
  [287,'Do not refuse to lend near the year of remission out of fear of loss','Deuteronomy 15:9','Agriculture','Both','binding','Do not use the Shemitah as an excuse not to help your brother.'],
  [288,'The court must count and determine the year of Jubilee','Leviticus 25:8','Agriculture','Both','suspended','Requires a functioning council of elders and judges of Israel and Israelite national system.'],
  [289,'The court must sanctify the fiftieth year — the Jubilee','Leviticus 25:10','Agriculture','Both','suspended','Requires a functioning council of elders and judges of Israel.'],
  [290,'Sound the ram\'s horn on Yom Kippur of the Jubilee year to free slaves','Leviticus 25:9','Agriculture','Both','suspended','Requires the Jubilee system and Israelite national governance.'],
  [291,'Do not work the land during the fiftieth year (Jubilee)','Leviticus 25:11','Agriculture','Both','suspended','Requires the Jubilee system.'],
  [292,'Do not reap or harvest in the fiftieth year','Leviticus 25:11','Agriculture','Both','suspended','Requires the Jubilee system.'],
  [293,'Do not pick gthe humbling of a virgins in the usual way in the fiftieth year','Leviticus 25:11','Agriculture','Both','suspended','Requires the Jubilee system.'],
  [294,'Follow the laws of sold and family properties','Leviticus 25:24','Agriculture','Both','suspended','Land redemption laws — require the Jubilee and national system.'],
  [295,'Do not sell land in Israel in perpetuity','Leviticus 25:23','Agriculture','Both','identity','The land belongs to the Most High — it cannot be permanently sold.'],
  [296,'Follow the laws pertaining to houses in walled cities','Leviticus 25:29','Agriculture','Both','suspended','Requires the Jubilee and Israelite land system.'],
  [297,'The Levites have no inheritance — they live in designated cities','Deuteronomy 18:1','Agriculture','Priests','identity','The Most High is the Levites\' inheritance — no land allotment.'],
  [298,'Levites will not partake in the spoils of war','Deuteronomy 18:1','Agriculture','Priests','suspended','Requires a functioning Israelite military system.'],
  [299,'Levites are to be given cities and surrounding fields','Numbers 35:2','Agriculture','Both','suspended','Requires national Israelite land distribution.'],
  [300,'Do not sell the fields of the Levites','Leviticus 25:34','Agriculture','Priests','identity','Levite cities are their permanent inheritance — cannot be sold.'],
  [301,'Build a Sanctuary for the Most High','Exodus 25:8','Temple & Sanctuary','Both','suspended','The Temple will be rebuilt in Jerusalem — this law awaits fulfillment.'],
  [302,'Do not build the altar with stones hewn by metal','Exodus 20:22','Temple & Sanctuary','Both','suspended','Requires the Temple.'],
  [303,'Do not climb steps to the altar','Exodus 20:23','Temple & Sanctuary','Both','suspended','Requires the Temple.'],
  [304,'Show reverence for the Temple','Leviticus 19:30','Temple & Sanctuary','Both','suspended','The Temple no longer stands — awaits restoration.'],
  [305,'Levites shall guard the Temple area','Numbers 18:3','Temple & Sanctuary','Priests','suspended','Requires the Temple.'],
  [306,'Do not leave the Temple unguarded','Numbers 18:5','Temple & Sanctuary','Priests','suspended','Requires the Temple.'],
  [307,'Blend the anointing oil','Exodus 30:31','Temple & Sanctuary','Priests','suspended','Requires the Temple and Levitical priesthood.'],
  [308,'Do not duplicate the formula for the anointing oil','Exodus 30:32','Temple & Sanctuary','Both','suspended','The sacred formula is reserved for the Temple only.'],
  [309,'Do not anoint anyone who is not a priest or king with the anointing oil','Exodus 30:32','Temple & Sanctuary','Both','suspended','Requires the Temple.'],
  [310,'Do not replicate the incense formula','Exodus 30:37','Temple & Sanctuary','Both','suspended','The sacred incense formula is reserved for Temple use only.'],
  [311,'Do not burn anything on the altar besides incense','Exodus 30:9','Temple & Sanctuary','Both','suspended','Requires the Temple altar.'],
  [312,'The Levites carry the ark on their shoulders','Numbers 7:9','Temple & Sanctuary','Priests','suspended','Requires the ark and Levitical order.'],
  [313,'Do not remove the poles from the ark','Exodus 25:15','Temple & Sanctuary','Both','suspended','Requires the ark.'],
  [314,'The Levites must work in the Temple','Numbers 18:23','Temple & Sanctuary','Priests','suspended','Requires the Temple.'],
  [315,'There are specified duties for the Levites','Numbers 18:3','Temple & Sanctuary','Priests','suspended','Requires the Temple.'],
  [316,'The priest must be treated as sacred','Leviticus 21:8','Temple & Sanctuary','Priests','suspended','Requires functioning Levitical priesthood.'],
  [317,'The priestly work shifts must be equal during holidays','Deuteronomy 18:6-8','Temple & Sanctuary','Priests','suspended','Requires the Temple.'],
  [318,'The priests must wear their priestly garments during service','Exodus 28:2','Temple & Sanctuary','Priests','suspended','Requires the Temple and Levitical order.'],
  [319,'The priestly garments must not be torn','Exodus 28:32','Temple & Sanctuary','Priests','suspended','Requires the Temple.'],
  [320,'The breastplate must not be loosened from the ephod','Exodus 28:28','Temple & Sanctuary','Priests','suspended','Requires the Temple and high priestly garments.'],
  [321,'A priest must not enter the Temple when drunk','Leviticus 10:9','Temple & Sanctuary','Priests','suspended','Requires the Temple.'],
  [322,'A priest must not enter the Temple with unkempt hair','Leviticus 10:6','Temple & Sanctuary','Priests','suspended','Requires the Temple.'],
  [323,'A priest must not enter the Temple with torn clothes','Leviticus 10:6','Temple & Sanctuary','Priests','suspended','Requires the Temple.'],
  [324,'A priest must not enter the sanctuary without reason','Leviticus 16:2','Temple & Sanctuary','Priests','suspended','Requires the Temple.'],
  [325,'A priest must not leave the Temple during the service','Leviticus 10:7','Temple & Sanctuary','Priests','suspended','Requires the Temple.'],
  [326,'Send the impure from the Temple','Numbers 5:2','Temple & Sanctuary','Both','suspended','Requires the Temple.'],
  [327,'Impure persons must not enter the Temple','Numbers 5:3','Temple & Sanctuary','Both','suspended','Requires the Temple.'],
  [328,'Unclean persons must not enter the Temple Mount area','Deuteronomy 23:11','Temple & Sanctuary','Both','suspended','Requires the Temple.'],
  [329,'Unclean priests cannot do Temple service','Leviticus 22:2','Temple & Sanctuary','Priests','suspended','Requires the Temple.'],
  [330,'An impure priest must not return to service until after sundown','Leviticus 21:6','Temple & Sanctuary','Priests','suspended','Requires the Temple.'],
  [331,'A priest must wash his hands and feet before ministering','Exodus 30:19','Temple & Sanctuary','Priests','suspended','Requires the Temple laver.'],
  [332,'A blemished priest must not enter the Temple','Leviticus 21:23','Temple & Sanctuary','Priests','suspended','Requires the Temple.'],
  [333,'A blemished priest must not serve','Leviticus 21:17','Temple & Sanctuary','Priests','suspended','Requires the Temple.'],
  [334,'A temporarily blemished priest must not serve','Leviticus 21:18','Temple & Sanctuary','Priests','suspended','Requires the Temple.'],
  [335,'A non-priest must not serve at the altar','Numbers 18:4','Temple & Sanctuary','Both','suspended','Requires the Temple.'],
  [336,'Blemished animals are unacceptable as offerings','Leviticus 22:21','Sacrifice Laws','Both','suspended','Requires the Temple and sacrifice system.'],
  [337,'Do not dedicate a blemished animal for the altar','Leviticus 22:20','Sacrifice Laws','Both','suspended','Requires the Temple.'],
  [338,'An animal with a discharge must not be slaughtered for offerings','Leviticus 22:22','Sacrifice Laws','Both','suspended','Requires the Temple.'],
  [339,'Do not sprinkle the blood of a disabled animal','Leviticus 22:24','Sacrifice Laws','Priests','suspended','Requires the Temple.'],
  [340,'Do not burn the fat of a defective animal','Leviticus 22:22','Sacrifice Laws','Priests','suspended','Requires the Temple.'],
  [341,'Do not offer an animal with a temporary blemish','Deuteronomy 17:1','Sacrifice Laws','Both','suspended','Requires the Temple.'],
  [342,'Do not accept defective offerings even from foreigners','Leviticus 22:25','Sacrifice Laws','Both','suspended','Requires the Temple.'],
  [343,'Do not inflict wounds upon dedicated animals','Leviticus 22:21','Sacrifice Laws','Both','suspended','Requires the Temple.'],
  [344,'Redeem disqualified dedicated animals','Deuteronomy 12:15','Sacrifice Laws','Both','suspended','Requires the Temple.'],
  [345,'Offer animals that are at least eight days old','Leviticus 22:27','Sacrifice Laws','Both','suspended','Requires the Temple.'],
  [346,'Do not offer animals purchased with a harlot\'s fees','Deuteronomy 23:19','Sacrifice Laws','Both','suspended','Requires the Temple.'],
  [347,'Do not burn yeast or honey on the altar','Leviticus 2:11','Sacrifice Laws','Both','suspended','Requires the Temple altar.'],
  [348,'Salt all sacrifices','Leviticus 2:13','Sacrifice Laws','Both','suspended','Requires the Temple altar.'],
  [349,'Do not omit the salt from grain offerings','Leviticus 2:13','Sacrifice Laws','Both','suspended','Requires the Temple.'],
  [350,'Follow the burnt offering (Olah) procedures','Leviticus 1:3','Sacrifice Laws','Men','suspended','Requires the Temple.'],
  [351,'Do not eat the meat of a burnt offering','Deuteronomy 12:17','Sacrifice Laws','Men','suspended','Requires the Temple.'],
  [352,'Carry out the procedure for a sin offering (Chatat)','Leviticus 6:18','Sacrifice Laws','Priests','suspended','Requires the Temple and Levitical priesthood.'],
  [353,'Do not eat the meat of a sin offering burned in fire','Leviticus 6:23','Sacrifice Laws','Priests','suspended','Requires the Temple.'],
  [354,'The priest shall not cut off the head of a bird sin offering','Leviticus 5:8','Sacrifice Laws','Priests','suspended','Requires the Temple.'],
  [355,'Follow the procedures of the guilt offering (Asham)','Leviticus 7:1','Sacrifice Laws','Priests','suspended','Requires the Temple.'],
  [356,'The priests must eat the sacrificed meat in the Temple','Exodus 29:33','Sacrifice Laws','Priests','suspended','Requires the Temple.'],
  [357,'Priests must not eat the sacrificial meat outside the Temple','Deuteronomy 12:17','Sacrifice Laws','Priests','suspended','Requires the Temple.'],
  [358,'A non-priest must not eat the sacrificial meat','Exodus 29:33','Sacrifice Laws','Both','suspended','Requires the Temple.'],
  [359,'Follow the procedure of the peace offering (Shelamim)','Leviticus 7:11','Sacrifice Laws','Priests','suspended','Requires the Temple.'],
  [360,'Do not eat minor sacrifices before sprinkling the blood','Deuteronomy 12:17','Sacrifice Laws','Both','suspended','Requires the Temple.'],
  [361,'Bring meal offerings in the prescribed manner','Leviticus 2:1','Sacrifice Laws','Both','suspended','Requires the Temple.'],
  [362,'Do not put oil on the meal offerings of wrongdoers','Leviticus 5:11','Sacrifice Laws','Priests','suspended','Requires the Temple.'],
  [363,'Do not put frankincense on the meal offerings of wrongdoers','Leviticus 5:11','Sacrifice Laws','Priests','suspended','Requires the Temple.'],
  [364,'Do not eat the cereal offering of the high priest','Leviticus 6:16','Sacrifice Laws','Priests','suspended','Requires the Temple.'],
  [365,'Do not bake meal offerings with leaven','Leviticus 6:10','Sacrifice Laws','Priests','suspended','Requires the Temple.'],
  [366,'The priests must eat the remains of the meal offerings','Leviticus 6:9','Sacrifice Laws','Priests','suspended','Requires the Temple.'],
  [367,'Bring all freewill offerings to the Temple','Deuteronomy 12:5-6','Sacrifice Laws','Both','suspended','Requires the Temple.'],
  [368,'Do not withhold payment fulfilling a vow to the Most High','Deuteronomy 23:22','Sacrifice Laws','Both','binding','Fulfill your vows to the Most High without delay (Ecclesiastes 5:4).'],
  [369,'Offer all sacrifices in the Temple','Deuteronomy 12:11','Sacrifice Laws','Both','suspended','Requires the Temple.'],
  [370,'Bring all votive offerings to the Temple','Deuteronomy 12:26','Sacrifice Laws','Both','suspended','Requires the Temple.'],
  [371,'Do not slaughter sacrifices outside the Temple courtyard','Leviticus 17:4','Sacrifice Laws','Both','suspended','Requires the Temple.'],
  [372,'Do not offer any sacrifices outside the Temple courtyard','Deuteronomy 12:13','Sacrifice Laws','Both','suspended','Requires the Temple.'],
  [373,'Offer two lambs every day as burnt offerings','Numbers 28:3','Sacrifice Laws','Priests','suspended','Requires the Temple.'],
  [374,'Light a fire on the altar every day','Leviticus 6:5','Sacrifice Laws','Priests','suspended','Requires the Temple altar.'],
  [375,'Do not extinguish the altar fire','Leviticus 6:5','Sacrifice Laws','Priests','suspended','Requires the Temple.'],
  [376,'Remove the ashes from the altar every day','Leviticus 6:3','Sacrifice Laws','Priests','suspended','Requires the Temple.'],
  [377,'Burn incense every day','Exodus 30:7','Sacrifice Laws','Priests','suspended','Requires the Temple altar.'],
  [378,'Keep the menorah burning every day','Exodus 27:21','Sacrifice Laws','Priests','suspended','Requires the Temple and Levitical order.'],
  [379,'The High Priest must bring a meal offering every day','Leviticus 6:13','Sacrifice Laws','Priests','suspended','Requires the Temple.'],
  [380,'Bring two additional lambs as burnt offerings on the Sabbath','Numbers 28:9','Sacrifice Laws','Priests','suspended','Requires the Temple.'],
  [381,'Make and present the showbread every Sabbath','Exodus 25:30','Sacrifice Laws','Priests','suspended','Requires the Temple.'],
  [382,'Bring additional offerings on the new moon','Numbers 28:11','Sacrifice Laws','Priests','suspended','Requires the Temple.'],
  [383,'Bring additional offerings on Passover','Numbers 28:19','Sacrifice Laws','Priests','suspended','Requires the Temple.'],
  [384,'Bring a wave offering from the meal of the new wheat at First Fruits','Leviticus 23:10','Sacrifice Laws','Priests','suspended','Requires the Temple — First Fruits offering.'],
  [385,'Count 50 days from First Fruits to Pentecost (Counting the Omer)','Leviticus 23:15','Feast Days','Both','binding','The counting of the Omer — 49 days between the feasts.'],
  [386,'Bring an additional offering on Shavuot','Numbers 28:26','Sacrifice Laws','Priests','suspended','Requires the Temple.'],
  [387,'Offer two loaves to accompany the Shavuot sacrifices','Leviticus 23:18','Sacrifice Laws','Priests','suspended','Requires the Temple.'],
  [388,'Bring additional offerings on Rosh Hashana','Numbers 29:2','Sacrifice Laws','Priests','suspended','Requires the Temple.'],
  [389,'Bring additional offerings on Yom Kippur','Numbers 29:8','Sacrifice Laws','Priests','suspended','Requires the Temple.'],
  [390,'Bring additional offerings on Sukkot','Numbers 29:13','Sacrifice Laws','Priests','suspended','Requires the Temple.'],
  [391,'Bring additional offerings on Shmini Atzeret','Numbers 29:35','Sacrifice Laws','Priests','suspended','Requires the Temple.'],
  [392,'Do not eat any unfit sacrifices','Deuteronomy 14:3','Sacrifice Laws','Both','suspended','Requires the Temple.'],
  [393,'Do not eat sacrifices offered with improper intentions','Leviticus 7:18','Sacrifice Laws','Both','suspended','Requires the Temple.'],
  [394,'Eat the Thanksgiving sacrifice on the day it was sacrificed','Leviticus 22:30','Sacrifice Laws','Both','suspended','Requires the Temple.'],
  [395,'Do not eat leftover sacrifices (Notar)','Leviticus 19:8','Sacrifice Laws','Both','suspended','Requires the Temple.'],
  [396,'Do not eat from sacrifices that have become impure','Leviticus 7:19','Sacrifice Laws','Both','suspended','Requires the Temple.'],
  [397,'An unclean person cannot eat from sacrifices','Leviticus 7:20','Sacrifice Laws','Both','suspended','Requires the Temple.'],
  [398,'Sacrificial remains must be burned on the third day','Leviticus 7:17','Sacrifice Laws','Both','suspended','Requires the Temple.'],
  [399,'Impure sacrifices must be burnt','Leviticus 7:19','Sacrifice Laws','Both','suspended','Requires the Temple.'],
  [400,'Follow the priestly rituals of Yom Kippur','Leviticus 16:3','Sacrifice Laws','Priests','suspended','The High Priest\'s Yom Kippur ritual requires the Temple.'],
  [401,'One who misuses sacred property must bring a penalty sacrifice','Leviticus 5:16','Sacrifice Laws','Both','suspended','Requires the Temple.'],
  [402,'Do not work consecrated animals','Deuteronomy 15:19','Sacrifice Laws','Both','suspended','Requires the Temple system.'],
  [403,'Do not shear the fleece of consecrated animals','Deuteronomy 15:19','Sacrifice Laws','Both','suspended','Requires the Temple system.'],
  [404,'Slaughter the Paschal sacrifice at the appointed time','Exodus 12:6','Sacrifice Laws','Men','suspended','Passover lamb sacrifice requires the Temple. Passover observance continues.'],
  [405,'Do not slaughter the Paschal sacrifice while possessing leaven','Exodus 23:18','Sacrifice Laws','Men','suspended','Requires the Temple.'],
  [406,'Do not leave the fat of the Paschal offering overnight','Exodus 23:18','Sacrifice Laws','Men','suspended','Requires the Temple.'],
  [407,'Slaughter the second Paschal Lamb (Pesach Sheni)','Numbers 9:11','Sacrifice Laws','Men','suspended','Requires the Temple.'],
  [408,'The Paschal Lamb must be eaten with matzoh on the night it was slaughtered','Exodus 12:8','Sacrifice Laws','Both','suspended','Requires the Temple.'],
  [409,'Eat the second Paschal Lamb on the night of the 15th of Iyar','Numbers 9:11','Sacrifice Laws','Both','suspended','Requires the Temple.'],
  [410,'Roast the Paschal Lamb — do not eat it raw or boiled','Exodus 12:9','Sacrifice Laws','Both','suspended','Requires the Temple.'],
  [411,'No part of the Paschal Lamb may be removed from the house','Exodus 12:46','Sacrifice Laws','Both','suspended','Requires the Temple.'],
  [412,'An apostate must not eat from the Paschal Lamb','Exodus 12:43','Sacrifice Laws','Both','suspended','Requires the Temple.'],
  [413,'A hired servant or traveler must not eat from the Paschal Lamb','Exodus 12:45','Sacrifice Laws','Both','suspended','Requires the Temple.'],
  [414,'An uncircumcised male must not eat from the Paschal Lamb','Exodus 12:48','Sacrifice Laws','Men','suspended','Requires the Temple.'],
  [415,'No bone of the Paschal Lamb shall be broken','Exodus 12:46','Sacrifice Laws','Both','suspended','Requires the Temple — fulfilled prophetically in Yeshua (John 19:36).'],
  [416,'Do not break any bones from the second Paschal offering','Numbers 9:12','Sacrifice Laws','Both','suspended','Requires the Temple.'],
  [417,'Do not leave any of the Lamb over until morning','Exodus 12:10','Sacrifice Laws','Both','suspended','Requires the Temple.'],
  [418,'Do not leave the second Paschal meat until morning','Numbers 9:12','Sacrifice Laws','Both','suspended','Requires the Temple.'],
  [419,'Eat the Passover meat entirely on the night it is offered','Deuteronomy 16:4','Sacrifice Laws','Both','suspended','Requires the Temple.'],
  [420,'Be seen at the Temple three times a year','Deuteronomy 16:16','Sacrifice Laws','Men','suspended','Requires the Temple — the three pilgrimage feasts.'],
  [421,'Celebrate and bring a peace offering on the three pilgrimage festivals','Exodus 23:14','Sacrifice Laws','Men','suspended','Requires the Temple.'],
  [422,'Rejoice on the three festivals','Deuteronomy 16:14','Feast Days','Both','binding','Rejoice on Passover, Shavuot, and Sukkot — this is still required today.'],
  [423,'Do not appear at the Temple for festivals without offerings','Deuteronomy 16:16','Sacrifice Laws','Men','suspended','Requires the Temple.'],
  [424,'Do not refrain from rejoicing with and giving gifts to the Levites','Deuteronomy 12:19','Social Laws','Both','binding','Honor and provide for the Levites at the feast seasons.'],
  [425,'Every seven years on Sukkot, assemble all the people and read the law (Hakhel)','Deuteronomy 31:12','Feast Days','Both','binding','The public reading of Torah — still applicable today.'],
  [426,'Consecrate the firstborn of man and beast to the Most High','Exodus 13:12','Sacrifice Laws','Both','binding','The principle of consecrating firstborn remains binding.'],
  [427,'Priests must not eat firstborn animals outside Jerusalem','Deuteronomy 12:17','Sacrifice Laws','Priests','suspended','Requires the Temple.'],
  [428,'The firstborn of clean animals cannot be redeemed','Numbers 18:17','Sacrifice Laws','Both','suspended','Requires the Temple.'],
  [429,'Separate the animal tithe','Leviticus 27:32','Sacrifice Laws','Both','suspended','Animal tithe requires the Temple system.'],
  [430,'Do not exchange a good animal for a bad one for the tithe','Leviticus 27:33','Sacrifice Laws','Both','suspended','Requires the Temple.'],
  [431,'Every person must bring a sin offering for transgression','Leviticus 4:27','Sacrifice Laws','Both','suspended','Animal sin offerings require the Temple. Repentance and prayer continue.'],
  [432,'An unintentional sin requires a sin offering when discovered','Leviticus 5:17-18','Sacrifice Laws','Both','suspended','Repentance and prayer substitute until Temple restoration.'],
  [433,'A guilt offering is required when one deals deceitfully','Leviticus 5:25','Sacrifice Laws','Both','suspended','Requires the Temple — restitution and repentance still required.'],
  [434,'For certain sins the wealthy offer an animal; the poor offer birds or meal','Leviticus 5:7-11','Sacrifice Laws','Both','suspended','Requires the Temple.'],
  [435,'The court must bring an offering when it rules in error','Leviticus 4:13','Sacrifice Laws','Both','suspended','Requires the Temple and a functioning council of elders and judges of Israel.'],
  [436,'A woman with an irregular discharge must bring an offering after immersion','Leviticus 15:28-29','Sacrifice Laws','Women','suspended','Requires the Temple.'],
  [437,'A woman who gives birth must bring an offering after immersion','Leviticus 12:6','Sacrifice Laws','Women','suspended','Requires the Temple.'],
  [438,'A man cured of a chronic discharge must bring an offering','Leviticus 15:13-14','Sacrifice Laws','Men','suspended','Requires the Temple.'],
  [439,'One cured of a skin disease must bring an offering after immersion','Leviticus 14:10','Sacrifice Laws','Both','suspended','Requires the Temple.'],
  [440,'Do not substitute another beast for one scheduled for sacrifice','Leviticus 27:10','Sacrifice Laws','Both','suspended','Requires the Temple.'],
  [441,'The substituted animal and the original both retain consecration','Leviticus 27:10','Sacrifice Laws','Both','suspended','Requires the Temple.'],
  [442,'Do not change consecrated animals from one type of offering to another','Leviticus 27:26','Sacrifice Laws','Both','suspended','Requires the Temple.'],
  [443,'Everyone under a roof with a corpse is unclean','Numbers 19:14','Ritual Purity','Both','binding','Corpse impurity — one of the most severe forms of uncleanness.'],
  [444,'Carry out the procedure of the Red Heifer','Numbers 19:9','Ritual Purity','Priests','suspended','Requires a red heifer, the Temple, and Levitical priests.'],
  [445,'A clean person sprinkles purification water on those who are unclean','Numbers 19:21','Ritual Purity','Both','suspended','Requires the Red Heifer ashes — suspended without Temple.'],
  [446,'The priest\'s role governs matters of skin disease','Leviticus 13:12','Ritual Purity','Priests','suspended','Requires functioning Levitical priesthood for diagnosis.'],
  [447,'The afflicted must not remove the signs of impurity','Deuteronomy 24:8','Ritual Purity','Both','binding','Do not hide or remove signs of skin disease — follow Torah instructions.'],
  [448,'The afflicted must not shave signs of impurity from his hair','Leviticus 13:33','Ritual Purity','Both','binding','Do not shave the afflicted area before the priest\'s inspection.'],
  [449,'A person with skin disease must declare himself unclean','Leviticus 13:45','Ritual Purity','Both','binding','Tear your clothes, let your hair grow long, and warn others — unclean.'],
  [450,'Carry out the procedure for purifying the person with skin disease','Leviticus 14:2','Ritual Purity','Priests','suspended','Requires the Temple and Levitical priesthood.'],
  [451,'The diseased person must shave off all his hair prior to purification','Leviticus 14:9','Ritual Purity','Both','suspended','Requires the Temple purification ceremony.'],
  [452,'Discover when a leprous infection is on a garment','Leviticus 13:47','Ritual Purity','Both','binding','Inspect garments for signs of infectious contamination.'],
  [453,'Discover when a house is infected by a skin disease','Leviticus 14:35','Ritual Purity','Both','binding','Inspect homes for signs of spreading contamination.'],
  [454,'Observe the laws of menstrual impurity (Niddah)','Leviticus 15:19','Ritual Purity','Women','binding','A woman is unclean for 7 days during her period — immersion required after.'],
  [455,'Observe the laws of impurity caused by childbirth','Leviticus 12:2','Ritual Purity','Women','binding','A woman is unclean after giving birth — varying days of purification.'],
  [456,'Observe the laws of impurity from an irregular discharge','Leviticus 15:25','Ritual Purity','Women','binding','Any unusual discharge renders uncleanness — immersion required.'],
  [457,'Observe the laws of impurity from a man\'s chronic discharge (Zav)','Leviticus 15:3','Ritual Purity','Men','binding','A man with a discharge is unclean — must count days and immerse.'],
  [458,'Observe the laws of impurity from contact with dead animals','Leviticus 11:39','Ritual Purity','Both','binding','Touching a dead unclean animal renders you unclean until evening.'],
  [459,'Observe the laws of impurity from contact with swarming creatures','Leviticus 11:29','Ritual Purity','Both','binding','Contact with certain swarming creatures causes uncleanness.'],
  [460,'Observe the laws of impurity of a seminal emission','Leviticus 15:16','Ritual Purity','Men','binding','A man who has a seminal emission is unclean until evening — must immerse.'],
  [461,'Observe the laws of impurity concerning liquid and solid foods','Leviticus 11:34','Ritual Purity','Both','binding','Impure liquids and foods can transmit uncleanness.'],
  [462,'Every impure person must immerse in a ritual bath (mikveh) to become pure','Leviticus 15:16','Ritual Purity','Both','binding','Immersion in living water is required to restore cleanness.'],
  [463,'The court must judge damages incurred by a goring ox','Exodus 21:28','Civil & Criminal','Both','suspended','Requires a functioning Israelite court.'],
  [464,'The court must judge damages incurred by an animal eating in another\'s field','Exodus 22:4','Civil & Criminal','Both','suspended','Requires a functioning Israelite court.'],
  [465,'The court must judge damages incurred by an open pit','Exodus 21:33','Civil & Criminal','Both','suspended','Requires a functioning Israelite court.'],
  [466,'The court must judge damages incurred by fire','Exodus 22:5','Civil & Criminal','Both','suspended','Requires a functioning Israelite court.'],
  [467,'Do not steal money stealthily','Leviticus 19:11','Civil & Criminal','Both','binding','The 8th commandment — theft in any form is forbidden.'],
  [468,'The court must implement punitive measures against the thief','Exodus 21:37','Civil & Criminal','Both','suspended','Restitution laws require a functioning Israelite court.'],
  [469,'Ensure your scales and weights are accurate','Leviticus 19:36','Civil & Criminal','Both','binding','Dishonest weights are an abomination (Proverbs 11:1).'],
  [470,'Do not commit injustice with scales and weights','Leviticus 19:35','Civil & Criminal','Both','binding','Fair commerce is commanded — no price gouging or fraud.'],
  [471,'Do not possess inaccurate weights even if not for use','Deuteronomy 25:13','Civil & Criminal','Both','binding','Having fraudulent weights is itself a violation — intent does not matter.'],
  [472,'Do not move a boundary marker to steal property','Deuteronomy 19:14','Civil & Criminal','Both','binding','Do not manipulate property lines or defraud someone of their land.'],
  [473,'Thou shalt not steal a man — he that stealeth a man and selleth him shall surely be put to death','Exodus 20:13','Civil & Criminal','Both','binding','And he that stealeth a man, and selleth him, or if he be found in his hand, he shall surely be put to death (Exodus 21:16).'],
  [474,'Do not rob openly','Leviticus 19:13','Civil & Criminal','Both','binding','Do not take by force what belongs to another.'],
  [475,'Do not withhold wages or fail to repay a debt','Leviticus 19:13','Civil & Criminal','Both','binding','Pay workers what is owed — same day for day laborers.'],
  [476,'Do not covet and scheme to acquire another\'s possession','Exodus 20:14','Civil & Criminal','Both','binding','Thou shalt not covet thy neighbour\'s house, thou shalt not covet thy neighbour\'s wife (Exodus 20:17) — the tenth commandment.'],
  [477,'Do not desire another\'s possession','Deuteronomy 5:18','Civil & Criminal','Both','binding','Includes another man\'s wife, house, field, or property.'],
  [478,'Return the robbed object or its value','Leviticus 5:23','Civil & Criminal','Both','binding','Restitution is required — return what was taken plus a fifth.'],
  [479,'Do not ignore a lost object','Deuteronomy 22:3','Civil & Criminal','Both','binding','If you find something lost, you are obligated to return it.'],
  [480,'Return the lost object to its owner','Deuteronomy 22:1','Civil & Criminal','Both','binding','This is the law of lost property — restore it.'],
  [481,'The court must implement laws against one who assaults another','Exodus 21:18','Civil & Criminal','Both','suspended','Requires a functioning Israelite court.'],
  [482,'Thou shalt not kill','Exodus 20:13','Civil & Criminal','Both','binding','Thou shalt not kill — the sixth commandment. The shedding of innocent blood is an abomination.'],
  [483,'Do not accept money to save a convicted manslayer','Numbers 35:31','Civil & Criminal','Both','suspended','Requires a functioning Israelite court.'],
  [484,'The court must send the accidental manslayer to a city of refuge','Numbers 35:25','Civil & Criminal','Both','suspended','Requires cities of refuge and a functioning Israelite court.'],
  [485,'Do not accept monetary restitution in place of sending an accidental manslayer to a city of refuge','Numbers 35:32','Civil & Criminal','Both','suspended','Requires the city of refuge system.'],
  [486,'Do not kill the manslayer before he stands trial','Numbers 35:12','Civil & Criminal','Both','suspended','Due process — requires a functioning Israelite court.'],
  [487,'Save someone being pursued even by taking the life of the pursuer','Deuteronomy 25:12','Civil & Criminal','Both','binding','You may and must stop someone in the act of the shedding of blood or assault.'],
  [488,'Do not pity the pursuer','Numbers 35:12','Civil & Criminal','Both','binding','No mercy for one pursuing to kill — stop them by any means necessary.'],
  [489,'Do not stand idly by if someone\'s life is in danger','Leviticus 19:16','Civil & Criminal','Both','binding','You are required to act when you can save a life.'],
  [490,'Designate refuge cities and prepare routes of access','Deuteronomy 19:3','Civil & Criminal','Both','suspended','Requires national Israelite governance.'],
  [491,'When a shedding of blood is unsolved and the murderer is not found, break the neck of a calf by the river valley (Eglah Arufah)','Deuteronomy 21:4','Civil & Criminal','Both','suspended','The Eglah Arufah ceremony — requires a functioning council of elders and judges of Israel.'],
  [492,'Do not work or plant that river valley after the Eglah Arufah','Deuteronomy 21:4','Civil & Criminal','Both','suspended','Requires the Eglah Arufah ceremony.'],
  [493,'Do not allow pitfalls or obstacles on your property','Deuteronomy 22:8','Civil & Criminal','Both','binding','You are responsible for hazards on your property.'],
  [494,'Make a guardrail around flat roofs','Deuteronomy 22:8','Civil & Criminal','Both','binding','Safety codes commanded by Torah — prevent death by negligence.'],
  [495,'Do not put a stumbling block before the blind','Leviticus 19:14','Civil & Criminal','Both','binding','Do not mislead anyone — physically or spiritually.'],
  [496,'Help another remove a load from a struggling beast','Exodus 23:5','Civil & Criminal','Both','binding','Care for animals — do not ignore an animal in distress.'],
  [497,'Help others load their beasts','Deuteronomy 22:4','Civil & Criminal','Both','binding','Assistance is commanded — do not pass by someone who needs help.'],
  [498,'Do not leave fallen beasts distraught with their burdens','Deuteronomy 22:4','Civil & Criminal','Both','binding','Actively help — do not walk past a struggling animal.'],
  [499,'Buy and sell according to Torah law','Leviticus 25:14','Civil & Criminal','Both','binding','All commerce must be governed by the law.'],
  [500,'Do not overcharge or underpay for an article','Leviticus 25:14','Civil & Criminal','Both','binding','Fraudulent pricing in either direction is forbidden.'],
  [501,'Do not insult or harm anybody with words','Leviticus 25:17','Civil & Criminal','Both','binding','Words carry weight — verbal oppression is forbidden.'],
  [502,'Do not cheat a sincere convert monetarily','Exodus 22:20','Civil & Criminal','Both','binding','Do not take financial advantage of those returning to the covenant.'],
  [503,'Do not insult or harm a sincere convert with words','Exodus 22:20','Civil & Criminal','Both','binding','Do not remind a convert of their past or speak against their journey.'],
  [504,'A Hebrew slave shall be released after six years','Exodus 21:2','Civil & Criminal','Men','binding','No Israelite can be held as a slave indefinitely.'],
  [505,'Do not sell an Israelite brother as a common slave','Leviticus 25:42','Civil & Criminal','Both','binding','He is the Most High\'s servant — treat him accordingly.'],
  [506,'Do not work an Israelite slave oppressively','Leviticus 25:43','Civil & Criminal','Both','binding','Treat the Israelite servant with dignity and respect.'],
  [507,'Do not allow a foreigner to work an Israelite slave oppressively','Leviticus 25:53','Civil & Criminal','Both','binding','Protect Israelites sold to non-Israelites from mistreatment.'],
  [508,'Do not have the kinsman-slave do menial slave labor','Leviticus 25:39','Civil & Criminal','Both','binding','An Israelite in your service must be treated as a hired worker, not a slave.'],
  [509,'Give the freed slave gifts when he goes free','Deuteronomy 15:14','Civil & Criminal','Both','binding','Send the freed servant away with provision — do not let him leave empty.'],
  [510,'Do not send the freed slave away empty-handed','Deuteronomy 15:13','Civil & Criminal','Both','binding','Provide generously for the freed servant.'],
  [511,'Redeem Jewish maidservants','Exodus 21:7-8','Civil & Criminal','Men','binding','If she please not her master, who hath betrothed her to himself, then shall he let her be redeemed: to sell her unto a strange nation he shall have no power (Exodus 21:8). A Hebrew maidservant must be redeemed — she cannot be abandoned or cast off.'],
  [512,'Betroth the Jewish maidservant','Exodus 21:8-9','Civil & Criminal','Men','binding','And if he have betrothed her unto his son, he shall deal with her after the manner of daughters (Exodus 21:9). If the master betrotheth her to his son, she must be treated with full honour as a daughter of the house.'],
  [513,'The master cannot resell a female servant','Exodus 21:7-11','Civil & Criminal','Men','binding','To sell her unto a strange nation he shall have no power, seeing he hath dealt deceitfully with her (Exodus 21:8). And if he do not these three unto her — food, raiment, and duty of marriage — then shall she go out free without money (Exodus 21:11). The master hath no power to sell her to another; if he neglect his duties toward her, she goeth out free.'],
  [514,'Canaanite slaves must work unless injured in a limb','Leviticus 25:46','Civil & Criminal','Both','suspended','Requires the broader Israelite slave law system.'],
  [515,'Do not extradite a slave who fled to Israel for refuge','Deuteronomy 23:16','Civil & Criminal','Both','binding','Protect the runaway slave — do not return him to his oppressor.'],
  [516,'Do not wrong a slave who has come to Israel for refuge','Deuteronomy 23:17','Civil & Criminal','Both','binding','The escaped slave seeking refuge must be protected and treated well.'],
  [517,'The courts must carry out the laws of a hired worker and guard','Exodus 22:9','Civil & Criminal','Both','suspended','Requires a functioning Israelite court.'],
  [518,'Pay wages on the day they were earned','Deuteronomy 24:15','Civil & Criminal','Both','binding','Do not withhold a poor man\'s wages overnight.'],
  [519,'Do not delay payment of wages past the agreed time','Leviticus 19:13','Civil & Criminal','Both','binding','The hire of him that is hired shall not abide with thee all night until the morning (Leviticus 19:13).'],
  [520,'The hired worker may eat from the unharvested crops where he works','Deuteronomy 23:25','Civil & Criminal','Both','binding','Workers have a right to eat from the produce they harvest.'],
  [521,'The worker must not eat while on hired time outside his work','Deuteronomy 23:26','Civil & Criminal','Both','binding','Eat while working the rows — not while performing other duties.'],
  [522,'The worker must not take more than he can eat','Deuteronomy 23:25','Civil & Criminal','Both','binding','Take only what you consume — do not fill a bag to take home.'],
  [523,'Do not muzzle an ox while it is plowing','Deuteronomy 25:4','Civil & Criminal','Both','binding','Workers and animals must benefit from their labor.'],
  [524,'The courts must carry out the laws of a borrower','Exodus 22:13','Civil & Criminal','Both','suspended','Requires a functioning Israelite court.'],
  [525,'The courts must carry out the laws of the unpaid guard','Exodus 22:6','Civil & Criminal','Both','suspended','Requires a functioning Israelite court.'],
  [526,'Lend without interest to fellow Israelites in need','Exodus 22:24','Civil & Criminal','Both','binding','Thou shalt not lend upon usury to thy brother; usury of money, usury of victuals, usury of any thing that is lent upon usury (Deuteronomy 23:19).'],
  [527,'Do not press the poor for repayment','Exodus 22:24','Civil & Criminal','Both','binding','Do not harass or pressure the poor man who owes you money.'],
  [528,'Press the idolater for payment','Deuteronomy 15:3','Civil & Criminal','Both','binding','Interest and debt collection from non-Israelites is permitted.'],
  [529,'The creditor must not forcibly take collateral','Deuteronomy 24:10','Civil & Criminal','Both','binding','Do not enter a man\'s home to take his pledge — let him bring it to you.'],
  [530,'Return the collateral to the debtor when it is needed','Deuteronomy 24:13','Civil & Criminal','Both','binding','Return a poor man\'s cloak by sundown so he can sleep in it.'],
  [531,'Do not delay returning the collateral when it is needed','Deuteronomy 24:12','Civil & Criminal','Both','binding','Do not keep the collateral overnight when the debtor needs it.'],
  [532,'Do not demand collateral from a widow','Deuteronomy 24:17','Civil & Criminal','Both','binding','Widows must not be burdened with collateral demands.'],
  [533,'Do not demand as collateral utensils needed for preparing food','Deuteronomy 24:6','Civil & Criminal','Both','binding','Do not take a man\'s millstone — you take his livelihood.'],
  [534,'Do not lend to a fellow Israelite with interest','Leviticus 25:37','Civil & Criminal','Both','binding','Thou shalt not give him thy money upon usury, nor lend him thy victuals for increase (Leviticus 25:37).'],
  [535,'Do not borrow from a fellow Israelite with interest','Deuteronomy 23:20','Civil & Criminal','Both','binding','Thou shalt not give nor receive usury among thy brethren.'],
  [536,'Do not play any role in an interest loan between Israelites','Exodus 22:24','Civil & Criminal','Both','binding','Neither be a witness to, nor facilitate, any usurious agreement between brethren.'],
  [537,'Lend to and borrow from non-Israelites at interest','Deuteronomy 23:21','Civil & Criminal','Both','binding','Unto a stranger thou mayest lend upon usury; but unto thy brother thou shalt not lend upon usury (Deuteronomy 23:20).'],
  [538,'The court must carry out the laws of the plaintiff, admitter, or denier','Exodus 22:8','Civil & Criminal','Both','suspended','Requires a functioning Israelite court.'],
  [539,'Carry out the laws of the order of inheritance','Numbers 27:8','Civil & Criminal','Both','binding','The order of inheritance — sons, daughters, brothers — follows Torah law.'],
  [540,'Appoint righteous judges','Deuteronomy 16:18','Courts & Judges','Both','suspended','Requires a functioning Israelite nation.'],
  [541,'Do not appoint judges unfamiliar with judicial procedure','Deuteronomy 1:17','Courts & Judges','Both','suspended','Requires a functioning Israelite court.'],
  [542,'Decide by majority in case of disagreement','Exodus 23:2','Courts & Judges','Both','suspended','Requires a functioning council of elders and judges of Israel or Israelite court.'],
  [543,'The court must not execute through a majority of one','Exodus 23:2','Courts & Judges','Both','suspended','Capital cases require a stronger majority — requires Israelite court.'],
  [544,'A judge who argues for acquittal must not argue for conviction in capital cases','Exodus 23:2','Courts & Judges','Both','suspended','Requires a functioning Israelite court.'],
  [545,'The court must carry out the death penalty of stoning','Deuteronomy 22:24','Courts & Judges','Both','suspended','Requires a functioning Israelite council of elders and judges of Israel.'],
  [546,'The court must carry out the death penalty of burning','Leviticus 20:14','Courts & Judges','Both','suspended','Requires a functioning Israelite council of elders and judges of Israel.'],
  [547,'The court must carry out the death penalty of the sword','Exodus 21:20','Courts & Judges','Both','suspended','Requires a functioning Israelite council of elders and judges of Israel.'],
  [548,'The court must carry out the death penalty of strangulation','Leviticus 20:10','Courts & Judges','Both','suspended','Requires a functioning Israelite council of elders and judges of Israel.'],
  [549,'The court must hang those stoned for blasphemy or idolatry','Deuteronomy 21:22','Courts & Judges','Both','suspended','Requires a functioning Israelite council of elders and judges of Israel.'],
  [550,'Bury the executed on the day they were killed','Deuteronomy 21:23','Courts & Judges','Both','binding','The dead must be buried without delay — applies today.'],
  [551,'Do not delay the burial overnight','Deuteronomy 21:23','Courts & Judges','Both','binding','Prompt burial is commanded — the body must not lie unburied overnight.'],
  [552,'The court must not let the witch live','Exodus 22:17','Courts & Judges','Both','suspended','Capital punishment requires a functioning Israelite council of elders and judges of Israel.'],
  [553,'The court must flog the wrongdoer','Deuteronomy 25:2','Courts & Judges','Both','suspended','Requires a functioning Israelite court.'],
  [554,'The court must not exceed the prescribed number of lashes','Deuteronomy 25:3','Courts & Judges','Both','suspended','Requires a functioning Israelite court.'],
  [555,'The court must not kill anybody on circumstantial evidence','Exodus 23:7','Courts & Judges','Both','suspended','Requires a functioning Israelite court.'],
  [556,'The court must not punish anybody who was forced to commit a crime','Deuteronomy 22:26','Courts & Judges','Both','suspended','Requires a functioning Israelite court.'],
  [557,'The judge must not pity the manslayer or assaulter at the trial','Deuteronomy 19:13','Courts & Judges','Both','suspended','Requires a functioning Israelite court.'],
  [558,'The judge must not have mercy on the poor man to pervert justice','Leviticus 19:15','Courts & Judges','Both','binding','Justice is blind — pity must not corrupt a verdict.'],
  [559,'The judge must not respect the great man to pervert justice','Leviticus 19:15','Courts & Judges','Both','binding','The powerful get no special treatment under Torah law.'],
  [560,'The judge must not decide unjustly against the habitual transgressor','Exodus 23:6','Courts & Judges','Both','binding','Even a habitual sinner deserves righteous judgment.'],
  [561,'The judge must not pervert justice','Leviticus 19:15','Courts & Judges','Both','binding','In any dispute or judgment — be fair and righteous always.'],
  [562,'The judge must not pervert a case involving a convert or an orphan','Deuteronomy 24:17','Courts & Judges','Both','binding','The vulnerable must receive special protection in judgment.'],
  [563,'Judge righteously','Leviticus 19:15','Courts & Judges','Both','binding','In any dispute — judge by the truth of Torah.'],
  [564,'The judge must not fear a violent man in judgment','Deuteronomy 1:17','Courts & Judges','Both','binding','Do not be intimidated — fear only the Most High.'],
  [565,'Do not accept bribes','Exodus 23:8','Courts & Judges','Both','binding','Thou shalt take no gift: for the gift blindeth the wise, and perverteth the words of the righteous (Exodus 23:8).'],
  [566,'Judges must not accept testimony unless both parties are present','Exodus 23:1','Courts & Judges','Both','binding','No ex parte communication — both sides must be heard.'],
  [567,'Do not curse judges','Exodus 22:27','Courts & Judges','Both','binding','Honor those in righteous authority — do not speak against them.'],
  [568,'Do not curse the head of state','Exodus 22:27','Courts & Judges','Both','binding','Do not curse the ruler of your people (Acts 23:5).'],
  [569,'Do not curse a deaf person','Leviticus 19:14','Courts & Judges','Both','binding','Do not curse anyone who cannot hear your words — it is still sin.'],
  [570,'Anyone who knows evidence must testify at a trial','Leviticus 5:1','Courts & Judges','Both','binding','Withholding evidence is sin — you are required to testify.'],
  [571,'Carefully interrogate the witness','Deuteronomy 13:15','Courts & Judges','Both','suspended','Requires a functioning Israelite court.'],
  [572,'A witness must not serve as a judge in capital crimes','Numbers 35:30','Courts & Judges','Both','suspended','Requires a functioning Israelite court.'],
  [573,'Do not accept testimony from a lone witness','Deuteronomy 19:15','Courts & Judges','Both','binding','Two or three witnesses are required to establish a matter (Matthew 18:16).'],
  [574,'Transgressors must not testify','Exodus 23:1','Courts & Judges','Both','suspended','Requires a functioning Israelite court.'],
  [575,'The litigant\'s relatives cannot testify','Deuteronomy 24:16','Courts & Judges','Both','suspended','Requires a functioning Israelite court.'],
  [576,'Do not testify falsely','Exodus 20:13','Courts & Judges','Both','binding','Thou shalt not bear false witness against thy neighbour (Exodus 20:16) — the ninth commandment.'],
  [577,'Do to the false witness what he tried to do to the defendant','Deuteronomy 19:19','Courts & Judges','Both','suspended','Requires a functioning Israelite court.'],
  [578,'Act according to the rulings of the high court','Deuteronomy 17:11','Courts & Judges','Both','suspended','Awaits restoration of the council of elders and judges of Israel and Israelite national governance.'],
  [579,'Do not deviate from a legal decision of the high court','Deuteronomy 17:11','Courts & Judges','Both','suspended','Awaits the council of elders and judges of Israel.'],
  [580,'Do not add to the Torah commandments','Deuteronomy 13:1','Courts & Judges','Both','binding','No man-made traditions may be added to the law of Moses.'],
  [581,'Do not diminish any commandments from the Torah','Deuteronomy 13:1','Courts & Judges','Both','binding','For verily I say unto you, Till heaven and earth pass, one jot or one tittle shall in no wise pass from the law, till all be fulfilled (Matthew 5:18).'],
  [582,'Do not curse your father and mother','Exodus 21:17','Family & Parents','Both','binding','And he that curseth his father, or his mother, shall surely be put to death (Exodus 21:17).'],
  [583,'Do not strike your father and mother','Exodus 21:15','Family & Parents','Both','binding','And he that smiteth his father, or his mother, shall be surely put to death (Exodus 21:15).'],
  [584,'Respect your father and mother','Exodus 20:12','Family & Parents','Both','binding','Honour thy father and thy mother: that thy days may be long upon the land which the LORD thy God giveth thee (Exodus 20:12) — the fifth commandment.'],
  [585,'Fear your father and mother','Leviticus 19:3','Family & Parents','Both','binding','Ye shall fear every man his mother, and his father, and keep my sabbaths: I am the LORD your God (Leviticus 19:3).'],
  [586,'Do not behave like the rebellious son described in the Torah','Deuteronomy 21:20','Family & Parents','Men','suspended','Capital punishment requires a functioning Israelite court.'],
  [587,'Mourn for relatives when they die','Leviticus 10:19','Family & Parents','Both','binding','Mourning is a righteous practice — honor the dead.'],
  [588,'The High Priest must not defile himself for any relatives','Leviticus 21:11','Priestly Laws','Priests','suspended','Requires a functioning High Priest.'],
  [589,'The High Priest must not enter under the same roof as a corpse','Leviticus 21:11','Priestly Laws','Priests','suspended','Requires a functioning High Priest.'],
  [590,'A priest must not defile himself for anyone other than his relatives','Leviticus 21:1','Priestly Laws','Priests','suspended','Requires functioning Levitical priesthood.'],
  [591,'Appoint a king from among the Israelites','Deuteronomy 17:15','Kingship','Both','suspended','The Israelite kingdom will be restored — but not yet.'],
  [592,'Do not appoint a convert as king','Deuteronomy 17:15','Kingship','Both','suspended','The king must be a native Israelite.'],
  [593,'The king must not have too many wives','Deuteronomy 17:17','Kingship','Men','suspended','Awaits restoration of Israelite kingship.'],
  [594,'The king must not have too many horses','Deuteronomy 17:16','Kingship','Men','suspended','No excessive military buildup — trust in the Most High.'],
  [595,'The king must not accumulate excessive silver and gold','Deuteronomy 17:17','Kingship','Men','suspended','No hoarding of wealth at the expense of the people.'],
  [596,'Destroy the seven Canaanite nations','Deuteronomy 20:17','Warfare & National','Men','suspended','Tied to national Israelite conquest — awaits restoration.'],
  [597,'Do not let any of the Canaanite nations remain alive','Deuteronomy 20:16','Warfare & National','Men','suspended','Requires national Israelite authority and military.'],
  [598,'Blot out the memory of Amalek','Deuteronomy 25:19','Warfare & National','Both','suspended','A national commandment — requires national Israelite authority.'],
  [599,'Remember what Amalek did to the Israelites','Deuteronomy 25:17','Warfare & National','Both','binding','Know your history and your enemies — remember the ambush in the wilderness.'],
  [600,'Do not forget Amalek\'s atrocities','Deuteronomy 25:19','Warfare & National','Both','binding','Keep the memory of your enemies alive — do not forget what was done.'],
  [601,'Do not dwell permanently in Egypt','Deuteronomy 17:16','Warfare & National','Both','identity','Spiritually: do not return to the systems and customs of your oppressors.'],
  [602,'Offer peace terms to a city before besieging it','Deuteronomy 20:10','Warfare & National','Men','suspended','Rules of Israelite warfare — requires national army.'],
  [603,'Do not offer peace to Ammon and Moab while besieging them','Deuteronomy 23:7','Warfare & National','Men','suspended','Requires national Israelite military.'],
  [604,'Do not destroy fruit trees during a siege','Deuteronomy 20:19','Warfare & National','Men','suspended','Rules of engagement — protect the food supply.'],
  [605,'Prepare latrines outside the camps','Deuteronomy 23:13','Warfare & National','Men','suspended','Sanitation laws for the military camp.'],
  [606,'Prepare a shovel for each soldier to dig with','Deuteronomy 23:14','Warfare & National','Men','suspended','Requires a functioning Israelite military.'],
  [607,'Appoint a priest to speak to soldiers during war','Deuteronomy 20:2','Warfare & National','Men','suspended','Spiritual leadership in battle — awaits national restoration.'],
  [608,'A newly married man is exempt from military service','Deuteronomy 24:5','Warfare & National','Men','suspended','Awaits a functioning Israelite military.'],
  [609,'Do not conscript the newly married man in any communal service','Deuteronomy 24:5','Warfare & National','Men','suspended','Family comes first — awaits Israelite national governance.'],
  [610,'Do not panic and retreat during battle','Deuteronomy 20:3','Warfare & National','Men','suspended','Courage is required — fear of the enemy is forbidden in battle.'],
  [611,'Carry out the laws of captive women','Deuteronomy 21:11','Warfare & National','Men','suspended','Requires a functioning Israelite military and governance.'],
  [612,'Do not sell a captive woman into slavery','Deuteronomy 21:14','Warfare & National','Men','suspended','Requires the Israelite laws of captive women to be in effect.'],
  [613,'Do not retain a captive woman for servitude after relations with her','Deuteronomy 21:14','Warfare & National','Men','suspended','Requires the Israelite laws of captive women.']];
const BUSINESS_IDS=new Set([201, 202, 211, 212, 214, 215, 216, 227, 228, 229, 230, 231, 232, 233, 254, 260, 261, 263, 265, 266, 267, 294, 295, 296, 429, 430, 440, 441, 442, 463, 464, 465, 466, 467, 468, 469, 470, 471, 472, 473, 474, 475, 476, 477, 478, 479, 480, 499, 500, 501, 502, 517, 518, 519, 520, 521, 522, 523, 524, 525, 526, 527, 528, 529, 530, 531, 532, 533, 534, 535, 536, 537, 538, 539, 565, 566]);
const FARMER_IDS=new Set([176, 177, 178, 179, 180, 181, 182, 183, 184, 185, 186, 187, 188, 189, 190, 191, 192, 193, 194, 200, 201, 202, 204, 205, 206, 207, 208, 234, 235, 236, 237, 238, 239, 240, 241, 242, 243, 244, 245, 246, 247, 248, 249, 250, 251, 252, 253, 254, 260, 261, 262, 263, 264, 265, 266, 267, 268, 269, 270, 271, 272, 273, 274, 275, 276, 277, 278, 279, 280, 281, 282, 283, 284, 285, 286, 287, 288, 289, 290, 291, 292, 293, 294, 295, 296, 402, 403, 426, 428, 429, 430, 463, 464, 465, 466, 472, 493, 494, 496, 497, 498, 523]);

const ALL_LAWS=ALL_LAWS_RAW.map(r=>({id:r[0],text:r[1],ref:r[2],category:r[3],who:r[4],status:r[5],note:r[6]}));

const STATUS_META={
  binding:  {label:"Fully Binding", bg:"#14532d",fg:"#86efac",dot:"#22c55e",desc:"In full effect — required observance today for all children of Israel"},
  suspended:{label:"Suspended",     bg:"#7c2d12",fg:"#fdba74",dot:"#f97316",desc:"Cannot be performed until the kingdom of Israel is restored — not abolished, will be fulfilled in the restoration"},
  identity: {label:"Identity Law",  bg:"#3b0764",fg:"#d8b4fe",dot:"#a855f7",desc:"Covenant boundary laws tied to the identity of the 12 Tribes and the national restoration of Israel"},
};
const WHO_BG={Men:"#1e3a5f",Women:"#4c0519",Both:"#1e293b",Priests:"#2e1065"};
const WHO_FG={Men:"#93c5fd",Women:"#fda4af",Both:"#cbd5e1",Priests:"#c4b5fd"};

// ── SCRIPTURE CACHE ───────────────────────────────────────────────────────────
const CACHE_KEY="heb_613_v3";
function getCache(){try{return JSON.parse(localStorage.getItem(CACHE_KEY)||"{}")}catch{return{}}}
function saveCache(d){try{localStorage.setItem(CACHE_KEY,JSON.stringify(d))}catch{}}
function updateCacheInfo(){
  const n=Object.keys(getCache()).length;
  document.getElementById("cache-info").textContent=n>0?`📦 ${n} verses cached offline`:"📖 Tap any scripture reference to load KJV verse · Cached after first load";
}

async function loadVerse(ref){
  const cache=getCache();
  if(cache[ref])return cache[ref];
  try{
    const r=await fetch("https://api.anthropic.com/v1/messages",{
      method:"POST",headers:{"Content-Type":"application/json"},
      body:JSON.stringify({model:"claude-sonnet-4-6",max_tokens:600,
        messages:[{role:"user",content:`Quote the exact King James Version (KJV 1611) text of ${ref}. Return ONLY the scripture text — no verse numbers inline, no commentary, no quotation marks, no preamble. If a range, quote all verses consecutively.`}]
      })
    });
    const d=await r.json();
    const t=d.content?.[0]?.text?.trim();
    if(t){const c={...getCache(),[ref]:t};saveCache(c);updateCacheInfo();return t;}
  }catch{}
  return null;
}

// ── MODAL ─────────────────────────────────────────────────────────────────────
function openModal(ref){
  document.getElementById("modal-ref").textContent="📖 "+ref;
  document.getElementById("modal-body").innerHTML=`<div class="modal-loading"><span class="spin" style="font-size:24px;display:block;margin-bottom:8px">⏳</span>Retrieving scripture…</div>`;
  document.getElementById("modal").style.display="flex";
  loadVerse(ref).then(v=>{
    const text=v||"Scripture not available. Please check your internet connection.";
    document.getElementById("modal-body").innerHTML=`
      <div class="modal-verse"><p>"${text}"</p></div>
      <p class="modal-cite">— ${ref} KJV 1611</p>
      <p class="modal-hint">Tap outside to close · Verses cached after first load</p>`;
  });
}
function closeModal(){document.getElementById("modal").style.display="none";}
document.getElementById("modal").addEventListener("click",function(e){if(e.target===this)closeModal();});

// ── HELPERS ───────────────────────────────────────────────────────────────────
function el(tag,cls,html){const e=document.createElement(tag);if(cls)e.className=cls;if(html!==undefined)e.innerHTML=html;return e;}
function statusBadge(status){const s=STATUS_META[status]||STATUS_META.binding;return `<span class="badge" style="background:${s.bg};color:${s.fg}">${s.label}</span>`;}
function whoBadge(who){return `<span class="badge" style="background:${WHO_BG[who]||"#1e293b"};color:${WHO_FG[who]||"#cbd5e1"}">${who}</span>`;}

function makeLawCard(law){
  const card=el("div","law-card");
  card.innerHTML=`
    <div class="law-card-top">
      <span class="law-id">#${law.id}</span>
      <div class="badges">${whoBadge(law.who)}${statusBadge(law.status)}</div>
    </div>
    <p class="law-text">${law.text}</p>
    <button class="law-ref" data-ref="${law.ref}">📖 ${law.ref}</button>
    <div class="law-note" style="display:none">${law.note}</div>
    <p class="law-toggle">▼ note</p>`;

  card.querySelector(".law-ref").addEventListener("click",e=>{e.stopPropagation();openModal(law.ref);});
  card.addEventListener("click",()=>{
    const note=card.querySelector(".law-note");
    const tog=card.querySelector(".law-toggle");
    const open=note.style.display==="block";
    note.style.display=open?"none":"block";
    tog.textContent=open?"▼ note":"▲ close note";
  });
  return card;
}

function sectionDivider(title,color,count){
  const d=el("div","section-div");
  d.innerHTML=`<span style="color:${color}">${title}</span><span class="s-count">(${count})</span><hr>`;
  return d;
}

// ── LAW LIST ──────────────────────────────────────────────────────────────────
function makeLawList(allLaws, defaultWho, hideWhoFilter){
  let who=defaultWho||"All", st="All", cat="All", q="", showAll=false;

  const wrap=el("div");

  // Search
  const searchInput=el("input","search-input");
  searchInput.placeholder="Search laws…";
  searchInput.addEventListener("input",e=>{q=e.target.value;render();});
  wrap.appendChild(searchInput);

  // Active chips bar
  const chipsBar=el("div","chips-bar");
  chipsBar.style.display="none";
  wrap.appendChild(chipsBar);

  // Who filter
  const whoGroup=el("div","filter-group");
  if(hideWhoFilter) whoGroup.style.display="none";
  whoGroup.innerHTML=`<span class="filter-label">Who</span><div class="filter-btns" id="who-btns"></div>`;
  wrap.appendChild(whoGroup);

  // Status filter
  const stGroup=el("div","filter-group");
  stGroup.innerHTML=`<span class="filter-label">Status</span><div class="filter-btns" id="st-btns"></div>`;
  wrap.appendChild(stGroup);

  // Category filter
  const catGroup=el("div","filter-group");
  catGroup.innerHTML=`<span class="filter-label">Category <span id="cat-count" style="color:#4b5563;text-transform:none"></span></span><div class="filter-cats" id="cat-btns"></div>`;
  wrap.appendChild(catGroup);

  // Toggle (Men/Women only)
  const toggleBtn=el("button","toggle-btn");
  toggleBtn.style.display="none";
  toggleBtn.addEventListener("click",()=>{showAll=!showAll;render();});
  wrap.appendChild(toggleBtn);

  // Count bar
  const countBar=el("div","count-bar");
  countBar.innerHTML=`<div style="display:flex;align-items:center"><span class="count-num" id="count-num">0</span><span class="count-text" id="count-text"></span></div><div class="progress-wrap" id="progress-wrap" style="display:none"><div class="progress-bar"><div class="progress-fill" id="progress-fill"></div></div><span class="progress-pct" id="progress-pct"></span></div>`;
  wrap.appendChild(countBar);

  // Results
  const results=el("div","results");
  wrap.appendChild(results);

  function makeFilterBtn(label,active,onClick){
    const b=el("button","filter-btn"+(active?" active":""),label);
    b.addEventListener("click",onClick);
    return b;
  }

  function getFiltered(){
    const isPersonal=who==="Men"||who==="Women";

    let specific=who==="All"?allLaws:who==="Both"?allLaws.filter(l=>l.who==="Both"):who==="Priests"?allLaws.filter(l=>l.who==="Priests"):allLaws.filter(l=>l.who===who);
    let shared=isPersonal&&showAll?allLaws.filter(l=>l.who==="Both"):[];

    const applyStatus=p=>st==="All"?p:p.filter(l=>l.status===st);
    const fSpec=applyStatus(specific);
    const fShare=applyStatus(shared);

    const combined=[...fSpec,...fShare];
    const cats=["All",...[...new Set(combined.map(l=>l.category))].sort()];
    const effCat=cats.includes(cat)?cat:"All";

    const applyCat=p=>effCat==="All"?p:p.filter(l=>l.category===effCat);
    const cSpec=applyCat(fSpec);
    const cShare=applyCat(fShare);

    const applyQ=p=>!q?p:p.filter(l=>l.text.toLowerCase().includes(q.toLowerCase())||l.ref.toLowerCase().includes(q.toLowerCase())||l.category.toLowerCase().includes(q.toLowerCase()));
    const finalSpec=applyQ(cSpec);
    const finalShare=applyQ(cShare);

    return{finalSpec,finalShare,cats,effCat,specific,shared:allLaws.filter(l=>l.who==="Both"),isPersonal};
  }

  function render(){
    const {finalSpec,finalShare,cats,effCat,specific,shared,isPersonal}=getFiltered();
    const shownTotal=finalSpec.length+finalShare.length;
    const grandTotal=isPersonal&&showAll?specific.length+shared.length:specific.length;
    const isFiltered=shownTotal<grandTotal;

    // Chips
    const chips=[];
    if(who!=="All")    chips.push({label:`Who: ${who}`,clear:()=>{who="All";showAll=false;render();}});
    if(st!=="All")     chips.push({label:`Status: ${STATUS_META[st]?.label||st}`,clear:()=>{st="All";render();}});
    if(effCat!=="All") chips.push({label:`Category: ${effCat}`,clear:()=>{cat="All";render();}});
    if(q)              chips.push({label:`Search: "${q}"`,clear:()=>{q="";searchInput.value="";render();}});

    if(chips.length>0){
      chipsBar.style.display="flex";
      chipsBar.innerHTML=`<span class="chip-label">Active:</span>`;
      chips.forEach(c=>{
        const chip=el("span","chip",c.label);
        const xBtn=el("button","","×");
        xBtn.addEventListener("click",c.clear);
        chip.appendChild(xBtn);
        chipsBar.appendChild(chip);
      });
      if(chips.length>1){
        const ca=el("button","clear-all","Clear all");
        ca.addEventListener("click",()=>{who=defaultWho||"All";st="All";cat="All";q="";searchInput.value="";showAll=false;render();});
        chipsBar.appendChild(ca);
      }
    } else {
      chipsBar.style.display="none";
    }

    // Who buttons
    if(!hideWhoFilter){
      const wb=wrap.querySelector("#who-btns");
      wb.innerHTML="";
      ["All","Men","Women","Both","Priests"].forEach(w=>{
        wb.appendChild(makeFilterBtn(w,who===w,()=>{who=w;showAll=false;render();}));
      });
    }

    // Status buttons
    const sb=wrap.querySelector("#st-btns");
    sb.innerHTML="";
    sb.appendChild(makeFilterBtn("All",st==="All",()=>{st="All";render();}));
    Object.entries(STATUS_META).forEach(([k,v])=>{
      sb.appendChild(makeFilterBtn(v.label,st===k,()=>{st=k;render();}));
    });

    // Category buttons
    const cb=wrap.querySelector("#cat-btns");
    cb.innerHTML="";
    wrap.querySelector("#cat-count").textContent=`(${cats.length-1} available)`;
    cats.forEach(c=>{
      cb.appendChild(makeFilterBtn(c,effCat===c,()=>{cat=c===effCat?"All":c;render();}));
    });

    // Toggle
    if(isPersonal){
      toggleBtn.style.display="flex";
      toggleBtn.className="toggle-btn"+(showAll?" on":"");
      toggleBtn.innerHTML=`<span>${showAll?`✓ Showing all laws that apply to ${who}`:`Show all laws that apply to ${who} (includes shared laws)`}</span><span class="toggle-hint">${showAll?`${specific.length} specific + ${shared.length} shared`:`+${shared.length} shared laws`}</span>`;
    } else {
      toggleBtn.style.display="none";
    }

    // Count bar
    countBar.className="count-bar"+(isFiltered?" filtered":"");
    wrap.querySelector("#count-num").textContent=shownTotal;
    const ct=wrap.querySelector("#count-text");
    ct.innerHTML=`of <span class="total">${grandTotal}</span> laws${isPersonal&&showAll&&!isFiltered?`<span class="shared">(${specific.length} specific + ${shared.length} shared)</span>`:""}${isFiltered?`<span class="out">· ${grandTotal-shownTotal} filtered out</span>`:""}`;
    const pw=wrap.querySelector("#progress-wrap");
    if(isFiltered){
      pw.style.display="flex";
      wrap.querySelector("#progress-fill").style.width=`${(shownTotal/grandTotal)*100}%`;
      wrap.querySelector("#progress-pct").textContent=Math.round((shownTotal/grandTotal)*100)+"%";
    } else pw.style.display="none";

    // Results
    results.innerHTML="";
    if(shownTotal===0){
      const e=el("div","empty");
      e.innerHTML=`<p>No laws match your filters.</p><button onclick="">Clear all filters</button>`;
      e.querySelector("button").addEventListener("click",()=>{who=defaultWho||"All";st="All";cat="All";q="";searchInput.value="";showAll=false;render();});
      results.appendChild(e);
    } else if(isPersonal&&showAll){
      results.appendChild(sectionDivider(`Laws specifically for ${who}`,who==="Men"?"#93c5fd":"#fda4af",finalSpec.length));
      if(finalSpec.length===0){const p=el("p","",`No ${who}-specific laws match your filters.`);p.style.cssText="color:#4b5563;font-size:12px;font-style:italic;padding:0 4px 12px";results.appendChild(p);}
      else finalSpec.forEach(l=>results.appendChild(makeLawCard(l)));
      results.appendChild(sectionDivider("Shared laws — also apply to you","#94a3b8",finalShare.length));
      if(finalShare.length===0){const p=el("p","","No shared laws match your filters.");p.style.cssText="color:#4b5563;font-size:12px;font-style:italic;padding:0 4px 12px";results.appendChild(p);}
      else finalShare.forEach(l=>results.appendChild(makeLawCard(l)));
    } else {
      finalSpec.forEach(l=>results.appendChild(makeLawCard(l)));
    }
  }

  render();
  return wrap;
}

// ── AGRICULTURE SPLIT ─────────────────────────────────────────────────────────
function makeAgriSplit(){
  const agriTabs=[
    {key:"men",    label:"♂ Men",     bg:"#1e3a5f",fg:"#93c5fd",abg:"#eab308",afg:"#000"},
    {key:"women",  label:"♀ Women",   bg:"#4c0519",fg:"#fda4af",abg:"#eab308",afg:"#000"},
    {key:"both",   label:"⚖️ Both",   bg:"#1e293b",fg:"#cbd5e1",abg:"#eab308",afg:"#000"},
    {key:"priests",label:"🕍 Priests", bg:"#2e1065",fg:"#c4b5fd",abg:"#eab308",afg:"#000"},
  ];
  const groups={
    men:    ALL_LAWS.filter(l=>l.category==="Agriculture"&&l.who==="Men"),
    women:  ALL_LAWS.filter(l=>l.category==="Agriculture"&&l.who==="Women"),
    both:   ALL_LAWS.filter(l=>l.category==="Agriculture"&&l.who==="Both"),
    priests:ALL_LAWS.filter(l=>l.category==="Agriculture"&&l.who==="Priests"),
  };
  let current="both";
  const wrap=el("div","panel");
  wrap.style.border="1px solid #3f6212";
  wrap.innerHTML=`<h2>🌾 Agricultural Laws</h2><p class="panel-sub">Laws governing planting, harvest, tithes, the seventh year, Jubilee, and land — split by who they apply to</p><div class="agri-tabs" id="agri-tabs"></div><div id="agri-results"></div>`;

  function renderAgri(){
    const tabsEl=wrap.querySelector("#agri-tabs");
    tabsEl.innerHTML="";
    agriTabs.forEach(t=>{
      const b=el("button","agri-tab",`${t.label} <span style="opacity:.6">(${groups[t.key].length})</span>`);
      b.style.cssText=`background:${current===t.key?"#eab308":t.bg};color:${current===t.key?"#000":t.fg};border:1px solid ${current===t.key?"#eab308":t.bg}`;
      b.addEventListener("click",()=>{current=t.key;renderAgri();});
      tabsEl.appendChild(b);
    });
    const res=wrap.querySelector("#agri-results");
    res.innerHTML="";
    const laws=groups[current];
    if(!laws.length){res.innerHTML=`<p style="color:#6b7280;font-style:italic;text-align:center;padding:24px">No Agricultural laws specifically for this group.</p>`;}
    else{const d=el("div","results");laws.forEach(l=>d.appendChild(makeLawCard(l)));res.appendChild(d);}
  }
  renderAgri();
  return wrap;
}

// ── OVERVIEW ──────────────────────────────────────────────────────────────────
function makeOverview(setTab){
  const binding  =ALL_LAWS.filter(l=>l.status==="binding").length;
  const suspended=ALL_LAWS.filter(l=>l.status==="suspended").length;
  const identity =ALL_LAWS.filter(l=>l.status==="identity").length;
  const men      =ALL_LAWS.filter(l=>l.who==="Men").length;
  const women    =ALL_LAWS.filter(l=>l.who==="Women").length;
  const both     =ALL_LAWS.filter(l=>l.who==="Both").length;
  const priests  =ALL_LAWS.filter(l=>l.who==="Priests").length;
  const business =ALL_LAWS.filter(l=>BUSINESS_IDS.has(l.id)).length;
  const farmer   =ALL_LAWS.filter(l=>FARMER_IDS.has(l.id)).length;

  const wrap=el("div");

  // Framework
  const fw=el("div","overview-framework");
  fw.innerHTML=`<h2>For the Children of Israel</h2>`;
  const points=[
    ['These 613 laws were given by the Most High unto Moses for the','children of Israel','— the scattered seed of the 12 Tribes (Exodus 19:3-6)'],
    ['The curses of','Deuteronomy 28','identify the true children of Israel as those taken into captivity by ships and sold into slavery among the nations'],
    ['Yeshua the Messiah came to','fulfil — not destroy','the law — Think not that I am come to destroy the law, or the prophets (Matthew 5:17)'],
    ['','No law was abolished','— the handwriting of ordinances in Colossians 2:14 speaketh of the debt record against us, not the laws of Moses'],
    ['','Suspended laws','cannot be performed until the kingdom of Israel is restored — they are not abolished, they shall be fulfilled in the restoration'],
    ['This is not the tradition of modern-day Jews nor Rabbinic Judaism — this is','the law given to the Hebrew Israelites','at Mount Sinai'],
    ['All scripture is from the','King James Version 1611',''],
  ];
  points.forEach(([pre,bold,post])=>{
    const r=el("div","fw-row");
    r.innerHTML=`<span class="fw-bullet">✦</span><p class="fw-text">${pre} <strong>${bold}</strong> ${post}</p>`;
    fw.appendChild(r);
  });
  wrap.appendChild(fw);

  // Status key
  const sk=el("div","status-key");
  sk.innerHTML=`<h2>Law Status Key</h2>`;
  Object.entries(STATUS_META).forEach(([k,v])=>{
    const r=el("div","sk-row");
    r.innerHTML=`<span class="sk-dot" style="background:${v.dot}"></span><p class="sk-text"><strong>${v.label}: </strong>${v.desc}</p>`;
    sk.appendChild(r);
  });
  wrap.appendChild(sk);

  // Cards
  const cards=el("div","overview-cards");
  const cardData=[
    {key:"binding",  label:"✅ Fully Binding",  count:binding,   color:"#4ade80",border:"#166534"},
    {key:"suspended",label:"⏸️ Suspended",      count:suspended, color:"#fb923c",border:"#9a3412"},
    {key:"identity", label:"🛡️ Identity Laws",  count:identity,  color:"#c084fc",border:"#6b21a8"},
    {key:"men",      label:"♂ Men",             countA:men, countB:both, color:"#93c5fd",border:"#1e40af"},
    {key:"women",    label:"♀ Women",           countA:women, countB:both, color:"#fda4af",border:"#9f1239"},
    {key:"both",     label:"⚖️ Both",           count:both,      color:"#e2e8f0",border:"#374151"},
    {key:"priests",  label:"🕍 Priests",        count:priests,   color:"#c4b5fd",border:"#4c1d95"},
    {key:"business", label:"💼 Business",       count:business,  color:"#fde68a",border:"#713f12"},
    {key:"farmer",   label:"🌾 Farmer",         count:farmer,    color:"#bef264",border:"#365314"},
    {key:"all",      label:"🔍 All 613",         count:ALL_LAWS.length, color:"#fbbf24",border:"#92400e"},
  ];
  cardData.forEach(c=>{
    const btn=el("button","ov-card");
    btn.style.cssText=`color:${c.color};border-color:${c.border}`;
    const countHTML=c.count!=null
      ?`${c.count}<span class="ov-arrow"> laws →</span>`
      :`${c.countA}<span style="opacity:.5;font-size:14px">+${c.countB}</span><span class="ov-arrow"> laws →</span>`;
    btn.innerHTML=`<div class="ov-label" style="color:${c.color}">${c.label}</div><div class="ov-count" style="color:${c.color}">${countHTML}</div>`;
    btn.addEventListener("click",()=>setTab(c.key));
    cards.appendChild(btn);
  });
  wrap.appendChild(cards);
  return wrap;
}

// ── APP ───────────────────────────────────────────────────────────────────────
let currentTab="overview";

const binding  =ALL_LAWS.filter(l=>l.status==="binding");
const suspended=ALL_LAWS.filter(l=>l.status==="suspended");
const identity =ALL_LAWS.filter(l=>l.status==="identity");
const men      =ALL_LAWS.filter(l=>l.who==="Men");
const women    =ALL_LAWS.filter(l=>l.who==="Women");
const both     =ALL_LAWS.filter(l=>l.who==="Both");
const priests  =ALL_LAWS.filter(l=>l.who==="Priests");
const business =ALL_LAWS.filter(l=>BUSINESS_IDS.has(l.id));
const farmer   =ALL_LAWS.filter(l=>FARMER_IDS.has(l.id));

// Stat cards
const statData=[
  {label:"Total",     count:ALL_LAWS.length,border:"#92400e",bg:"#1c0a00",color:"#fbbf24"},
  {label:"Binding",   count:binding.length, border:"#166534",bg:"#052e16",color:"#4ade80"},
  {label:"Suspended", count:suspended.length,border:"#9a3412",bg:"#1c0a00",color:"#fb923c"},
  {label:"Identity",  count:identity.length,border:"#6b21a8",bg:"#1a0a2e",color:"#c084fc"},
];
const sg=document.getElementById("stat-grid");
statData.forEach(s=>{
  const c=el("div","stat-card");
  c.style.cssText=`border:1px solid ${s.border};background:${s.bg}`;
  c.innerHTML=`<div class="num" style="color:${s.color}">${s.count}</div><div class="lbl" style="color:${s.color}">${s.label}</div>`;
  sg.appendChild(c);
});

// Tab definitions
const tabs=[
  {key:"overview", label:"Overview",  icon:"📜"},
  {key:"all",      label:"All 613",   icon:"🔍", count:ALL_LAWS.length},
  {key:"binding",  label:"Binding",   icon:"✅", count:binding.length},
  {key:"suspended",label:"Suspended", icon:"⏸️", count:suspended.length},
  {key:"identity", label:"Identity",  icon:"🛡️", count:identity.length},
  {key:"men",      label:"Men",       icon:"♂",  countA:men.length, countB:both.length},
  {key:"women",    label:"Women",     icon:"♀",  countA:women.length, countB:both.length},
  {key:"both",     label:"Both",      icon:"⚖️", count:both.length},
  {key:"priests",  label:"Priests",   icon:"🕍", count:priests.length},
  {key:"business", label:"Business",  icon:"💼", count:business.length},
  {key:"farmer",   label:"Farmer",    icon:"🌾", count:farmer.length},
];

function makePanel(title,sub,border,lawList,defaultWho,hideWho){
  const p=el("div","panel");
  p.style.border=`2px solid ${border}`;
  p.innerHTML=`<h2>${title}</h2>${sub?`<p class="panel-sub">${sub}</p>`:""}`;
  p.appendChild(makeLawList(lawList,defaultWho,hideWho));
  return p;
}

function setTab(key){
  currentTab=key;
  // Update nav buttons
  document.querySelectorAll(".nav button").forEach(b=>{
    b.classList.toggle("active",b.dataset.key===key);
  });
  // Render content
  const main=document.getElementById("main-content");
  main.innerHTML="";
  let content;
  switch(key){
    case"overview":  content=makeOverview(setTab); break;
    case"all":       content=makePanel("🔍 All 613 Laws","Complete list — use filters to narrow down","#92400e",ALL_LAWS); break;
    case"binding":   content=makePanel("✅ Fully Binding Laws","In full effect — required observance today for all children of Israel","#166534",binding); break;
    case"suspended": content=makePanel("⏸️ Suspended Laws","Cannot be performed until the kingdom of Israel is restored — not abolished","#9a3412",suspended); break;
    case"identity":  content=makePanel("🛡️ Identity & Covenant Laws","Covenant boundary laws tied to the identity of the 12 Tribes","#6b21a8",identity); break;
    case"men":       content=makePanel("♂ Laws for Men","Start with laws specific to you — tap the toggle to also see shared laws that apply to you","#1e40af",ALL_LAWS,"Men",true); break;
    case"women":     content=makePanel("♀ Laws for Women","Start with laws specific to you — tap the toggle to also see shared laws that apply to you","#9f1239",ALL_LAWS,"Women",true); break;
    case"both":      content=makePanel("⚖️ Laws for Both","Commandments binding on all Israelites regardless of gender","#374151",both); break;
    case"priests":   content=makePanel("🕍 Laws for the Priesthood","Commandments specific to the sons of Levi and the sons of Aaron","#4c1d95",priests); break;
    case"business":  content=makePanel("💼 Laws for Businessmen","Laws governing commerce, trade, wages, lending, weights, contracts, and property","#713f12",business); break;
    case"farmer":    content=makeAgriSplit(); break;
    default:         content=makeOverview(setTab);
  }
  main.appendChild(content);
}

// Build nav
const nav=document.getElementById("nav");
tabs.forEach(t=>{
  const b=el("button","","");
  b.dataset.key=t.key;
  const countStr=t.count!=null?` (${t.count})`:t.countA!=null?` (${t.countA}<span style="opacity:.5">+${t.countB}</span>)`:"";
  b.innerHTML=`${t.icon} ${t.label}${countStr}`;
  if(t.key==="overview") b.classList.add("active");
  b.addEventListener("click",()=>setTab(t.key));
  nav.appendChild(b);
});

// Init
updateCacheInfo();
setTab("overview");
</script>
</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
<title>Evan's Job Hub</title>
<style>
  :root{
    --navy:#1F3864;
    --navy-light:#2f4f8f;
    --navy-dark:#152748;
    --white:#ffffff;
    --bg:#eef1f6;
    --gray:#6b7280;
    --light-gray:#e5e7eb;
    --green:#16a34a;
    --red:#dc2626;
    --amber:#d97706;
    --shadow:0 6px 24px rgba(31,56,100,.15);
  }
  *{box-sizing:border-box;margin:0;padding:0;-webkit-tap-highlight-color:transparent;}
  html,body{height:100%;}
  body{
    font-family:-apple-system,BlinkMacSystemFont,"Segoe UI",Roboto,Helvetica,Arial,sans-serif;
    background:var(--bg);
    color:#1f2937;
    overflow:hidden;
  }
  /* ---------- Header ---------- */
  header{
    background:var(--navy);
    color:#fff;
    padding:14px 18px;
    display:flex;align-items:center;justify-content:space-between;
    box-shadow:0 2px 8px rgba(0,0,0,.12);
    position:relative;z-index:20;
  }
  header h1{font-size:18px;font-weight:700;letter-spacing:.3px;}
  header .sub{font-size:11px;opacity:.8;font-weight:400;}
  /* ---------- Main scroll area ---------- */
  main{
    position:absolute;
    top:56px;bottom:64px;left:0;right:0;
    overflow-y:auto;
    -webkit-overflow-scrolling:touch;
  }
  .view{display:none;padding:16px;min-height:100%;}
  .view.active{display:block;}
  #view-discover.active{display:flex;flex-direction:column;}
  /* ---------- Bottom nav ---------- */
  nav{
    position:absolute;bottom:0;left:0;right:0;height:64px;
    background:#fff;border-top:1px solid var(--light-gray);
    display:flex;z-index:20;
    box-shadow:0 -2px 10px rgba(31,56,100,.06);
  }
  nav button{
    flex:1;background:none;border:none;cursor:pointer;
    display:flex;flex-direction:column;align-items:center;justify-content:center;gap:3px;
    color:var(--gray);font-size:11px;font-weight:600;padding:6px 0;
    transition:color .15s;
  }
  nav button svg{width:24px;height:24px;stroke:currentColor;fill:none;stroke-width:2;}
  nav button.active{color:var(--navy);}
  nav button.active svg{fill:rgba(31,56,100,.08);}
  /* ---------- Buttons ---------- */
  .btn{
    background:var(--navy);color:#fff;border:none;border-radius:10px;
    padding:12px 18px;font-size:15px;font-weight:600;cursor:pointer;
    transition:background .15s,transform .05s;width:100%;
  }
  .btn:hover{background:var(--navy-light);}
  .btn:active{transform:scale(.98);}
  .btn:disabled{opacity:.55;cursor:not-allowed;}
  .btn.secondary{background:#fff;color:var(--navy);border:2px solid var(--navy);}
  .btn.secondary:hover{background:#f3f6fc;}
  .btn.danger{background:var(--red);}
  .btn.small{padding:8px 12px;font-size:13px;width:auto;}
  /* ---------- Discover ---------- */
  .deck-wrap{
    flex:1;display:flex;flex-direction:column;align-items:center;justify-content:center;
    width:100%;max-width:460px;margin:0 auto;
  }
  .card-stack{position:relative;width:100%;height:440px;margin-bottom:8px;}
  .job-card{
    position:absolute;top:0;left:0;right:0;
    background:#fff;border-radius:18px;box-shadow:var(--shadow);
    padding:22px;height:100%;display:flex;flex-direction:column;
    cursor:grab;touch-action:pan-y;
    border-top:6px solid var(--navy);
    overflow:hidden;
  }
  .job-card .badge-type{
    align-self:flex-start;background:rgba(31,56,100,.1);color:var(--navy);
    font-size:11px;font-weight:700;padding:4px 10px;border-radius:20px;
    text-transform:uppercase;letter-spacing:.5px;margin-bottom:10px;
  }
  .job-card h2{font-size:21px;color:var(--navy);line-height:1.2;margin-bottom:4px;}
  .job-card .company{font-size:15px;font-weight:600;color:#374151;margin-bottom:10px;}
  .job-card .meta{display:flex;flex-wrap:wrap;gap:8px;margin-bottom:14px;}
  .job-card .meta span{
    background:#f3f6fc;color:#374151;font-size:12px;font-weight:600;
    padding:5px 10px;border-radius:8px;display:inline-flex;align-items:center;gap:4px;
  }
  .job-card .pay{color:var(--green);}
  .job-card .summary{
    font-size:14px;line-height:1.55;color:#4b5563;overflow-y:auto;flex:1;
  }
  .job-card .summary ul{margin:8px 0 0 18px;}
  .job-card .summary li{margin-bottom:4px;}
  .stamp{
    position:absolute;top:24px;font-size:30px;font-weight:900;
    padding:6px 16px;border:5px solid;border-radius:12px;opacity:0;
    transition:opacity .1s;pointer-events:none;text-transform:uppercase;
  }
  .stamp.like{right:20px;color:var(--green);border-color:var(--green);transform:rotate(14deg);}
  .stamp.nope{left:20px;color:var(--red);border-color:var(--red);transform:rotate(-14deg);}
  .swipe-actions{display:flex;gap:24px;justify-content:center;align-items:center;margin-top:6px;}
  .circle-btn{
    width:66px;height:66px;border-radius:50%;border:none;cursor:pointer;
    display:flex;align-items:center;justify-content:center;
    box-shadow:0 4px 14px rgba(0,0,0,.15);transition:transform .1s;background:#fff;
  }
  .circle-btn:active{transform:scale(.9);}
  .circle-btn svg{width:32px;height:32px;stroke-width:3;fill:none;}
  .circle-btn.skip svg{stroke:var(--red);}
  .circle-btn.like svg{stroke:var(--green);}
  .deck-empty{text-align:center;color:var(--gray);padding:40px 20px;}
  .deck-empty h3{color:var(--navy);margin-bottom:8px;}
  .counter{font-size:12px;color:var(--gray);margin-top:10px;font-weight:600;}
  /* ---------- Toast ---------- */
  #toast{
    position:fixed;left:50%;bottom:84px;transform:translateX(-50%) translateY(20px);
    background:var(--navy-dark);color:#fff;padding:12px 18px;border-radius:12px;
    font-size:13px;max-width:90%;line-height:1.4;box-shadow:0 6px 20px rgba(0,0,0,.3);
    opacity:0;pointer-events:none;transition:opacity .3s,transform .3s;z-index:60;text-align:center;
  }
  #toast.show{opacity:1;transform:translateX(-50%) translateY(0);}
  /* ---------- Applied table ---------- */
  .stats{display:flex;gap:10px;margin-bottom:16px;}
  .stat-card{
    flex:1;background:var(--navy);color:#fff;border-radius:14px;padding:14px 10px;text-align:center;
  }
  .stat-card .num{font-size:26px;font-weight:800;line-height:1;}
  .stat-card .label{font-size:11px;opacity:.85;margin-top:5px;font-weight:600;}
  .table-card{background:#fff;border-radius:14px;box-shadow:var(--shadow);overflow:hidden;}
  .table-scroll{overflow-x:auto;}
  table{width:100%;border-collapse:collapse;font-size:13px;min-width:680px;}
  th{background:var(--navy);color:#fff;padding:10px 8px;text-align:left;font-weight:600;font-size:12px;white-space:nowrap;}
  td{padding:9px 8px;border-bottom:1px solid var(--light-gray);vertical-align:middle;}
  tr:last-child td{border-bottom:none;}
  td .co{font-weight:700;color:var(--navy);}
  select,input,textarea{font-family:inherit;}
  td select,td input{
    border:1px solid var(--light-gray);border-radius:7px;padding:6px;font-size:12px;width:100%;background:#fff;
  }
  td select:focus,td input:focus{outline:2px solid var(--navy-light);border-color:var(--navy);}
  .del-btn{
    background:none;border:none;cursor:pointer;color:var(--red);padding:4px;border-radius:6px;
  }
  .del-btn:hover{background:rgba(220,38,38,.1);}
  .del-btn svg{width:18px;height:18px;stroke:currentColor;fill:none;stroke-width:2;}
  .empty-state{text-align:center;color:var(--gray);padding:40px 20px;}
  /* ---------- Forms / Settings / Cover ---------- */
  .panel{background:#fff;border-radius:14px;box-shadow:var(--shadow);padding:18px;margin-bottom:16px;}
  .panel h3{color:var(--navy);font-size:16px;margin-bottom:14px;display:flex;align-items:center;gap:8px;}
  .field{margin-bottom:14px;}
  .field label{display:block;font-size:13px;font-weight:600;color:#374151;margin-bottom:5px;}
  .field input[type=text],.field input[type=email],.field input[type=password],.field input[type=tel],.field select,.field textarea{
    width:100%;border:1.5px solid var(--light-gray);border-radius:9px;padding:11px;font-size:14px;background:#fff;
  }
  .field input:focus,.field textarea:focus,.field select:focus{outline:none;border-color:var(--navy);box-shadow:0 0 0 3px rgba(31,56,100,.12);}
  .field textarea{resize:vertical;min-height:120px;}
  .checks{display:flex;flex-wrap:wrap;gap:8px;}
  .check{
    display:flex;align-items:center;gap:6px;background:#f3f6fc;padding:8px 11px;border-radius:9px;
    font-size:13px;cursor:pointer;font-weight:500;border:1.5px solid transparent;
  }
  .check input{width:16px;height:16px;accent-color:var(--navy);}
  .check.checked{border-color:var(--navy);background:#e7eefb;}
  .row-btns{display:flex;gap:10px;margin-top:6px;}
  .letter-out{
    background:#f9fafb;border:1.5px solid var(--light-gray);border-radius:10px;padding:16px;
    font-size:14px;line-height:1.65;white-space:pre-wrap;margin-top:12px;color:#1f2937;
  }
  .hist-item{
    display:flex;justify-content:space-between;align-items:center;
    padding:11px;border:1px solid var(--light-gray);border-radius:10px;margin-bottom:8px;cursor:pointer;
  }
  .hist-item:hover{background:#f3f6fc;}
  .hist-item .h-co{font-weight:700;color:var(--navy);font-size:14px;}
  .hist-item .h-date{font-size:11px;color:var(--gray);}
  /* ---------- Modal ---------- */
  .modal-bg{
    position:fixed;inset:0;background:rgba(15,23,42,.55);z-index:80;
    display:none;align-items:center;justify-content:center;padding:20px;
  }
  .modal-bg.show{display:flex;}
  .modal{
    background:#fff;border-radius:16px;max-width:420px;width:100%;max-height:80vh;overflow-y:auto;
    box-shadow:0 20px 60px rgba(0,0,0,.3);
  }
  .modal-head{background:var(--navy);color:#fff;padding:16px 18px;font-weight:700;font-size:16px;border-radius:16px 16px 0 0;display:flex;justify-content:space-between;align-items:center;}
  .modal-head .x{cursor:pointer;font-size:22px;line-height:1;}
  .modal-body{padding:18px;font-size:14px;line-height:1.6;color:#374151;}
  .reason-opt{
    display:block;width:100%;text-align:left;background:#f3f6fc;border:1.5px solid transparent;
    border-radius:10px;padding:13px 14px;margin-bottom:9px;cursor:pointer;font-size:14px;font-weight:600;color:#374151;
  }
  .reason-opt:hover{border-color:var(--navy);background:#e7eefb;}
  .spinner{
    width:34px;height:34px;border:4px solid rgba(31,56,100,.2);border-top-color:var(--navy);
    border-radius:50%;animation:spin .8s linear infinite;margin:14px auto;
  }
  @keyframes spin{to{transform:rotate(360deg);}}
  .loading-box{text-align:center;color:var(--gray);padding:30px 10px;font-size:14px;}
  .hint{font-size:11px;color:var(--gray);margin-top:4px;line-height:1.4;}
  .pill-note{background:#fff7ed;border:1px solid #fed7aa;color:#9a3412;font-size:12px;padding:10px 12px;border-radius:10px;margin-bottom:14px;line-height:1.5;}
</style>
</head>
<body>

<header>
  <div>
    <h1>Evan's Job Hub</h1>
    <div class="sub">Find · Track · Apply — Calgary, AB</div>
  </div>
  <div class="sub" id="hdr-count"></div>
</header>

<main>
  <!-- ============ DISCOVER ============ -->
  <section class="view active" id="view-discover">
    <div class="deck-wrap">
      <div class="card-stack" id="cardStack">
        <div class="loading-box" id="deckLoading">
          <div class="spinner"></div>
          Loading fresh job matches…
        </div>
      </div>
      <div class="swipe-actions" id="swipeActions" style="display:none;">
        <button class="circle-btn skip" id="btnSkip" aria-label="Skip">
          <svg viewBox="0 0 24 24"><line x1="18" y1="6" x2="6" y2="18"/><line x1="6" y1="6" x2="18" y2="18"/></svg>
        </button>
        <button class="circle-btn like" id="btnLike" aria-label="Save and apply">
          <svg viewBox="0 0 24 24"><polyline points="20 6 9 17 4 12"/></svg>
        </button>
      </div>
      <div class="counter" id="deckCounter"></div>
    </div>
  </section>

  <!-- ============ APPLIED ============ -->
  <section class="view" id="view-applied">
    <div class="stats">
      <div class="stat-card"><div class="num" id="statSaved">0</div><div class="label">Saved</div></div>
      <div class="stat-card"><div class="num" id="statApplied">0</div><div class="label">Applied</div></div>
      <div class="stat-card"><div class="num" id="statInterview">0</div><div class="label">Interviews</div></div>
    </div>
    <div class="table-card">
      <div class="table-scroll">
        <table id="appTable">
          <thead>
            <tr>
              <th>Company</th><th>Role</th><th>Pay</th><th>Date Saved</th>
              <th>How Applied</th><th>Status</th><th>Notes</th><th></th>
            </tr>
          </thead>
          <tbody id="appBody"></tbody>
        </table>
      </div>
      <div class="empty-state" id="appEmpty">No saved jobs yet. Swipe right on the Discover tab to add jobs here.</div>
    </div>
  </section>

  <!-- ============ COVER LETTER ============ -->
  <section class="view" id="view-cover">
    <div class="panel">
      <h3>Cover Letter Generator</h3>
      <div class="field">
        <label for="clCompany">Company Name</label>
        <input type="text" id="clCompany" placeholder="e.g. Calgary Co-op">
      </div>
      <div class="field">
        <label for="clTitle">Job Title</label>
        <input type="text" id="clTitle" placeholder="e.g. Retail Cashier">
      </div>
      <div class="field">
        <label for="clDesc">Paste the job posting (optional but helps)</label>
        <textarea id="clDesc" placeholder="Paste the job description here…"></textarea>
      </div>
      <button class="btn" id="clGenerate">Generate Cover Letter</button>
      <div id="clResultWrap"></div>
    </div>
    <div class="panel">
      <h3>Recent Letters</h3>
      <div id="clHistory"><div class="empty-state">No letters yet.</div></div>
    </div>
  </section>

  <!-- ============ SETTINGS ============ -->
  <section class="view" id="view-settings">
    <div class="panel">
      <h3>API Connection</h3>
      <div class="field">
        <label for="setApiKey">Anthropic API Key</label>
        <input type="password" id="setApiKey" placeholder="sk-ant-...">
        <div class="hint">Stored only in your browser (localStorage). Required to generate jobs and cover letters.</div>
      </div>
    </div>
    <div class="panel">
      <h3>Your Details</h3>
      <div class="field"><label for="setName">Name</label><input type="text" id="setName"></div>
      <div class="field"><label for="setEmail">Email</label><input type="email" id="setEmail"></div>
      <div class="field"><label for="setPhone">Phone</label><input type="tel" id="setPhone"></div>
      <div class="field"><label for="setPostal">Neighbourhood / Postal Code</label><input type="text" id="setPostal" placeholder="e.g. T2P 1J9 / Downtown"></div>
      <div class="field">
        <label for="setCommute">Max Commute Preference</label>
        <select id="setCommute">
          <option>Walking distance only</option>
          <option>Up to 15 min by bus/bike</option>
          <option>Up to 30 min by bus/bike</option>
          <option>Anywhere in Calgary</option>
        </select>
      </div>
    </div>
    <div class="panel">
      <h3>Preferred Job Types</h3>
      <div class="checks" id="jobTypeChecks"></div>
    </div>
    <div class="panel">
      <h3>Availability</h3>
      <div class="checks" id="availChecks"></div>
    </div>
    <div class="panel">
      <h3>AI Preference Profile</h3>
      <div class="pill-note">The app learns what you like as you swipe and uses it to pick better jobs.</div>
      <div class="row-btns">
        <button class="btn secondary" id="btnViewProfile">View Profile</button>
        <button class="btn danger" id="btnResetProfile">Reset Preferences</button>
      </div>
    </div>
  </section>
</main>

<nav>
  <button data-view="discover" class="active">
    <svg viewBox="0 0 24 24"><path d="M12 2L2 7l10 5 10-5-10-5z"/><path d="M2 17l10 5 10-5"/><path d="M2 12l10 5 10-5"/></svg>
    Discover
  </button>
  <button data-view="applied">
    <svg viewBox="0 0 24 24"><path d="M9 11l3 3L22 4"/><path d="M21 12v7a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V5a2 2 0 0 1 2-2h11"/></svg>
    Applied
  </button>
  <button data-view="cover">
    <svg viewBox="0 0 24 24"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"/><polyline points="14 2 14 8 20 8"/><line x1="16" y1="13" x2="8" y2="13"/><line x1="16" y1="17" x2="8" y2="17"/></svg>
    Cover Letter
  </button>
  <button data-view="settings">
    <svg viewBox="0 0 24 24"><circle cx="12" cy="12" r="3"/><path d="M19.4 15a1.65 1.65 0 0 0 .33 1.82l.06.06a2 2 0 1 1-2.83 2.83l-.06-.06a1.65 1.65 0 0 0-1.82-.33 1.65 1.65 0 0 0-1 1.51V21a2 2 0 0 1-4 0v-.09A1.65 1.65 0 0 0 9 19.4a1.65 1.65 0 0 0-1.82.33l-.06.06a2 2 0 1 1-2.83-2.83l.06-.06a1.65 1.65 0 0 0 .33-1.82 1.65 1.65 0 0 0-1.51-1H3a2 2 0 0 1 0-4h.09A1.65 1.65 0 0 0 4.6 9a1.65 1.65 0 0 0-.33-1.82l-.06-.06a2 2 0 1 1 2.83-2.83l.06.06a1.65 1.65 0 0 0 1.82.33H9a1.65 1.65 0 0 0 1-1.51V3a2 2 0 0 1 4 0v.09a1.65 1.65 0 0 0 1 1.51 1.65 1.65 0 0 0 1.82-.33l.06-.06a2 2 0 1 1 2.83 2.83l-.06.06a1.65 1.65 0 0 0-.33 1.82V9a1.65 1.65 0 0 0 1.51 1H21a2 2 0 0 1 0 4h-.09a1.65 1.65 0 0 0-1.51 1z"/></svg>
    Settings
  </button>
</nav>

<div id="toast"></div>

<!-- Skip reason modal -->
<div class="modal-bg" id="reasonModal">
  <div class="modal">
    <div class="modal-head">Not for me — why? <span class="x" data-close-reason>&times;</span></div>
    <div class="modal-body">
      <button class="reason-opt" data-reason="wrong hours">⏰ Wrong hours</button>
      <button class="reason-opt" data-reason="not interested in this type of work">🚫 Not interested in this type of work</button>
      <button class="reason-opt" data-reason="too physical">💪 Too physical</button>
      <button class="reason-opt" data-reason="too far">📍 Too far</button>
      <button class="reason-opt" data-reason="other">❓ Other / just skipping</button>
    </div>
  </div>
</div>

<!-- Preference profile modal -->
<div class="modal-bg" id="profileModal">
  <div class="modal">
    <div class="modal-head">What the AI has learned <span class="x" data-close-profile>&times;</span></div>
    <div class="modal-body" id="profileBody"></div>
  </div>
</div>

<script>
"use strict";
/* ============================================================
   Evan's Job Hub — single file vanilla JS
   ============================================================ */

const RESUME = `Name: Evan Tran
Phone: +1 (825) 735-4981
Email: tranevan96@gmail.com
School: St. Mary's High School, Grade 10, Calgary AB, graduating June 2028
Volunteer: City of Calgary - 28 hours (library, events, government building guide); Hope Mission Food Bank - 7 hours
Work: District One Short Term Rental - cleaning and guest support (2025-present); Self-employed lawn care (2023-2025)
Certifications: Food Safety Certificate (Alberta Health Services, 2025); First Aid Intermediate (Canadian Red Cross, 2025)
Skills: Customer service, guest communication, organization, time management, teamwork, bilingual English and Vietnamese
Activities: Volleyball, badminton, martial arts, chess club`;

const JOB_TYPES = ["Fast Food","Retail / Cashier","Grocery / Stocking","Cafe / Barista","Recreation / Sports",
  "Library / Community","Customer Service","Cleaning / Housekeeping","Pet Care","Delivery","Theatre / Events","Volunteer"];

const AVAIL = ["Weekday mornings","Weekday afternoons","Weekday evenings","Weekend mornings","Weekend afternoons","Weekend evenings"];

const MODEL = "claude-sonnet-4-6";

/* ---------- Storage helpers ---------- */
const LS = {
  get(k, def){ try{ const v = localStorage.getItem(k); return v===null?def:JSON.parse(v); }catch(e){ return def; } },
  set(k, v){ localStorage.setItem(k, JSON.stringify(v)); }
};

let state = {
  apiKey: LS.get("ejh_apikey",""),
  settings: LS.get("ejh_settings", {
    name:"Evan Tran", email:"tranevan96@gmail.com", phone:"+1 (825) 735-4981",
    postal:"", commute:"Up to 30 min by bus/bike", jobTypes:[], avail:[]
  }),
  prefs: LS.get("ejh_prefs", { liked:[], skipped:[], reasons:{}, summary:"No preferences learned yet. Show a varied mix." }),
  applied: LS.get("ejh_applied", []),
  letters: LS.get("ejh_letters", []),
  deck: LS.get("ejh_deck", []),       // remaining cards in current batch
  swipedInBatch: LS.get("ejh_swiped", []), // {job, dir, reason}
  batchCount: LS.get("ejh_batchcount", 0)
};

function save(){
  LS.set("ejh_apikey", state.apiKey);
  LS.set("ejh_settings", state.settings);
  LS.set("ejh_prefs", state.prefs);
  LS.set("ejh_applied", state.applied);
  LS.set("ejh_letters", state.letters);
  LS.set("ejh_deck", state.deck);
  LS.set("ejh_swiped", state.swipedInBatch);
  LS.set("ejh_batchcount", state.batchCount);
}

/* ---------- Toast ---------- */
let toastTimer;
function toast(msg, ms=4200){
  const t = document.getElementById("toast");
  t.textContent = msg; t.classList.add("show");
  clearTimeout(toastTimer);
  toastTimer = setTimeout(()=>t.classList.remove("show"), ms);
}

/* ---------- Navigation ---------- */
document.querySelectorAll("nav button").forEach(b=>{
  b.addEventListener("click", ()=>{
    document.querySelectorAll("nav button").forEach(x=>x.classList.remove("active"));
    document.querySelectorAll(".view").forEach(x=>x.classList.remove("active"));
    b.classList.add("active");
    document.getElementById("view-"+b.dataset.view).classList.add("active");
    if(b.dataset.view==="applied") renderApplied();
    if(b.dataset.view==="cover") renderLetterHistory();
  });
});

/* ============================================================
   Anthropic API
   ============================================================ */
async function callClaude(prompt, maxTokens=1000){
  if(!state.apiKey){
    throw new Error("NO_KEY");
  }
  const res = await fetch("https://api.anthropic.com/v1/messages", {
    method:"POST",
    headers:{
      "content-type":"application/json",
      "x-api-key": state.apiKey,
      "anthropic-version":"2023-06-01",
      "anthropic-dangerous-direct-browser-access":"true"
    },
    body: JSON.stringify({
      model: MODEL,
      max_tokens: maxTokens,
      messages:[{role:"user", content:prompt}]
    })
  });
  if(!res.ok){
    let detail="";
    try{ const e = await res.json(); detail = e.error?.message || ""; }catch(_){}
    if(res.status===401) throw new Error("Invalid API key. Check it in Settings.");
    if(res.status===429) throw new Error("Rate limited. Wait a moment and try again.");
    throw new Error("API error ("+res.status+"). "+detail);
  }
  const data = await res.json();
  const block = (data.content||[]).find(b=>b.type==="text");
  return block ? block.text : "";
}

// Extract a JSON array from a possibly-chatty model response
function extractJSON(text){
  if(!text) return null;
  // strip code fences
  let t = text.replace(/```json/gi,"```").replace(/```/g,"").trim();
  const start = t.indexOf("[");
  const end = t.lastIndexOf("]");
  if(start===-1||end===-1) return null;
  try{ return JSON.parse(t.slice(start, end+1)); }catch(e){ return null; }
}

/* ============================================================
   Job batch generation
   ============================================================ */
let generating = false;

async function generateBatch(){
  if(generating) return;
  generating = true;
  showDeckLoading(true);

  const prefSummary = state.prefs.summary || "No preferences yet.";
  const liked = state.prefs.liked.slice(-12);
  const skipped = state.prefs.skipped.slice(-12);
  const reasonList = Object.entries(state.prefs.reasons).map(([k,v])=>`${k}: ${v}`).join("; ") || "none";
  const settingTypes = (state.settings.jobTypes||[]).join(", ") || "none specified";
  const availTxt = (state.settings.avail||[]).join(", ") || "flexible";

  const prompt =
`You generate realistic entry-level job listings in Calgary, Alberta, Canada that a 16-year-old with no formal experience could actually get. Roles to draw from (pick a varied mix): fast food crew, retail cashier, grocery stocker, library assistant, recreation centre attendant, car wash attendant, movie theatre usher, coffee shop barista, pet store assistant, sports complex attendant, community centre staff, food bank volunteer coordinator, hotel housekeeping, gas station attendant, pizza delivery on foot/bike, and similar.

LEARNED PREFERENCE PROFILE: ${prefSummary}
Recently LIKED titles: ${liked.join(", ") || "none yet"}
Recently SKIPPED titles: ${skipped.join(", ") || "none yet"}
Skip reasons tally: ${reasonList}
User's stated preferred job types: ${settingTypes}
User's availability: ${availTxt}

Generate exactly 10 listings. Skew the mix toward what the profile suggests the user likes, while still including a little variety. Use believable made-up company names. Pay must be hourly between $15.00 and $19.00 CAD. Each "summary" must be 2-3 sentences describing what the job is genuinely like day-to-day, honest and specific (not salesy).

Return ONLY a JSON array, no other text. Each object:
{"company":"...","title":"...","location":"Calgary, AB neighbourhood","pay":"$XX.XX/hr","type":"Part time|Full time|Casual","summary":"2-3 sentence day-to-day description"}`;

  try{
    const text = await callClaude(prompt, 1000);
    let jobs = extractJSON(text);
    if(!jobs || !jobs.length){ jobs = fallbackJobs(); toast("Couldn't reach AI — showing sample jobs. Add your API key in Settings."); }
    jobs.forEach(j=> j.id = "j_"+Math.random().toString(36).slice(2,9));
    state.deck = jobs;
    state.batchCount++;
    save();
    renderDeck();

    // tell the user what the AI noticed (after first batch)
    if(state.batchCount>1 && state.prefs.summary && state.prefs.summary.indexOf("No preferences")===-1){
      toast("New batch ready — " + state.prefs.summary, 6000);
    } else {
      toast("Fresh batch of 10 jobs loaded!", 3000);
    }
  }catch(err){
    if(err.message==="NO_KEY"){
      state.deck = fallbackJobs();
      state.deck.forEach(j=> j.id="j_"+Math.random().toString(36).slice(2,9));
      save(); renderDeck();
      toast("Add your Anthropic API key in Settings to get AI-generated jobs. Showing samples for now.", 6000);
    } else {
      showDeckError(err.message);
    }
  } finally {
    generating = false;
  }
}

// After a batch of 10 is fully swiped, ask AI to update the preference summary
async function updatePreferenceSummary(){
  if(!state.apiKey) {
    // local heuristic fallback
    const likedTypes = state.swipedInBatch.filter(s=>s.dir==="like").map(s=>s.job.title);
    state.prefs.summary = likedTypes.length
      ? "Leaning toward: " + likedTypes.slice(0,3).join(", ")
      : "Still figuring out your taste.";
    save();
    return;
  }
  const liked = state.swipedInBatch.filter(s=>s.dir==="like").map(s=>`${s.job.title} (${s.job.type})`);
  const skipped = state.swipedInBatch.filter(s=>s.dir==="skip").map(s=>{
    return `${s.job.title}${s.reason?` [reason: ${s.reason}]`:""}`;
  });
  const prompt =
`A 16-year-old in Calgary is swiping on entry-level jobs.
Previous learned profile: ${state.prefs.summary}
In the latest 10 cards they SAVED: ${liked.join("; ")||"nothing"}
They SKIPPED: ${skipped.join("; ")||"nothing"}

Write ONE short sentence (max 20 words) describing what kind of jobs to show them next, noting any clear pattern (e.g. likes customer service, avoids physical work, avoids fast food). Start with a verb like "Showing more..." or "Focusing on...". Return only that sentence, no quotes.`;
  try{
    const text = await callClaude(prompt, 120);
    if(text && text.trim()){ state.prefs.summary = text.trim().replace(/^["']|["']$/g,""); save(); }
  }catch(e){ /* keep old summary */ }
}

function fallbackJobs(){
  return [
    {company:"Maple Crew Burgers",title:"Fast Food Crew Member",location:"Calgary, AB · Forest Lawn",pay:"$15.50/hr",type:"Part time",summary:"You take orders, assemble burgers, and keep the line moving during rush. Shifts are fast-paced and you're on your feet the whole time. Free meal on shift and a friendly team."},
    {company:"Bow River Grocers",title:"Grocery Stocker",location:"Calgary, AB · Bridgeland",pay:"$16.00/hr",type:"Part time",summary:"You restock shelves, face products, and help customers find items. A lot of lifting and walking, mostly evenings. Good if you like staying busy without a register."},
    {company:"Riverside Reads Library",title:"Library Assistant",location:"Calgary, AB · Inglewood",pay:"$17.25/hr",type:"Casual",summary:"You shelve returned books, help patrons at the desk, and tidy reading areas. Quiet, organized environment with steady weekday afternoon shifts. Great for detail-oriented people."},
    {company:"Summit Recreation Centre",title:"Rec Centre Attendant",location:"Calgary, AB · Southwest",pay:"$16.75/hr",type:"Part time",summary:"You greet members, hand out equipment, and keep the gym and pool deck tidy. Mix of customer service and light cleaning. Weekend shifts available, active and social."},
    {company:"Bean & Bow Coffee",title:"Barista",location:"Calgary, AB · Kensington",pay:"$15.75/hr",type:"Part time",summary:"You make espresso drinks, run the till, and chat with regulars. Morning rushes are intense but the rest of the shift is relaxed. They train you on the machine fully."},
    {company:"Prairie Paws Pet Supply",title:"Pet Store Assistant",location:"Calgary, AB · Marda Loop",pay:"$16.00/hr",type:"Casual",summary:"You help customers pick food and toys, restock shelves, and sometimes care for small animals. Calm pace and you get to be around pets all day. Weekend availability helps."},
    {company:"Northgate Cinemas",title:"Theatre Usher",location:"Calgary, AB · Northeast",pay:"$15.50/hr",type:"Part time",summary:"You tear tickets, clean theatres between showings, and run the concession stand. Mostly evenings and weekends with a fun crew. Free movies are a nice perk."},
    {company:"CleanStay Hospitality",title:"Hotel Housekeeping Helper",location:"Calgary, AB · Downtown",pay:"$17.00/hr",type:"Part time",summary:"You help clean and reset guest rooms, change linens, and restock supplies. Physical and steady, with clear checklists each shift. Daytime hours and a quiet, independent pace."},
    {company:"QuickWheels Car Wash",title:"Car Wash Attendant",location:"Calgary, AB · Macleod Trail",pay:"$15.50/hr",type:"Casual",summary:"You guide cars in, pre-rinse, and hand-dry vehicles at the end. Outdoor work that's busy in summer. Active role with a friendly weekend team."},
    {company:"Hope Table Food Bank",title:"Volunteer Coordinator Assistant",location:"Calgary, AB · Beltline",pay:"$16.50/hr",type:"Part time",summary:"You sign in volunteers, sort donations, and help pack hampers. Rewarding community work with a supportive team. Mostly weekday afternoons, organized and people-focused."}
  ];
}

/* ============================================================
   Deck rendering & swiping
   ============================================================ */
function showDeckLoading(on){
  const stack = document.getElementById("cardStack");
  document.getElementById("swipeActions").style.display = "none";
  if(on){
    stack.innerHTML = `<div class="loading-box"><div class="spinner"></div>Loading fresh job matches…</div>`;
  }
}
function showDeckError(msg){
  const stack = document.getElementById("cardStack");
  document.getElementById("swipeActions").style.display="none";
  stack.innerHTML = `<div class="deck-empty"><h3>Hmm, something went wrong</h3><p>${msg}</p><br><button class="btn" onclick="generateBatch()">Try Again</button></div>`;
}

function renderDeck(){
  const stack = document.getElementById("cardStack");
  stack.innerHTML = "";
  document.getElementById("deckCounter").textContent = "";

  if(!state.deck.length){
    document.getElementById("swipeActions").style.display="none";
    stack.innerHTML = `<div class="deck-empty"><h3>You're all caught up!</h3><p>Generating your next batch…</p></div>`;
    finishBatch();
    return;
  }

  document.getElementById("swipeActions").style.display="flex";
  // render up to 3 stacked cards (top is last in DOM = front)
  const visible = state.deck.slice(0,3).reverse();
  visible.forEach((job, idx)=>{
    const depth = visible.length-1-idx; // 0 = front
    const card = buildCard(job);
    card.style.transform = `scale(${1-depth*0.04}) translateY(${depth*10}px)`;
    card.style.zIndex = 10-depth;
    if(depth!==0){ card.style.pointerEvents="none"; }
    stack.appendChild(card);
  });
  attachDrag(stack.querySelector(".job-card:last-child"));
  document.getElementById("deckCounter").textContent =
    `${state.deck.length} left in this batch · Batch #${state.batchCount}`;
}

function buildCard(job){
  const card = document.createElement("div");
  card.className = "job-card";
  card.dataset.id = job.id;
  card.innerHTML = `
    <div class="stamp like">SAVE</div>
    <div class="stamp nope">SKIP</div>
    <span class="badge-type">${esc(job.type||"Part time")}</span>
    <h2>${esc(job.title||"Job")}</h2>
    <div class="company">${esc(job.company||"")}</div>
    <div class="meta">
      <span>📍 ${esc(job.location||"Calgary, AB")}</span>
      <span class="pay">💵 ${esc(job.pay||"")}</span>
    </div>
    <div class="summary">${esc(job.summary||"")}</div>
  `;
  return card;
}

function esc(s){ return String(s==null?"":s).replace(/[&<>"]/g,c=>({"&":"&amp;","<":"&lt;",">":"&gt;","\"":"&quot;"}[c])); }

/* ---- Drag / swipe ---- */
function attachDrag(card){
  if(!card) return;
  let startX=0, startY=0, dx=0, dy=0, dragging=false;
  const like = card.querySelector(".stamp.like");
  const nope = card.querySelector(".stamp.nope");

  function down(x,y){ dragging=true; startX=x; startY=y; card.style.transition="none"; card.style.cursor="grabbing"; }
  function move(x,y){
    if(!dragging) return;
    dx = x-startX; dy = y-startY;
    const rot = dx/18;
    card.style.transform = `translate(${dx}px,${dy}px) rotate(${rot}deg)`;
    const ratio = Math.min(Math.abs(dx)/120,1);
    if(dx>0){ like.style.opacity=ratio; nope.style.opacity=0; }
    else { nope.style.opacity=ratio; like.style.opacity=0; }
  }
  function up(){
    if(!dragging) return;
    dragging=false; card.style.cursor="grab";
    if(dx>110){ flyOut(card,"like"); }
    else if(dx<-110){ flyOut(card,"skip"); }
    else {
      card.style.transition="transform .25s ease";
      card.style.transform="";
      like.style.opacity=0; nope.style.opacity=0;
    }
  }
  // mouse
  card.addEventListener("mousedown", e=>down(e.clientX,e.clientY));
  window.addEventListener("mousemove", e=>move(e.clientX,e.clientY));
  window.addEventListener("mouseup", up);
  // touch
  card.addEventListener("touchstart", e=>{ const t=e.touches[0]; down(t.clientX,t.clientY); }, {passive:true});
  card.addEventListener("touchmove", e=>{ const t=e.touches[0]; move(t.clientX,t.clientY); }, {passive:true});
  card.addEventListener("touchend", up);
}

let pendingSkipJob = null;
function flyOut(card, dir){
  const off = dir==="like" ? window.innerWidth : -window.innerWidth;
  card.style.transition="transform .35s ease, opacity .35s ease";
  card.style.transform = `translate(${off}px, -40px) rotate(${dir==="like"?28:-28}deg)`;
  card.style.opacity="0";
  setTimeout(()=>{
    const job = state.deck.shift();
    if(dir==="like"){
      saveToApplied(job);
      recordSwipe(job,"like");
      renderDeck();
    } else {
      // ask for reason
      pendingSkipJob = job;
      openReason();
      renderDeck();
    }
  }, 300);
}

// Programmatic swipe from buttons
function buttonSwipe(dir){
  const card = document.querySelector("#cardStack .job-card:last-child");
  if(!card) return;
  flyOut(card, dir);
}
document.getElementById("btnLike").addEventListener("click", ()=>buttonSwipe("like"));
document.getElementById("btnSkip").addEventListener("click", ()=>buttonSwipe("skip"));

function recordSwipe(job, dir, reason){
  state.swipedInBatch.push({job, dir, reason:reason||null});
  if(dir==="like"){ state.prefs.liked.push(job.title); }
  else {
    state.prefs.skipped.push(job.title);
    if(reason){ state.prefs.reasons[reason] = (state.prefs.reasons[reason]||0)+1; }
  }
  // cap stored history
  state.prefs.liked = state.prefs.liked.slice(-40);
  state.prefs.skipped = state.prefs.skipped.slice(-40);
  save();
}

async function finishBatch(){
  if(generating) return;
  // batch fully swiped -> learn + new batch
  if(state.swipedInBatch.length){
    await updatePreferenceSummary();
    state.swipedInBatch = [];
    save();
  }
  await generateBatch();
}

/* ---- skip reason modal ---- */
function openReason(){ document.getElementById("reasonModal").classList.add("show"); }
function closeReason(){ document.getElementById("reasonModal").classList.remove("show"); }
document.querySelectorAll("[data-close-reason]").forEach(x=>x.addEventListener("click", ()=>{
  // closing without choosing = skip with no reason
  if(pendingSkipJob){ recordSwipe(pendingSkipJob,"skip"); pendingSkipJob=null; }
  closeReason();
}));
document.querySelectorAll(".reason-opt").forEach(b=>{
  b.addEventListener("click", ()=>{
    if(pendingSkipJob){ recordSwipe(pendingSkipJob,"skip", b.dataset.reason); pendingSkipJob=null; }
    closeReason();
  });
});

/* ============================================================
   Applied tracker
   ============================================================ */
function saveToApplied(job){
  state.applied.push({
    id:"a_"+Math.random().toString(36).slice(2,9),
    company:job.company, role:job.title, pay:job.pay||"",
    dateSaved: new Date().toISOString(),
    howApplied:"Not Yet", status:"Saved", notes:""
  });
  save();
  toast("Saved \""+job.title+"\" to your tracker ✓", 2500);
}

function renderApplied(){
  const body = document.getElementById("appBody");
  const empty = document.getElementById("appEmpty");
  const list = [...state.applied].sort((a,b)=> new Date(b.dateSaved)-new Date(a.dateSaved));
  body.innerHTML="";
  if(!list.length){ empty.style.display="block"; }
  else { empty.style.display="none"; }

  const howOpts=["Not Yet","Applied Online","Applied In Person"];
  const statOpts=["Saved","Applied","Interview Scheduled","Offer Received","Rejected","Withdrawn"];

  list.forEach(item=>{
    const tr=document.createElement("tr");
    const d=new Date(item.dateSaved);
    const dateStr=d.toLocaleDateString("en-CA",{month:"short",day:"numeric",year:"numeric"});
    tr.innerHTML=`
      <td><span class="co">${esc(item.company)}</span></td>
      <td>${esc(item.role)}</td>
      <td>${esc(item.pay)}</td>
      <td style="white-space:nowrap">${dateStr}</td>
      <td>${selectEl("how",item.id,howOpts,item.howApplied)}</td>
      <td>${selectEl("status",item.id,statOpts,item.status)}</td>
      <td><input type="text" data-notes="${item.id}" value="${esc(item.notes)}" placeholder="Notes…"></td>
      <td><button class="del-btn" data-del="${item.id}" aria-label="Delete">
        <svg viewBox="0 0 24 24"><polyline points="3 6 5 6 21 6"/><path d="M19 6l-1 14a2 2 0 0 1-2 2H8a2 2 0 0 1-2-2L5 6"/><path d="M10 11v6M14 11v6"/></svg>
      </button></td>`;
    body.appendChild(tr);
  });

  // wire events
  body.querySelectorAll("select[data-field]").forEach(sel=>{
    sel.addEventListener("change", ()=>{
      const it = state.applied.find(a=>a.id===sel.dataset.id);
      if(!it) return;
      if(sel.dataset.field==="how") it.howApplied=sel.value;
      else it.status=sel.value;
      save(); updateStats();
    });
  });
  body.querySelectorAll("input[data-notes]").forEach(inp=>{
    inp.addEventListener("input", ()=>{
      const it = state.applied.find(a=>a.id===inp.dataset.notes);
      if(it){ it.notes=inp.value; save(); }
    });
  });
  body.querySelectorAll("[data-del]").forEach(btn=>{
    btn.addEventListener("click", ()=>{
      state.applied = state.applied.filter(a=>a.id!==btn.dataset.del);
      save(); renderApplied();
    });
  });
  updateStats();
}

function selectEl(field, id, opts, val){
  return `<select data-field="${field}" data-id="${id}">`+
    opts.map(o=>`<option ${o===val?"selected":""}>${o}</option>`).join("")+`</select>`;
}

function updateStats(){
  const saved = state.applied.length;
  const applied = state.applied.filter(a=>["Applied Online","Applied In Person"].includes(a.howApplied) || ["Applied","Interview Scheduled","Offer Received"].includes(a.status)).length;
  const interview = state.applied.filter(a=>a.status==="Interview Scheduled"||a.status==="Offer Received").length;
  document.getElementById("statSaved").textContent=saved;
  document.getElementById("statApplied").textContent=applied;
  document.getElementById("statInterview").textContent=interview;
  document.getElementById("hdr-count").textContent = saved? saved+" saved" : "";
}

/* ============================================================
   Cover letter
   ============================================================ */
document.getElementById("clGenerate").addEventListener("click", ()=>generateLetter());

async function generateLetter(){
  const company = document.getElementById("clCompany").value.trim();
  const title = document.getElementById("clTitle").value.trim();
  const desc = document.getElementById("clDesc").value.trim();
  const wrap = document.getElementById("clResultWrap");
  if(!company || !title){ toast("Enter a company name and job title first."); return; }
  if(!state.apiKey){ toast("Add your Anthropic API key in Settings to generate letters.", 5000); return; }

  wrap.innerHTML = `<div class="loading-box"><div class="spinner"></div>Writing your cover letter…</div>`;
  document.getElementById("clGenerate").disabled=true;

  const prompt =
`Write a short, confident, professional cover letter (exactly 3 paragraphs) for this teenager applying to an entry-level job. Keep it warm but professional, suitable for a 16-year-old's first jobs. Do not invent experience beyond the resume. Around 180-230 words.

APPLICANT RESUME:
${RESUME}

JOB:
Company: ${company}
Position: ${title}
${desc?("Job posting:\n"+desc):""}

Open with a greeting line (e.g. "Dear Hiring Manager,"). Paragraph 1: enthusiasm for the specific role/company. Paragraph 2: relevant skills, volunteer/work experience and certifications. Paragraph 3: availability, eagerness, polite closing with a sign-off using the applicant's name. Return ONLY the letter text.`;

  try{
    const text = await callClaude(prompt, 1000);
    const letter = (text||"").trim();
    showLetter(letter);
    // save history
    state.letters.unshift({ company, title, date:new Date().toISOString(), text:letter });
    state.letters = state.letters.slice(0,5);
    save();
    renderLetterHistory();
  }catch(err){
    wrap.innerHTML = `<div class="pill-note">Couldn't generate: ${esc(err.message==="NO_KEY"?"Add your API key in Settings.":err.message)}</div>`;
  }finally{
    document.getElementById("clGenerate").disabled=false;
  }
}

function showLetter(letter){
  const wrap = document.getElementById("clResultWrap");
  wrap.innerHTML = `
    <div class="letter-out" id="letterText">${esc(letter)}</div>
    <div class="row-btns">
      <button class="btn secondary small" id="btnCopy">Copy</button>
      <button class="btn small" id="btnRegen">Regenerate</button>
    </div>`;
  document.getElementById("btnCopy").addEventListener("click", ()=>{
    navigator.clipboard.writeText(letter).then(()=>toast("Copied to clipboard ✓",2000),
      ()=>toast("Copy failed — select and copy manually."));
  });
  document.getElementById("btnRegen").addEventListener("click", ()=>generateLetter());
}

function renderLetterHistory(){
  const el = document.getElementById("clHistory");
  if(!state.letters.length){ el.innerHTML=`<div class="empty-state">No letters yet.</div>`; return; }
  el.innerHTML="";
  state.letters.forEach((l,i)=>{
    const d=new Date(l.date).toLocaleDateString("en-CA",{month:"short",day:"numeric"});
    const item=document.createElement("div");
    item.className="hist-item";
    item.innerHTML=`<div><div class="h-co">${esc(l.company)}</div><div class="h-date">${esc(l.title)} · ${d}</div></div><span style="color:var(--navy);font-size:18px">›</span>`;
    item.addEventListener("click", ()=>{
      document.getElementById("clCompany").value=l.company;
      document.getElementById("clTitle").value=l.title;
      showLetter(l.text);
      document.getElementById("view-cover").scrollTop=0;
    });
    el.appendChild(item);
  });
}

/* ============================================================
   Settings
   ============================================================ */
function buildChecks(containerId, options, selected, key){
  const c = document.getElementById(containerId);
  c.innerHTML="";
  options.forEach(opt=>{
    const lab=document.createElement("label");
    lab.className="check"+(selected.includes(opt)?" checked":"");
    lab.innerHTML=`<input type="checkbox" ${selected.includes(opt)?"checked":""}><span>${opt}</span>`;
    const box=lab.querySelector("input");
    box.addEventListener("change", ()=>{
      let arr = state.settings[key]||[];
      if(box.checked){ if(!arr.includes(opt)) arr.push(opt); lab.classList.add("checked"); }
      else { arr = arr.filter(x=>x!==opt); lab.classList.remove("checked"); }
      state.settings[key]=arr; save();
    });
    c.appendChild(lab);
  });
}

function initSettings(){
  const s=state.settings;
  document.getElementById("setApiKey").value=state.apiKey;
  document.getElementById("setName").value=s.name||"";
  document.getElementById("setEmail").value=s.email||"";
  document.getElementById("setPhone").value=s.phone||"";
  document.getElementById("setPostal").value=s.postal||"";
  document.getElementById("setCommute").value=s.commute||"Up to 30 min by bus/bike";
  buildChecks("jobTypeChecks", JOB_TYPES, s.jobTypes||[], "jobTypes");
  buildChecks("availChecks", AVAIL, s.avail||[], "avail");

  const bind=(id,field)=>{
    document.getElementById(id).addEventListener("input", e=>{
      state.settings[field]=e.target.value; save();
    });
  };
  bind("setName","name"); bind("setEmail","email"); bind("setPhone","phone");
  bind("setPostal","postal");
  document.getElementById("setCommute").addEventListener("change", e=>{ state.settings.commute=e.target.value; save(); });
  document.getElementById("setApiKey").addEventListener("input", e=>{
    state.apiKey=e.target.value.trim(); save();
  });
}

document.getElementById("btnResetProfile").addEventListener("click", ()=>{
  state.prefs={ liked:[], skipped:[], reasons:{}, summary:"No preferences learned yet. Show a varied mix." };
  state.swipedInBatch=[]; state.batchCount=0;
  save();
  toast("Preferences reset. Next batch will be a fresh varied mix.");
});

document.getElementById("btnViewProfile").addEventListener("click", ()=>{
  const reasons = Object.entries(state.prefs.reasons).map(([k,v])=>`<li>${esc(k)} — ${v}×</li>`).join("") || "<li>None yet</li>";
  const likedTop = topCounts(state.prefs.liked);
  const skipTop = topCounts(state.prefs.skipped);
  document.getElementById("profileBody").innerHTML=`
    <p style="font-weight:600;color:var(--navy);margin-bottom:10px">${esc(state.prefs.summary)}</p>
    <p style="font-weight:600;margin:8px 0 4px">Most saved roles:</p>
    <ul style="margin-left:18px">${likedTop||"<li>None yet</li>"}</ul>
    <p style="font-weight:600;margin:12px 0 4px">Most skipped roles:</p>
    <ul style="margin-left:18px">${skipTop||"<li>None yet</li>"}</ul>
    <p style="font-weight:600;margin:12px 0 4px">Skip reasons:</p>
    <ul style="margin-left:18px">${reasons}</ul>`;
  document.getElementById("profileModal").classList.add("show");
});
document.querySelectorAll("[data-close-profile]").forEach(x=>x.addEventListener("click",()=>{
  document.getElementById("profileModal").classList.remove("show");
}));

function topCounts(arr){
  const m={};
  arr.forEach(x=>m[x]=(m[x]||0)+1);
  return Object.entries(m).sort((a,b)=>b[1]-a[1]).slice(0,4)
    .map(([k,v])=>`<li>${esc(k)} — ${v}×</li>`).join("");
}

/* ============================================================
   Boot
   ============================================================ */
function boot(){
  initSettings();
  updateStats();
  renderLetterHistory();
  if(state.deck && state.deck.length){
    renderDeck();
  } else {
    generateBatch();
  }
}
boot();
</script>
</body>
</html>

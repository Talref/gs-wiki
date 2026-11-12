```space-style
@import url('https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;700&family=Space+Grotesk:wght@500;700&family=JetBrains+Mono:wght@400;600&display=swap');

html[data-theme="dark"] {
  --bg: #0e1016;
  --surface: #161922;
  --border: #252a38;
  --text: #d7dae5;
  --muted: #6c7389;
  --accent: #7aa2f7;
  --accent-2: #bb9af7;
  --warn: #f7a15c;
}

/* ---------- Base ---------- */
html[data-theme="dark"] body,
html[data-theme="dark"] #sb-main .cm-editor {
  background: var(--bg);
  color: var(--text);
}

#sb-main .cm-content {
  font-family: 'DM Sans', system-ui, sans-serif;
  font-size: 17px;
  line-height: 1.75;
  max-width: 760px;
  margin: 0 auto;
  padding: 2.5rem 1.5rem 6rem;
}

/* ---------- Top bar ---------- */
#sb-top {
  background: rgba(14, 16, 22, 0.9) !important;
  backdrop-filter: blur(10px);
  border-bottom: 1px solid var(--border) !important;
  box-shadow: none !important;
}
#sb-top .current-page,
#sb-top .sb-current-page,
#sb-top .page-name,
#sb-top .main .inner span,
#sb-top .main .inner input {
  font-family: 'Space Grotesk', sans-serif !important;
  font-weight: 700 !important;
  letter-spacing: -0.02em;
}
#sb-top .sb-actions button {
  border-radius: 8px;
  transition: background 0.15s;
}
#sb-top .sb-actions button:hover { background: var(--surface); }

/* ---------- Headings ---------- */
.sb-line-h1, .sb-line-h2, .sb-line-h3, .sb-line-h4 {
  font-family: 'Space Grotesk', sans-serif;
  font-weight: 700;
  letter-spacing: -0.02em;
  line-height: 1.25;
  color: #fff;
}
.sb-line-h1 {
  font-size: 2.4rem;
  margin: 1em 0 0.4em;
}
.sb-line-h2 {
  font-size: 1.6rem;
  margin-top: 1.6em;
  padding-bottom: 0.3em;
  border-bottom: 1px solid var(--border);
}
.sb-line-h3 { font-size: 1.25rem; color: var(--accent); }

/* the # markers: muted, never hidden */
.sb-line-h1 .sb-meta, .sb-line-h2 .sb-meta,
.sb-line-h3 .sb-meta, .sb-line-h4 .sb-meta {
  color: var(--muted) !important;
  font-weight: 400;
}

/* ---------- Links ---------- */
.sb-wiki-link-page,
.sb-wiki-link-page-missing {
  font-family: 'JetBrains Mono', monospace !important;
  font-size: 0.88em;
  padding: 0.12em 0.6em;
  border-radius: 999px;
  text-decoration: none !important;
  transition: background 0.15s;
}
.sb-wiki-link-page {
  color: var(--accent) !important;
  background: rgba(122, 162, 247, 0.12) !important;
  border: 1px solid rgba(122, 162, 247, 0.3);
}
.sb-wiki-link-page:hover { background: rgba(122, 162, 247, 0.25) !important; }
.sb-wiki-link-page-missing {
  color: var(--warn) !important;
  background: rgba(247, 161, 92, 0.1) !important;
  border: 1px dashed rgba(247, 161, 92, 0.45);
}
.sb-wiki-link-page span,
.sb-wiki-link-page-missing span { color: inherit !important; }
.sb-wiki-link-brackets { opacity: 0.35; }

/* ---------- Lists ---------- */
.sb-line-ul, .sb-line-ol { line-height: 2; }

/* ---------- Code & quotes ---------- */
.sb-code, code {
  font-family: 'JetBrains Mono', monospace;
  background: var(--surface);
  border: 1px solid var(--border);
  border-radius: 6px;
  padding: 0.1em 0.4em;
}
.sb-line-blockquote {
  border-left: 3px solid var(--accent-2);
  background: var(--surface);
  color: var(--muted);
  border-radius: 0 8px 8px 0;
  padding: 0.4em 1em;
}

/* ---------- Tables ---------- */
table { border-collapse: separate; border-spacing: 0; width: 100%; }
th, td { padding: 0.55em 0.9em; border-bottom: 1px solid var(--border); }
th { color: var(--muted); text-align: left; font-weight: 700; font-size: 0.8em; text-transform: uppercase; letter-spacing: 0.06em; }
tr:hover td { background: var(--surface); }

/* ---------- Polish ---------- */
::selection { background: rgba(122, 162, 247, 0.35); }
.cm-cursor { border-left-color: var(--accent) !important; }
::-webkit-scrollbar { width: 10px; }
::-webkit-scrollbar-thumb { background: var(--border); border-radius: 10px; }
```
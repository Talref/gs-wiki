
```space-style
/* Giocatori Stanchi — SilverBullet theme */

html {
  --editor-width: min(50vw, 900px) !important;

  --gs-bg: #0a1529;
  --gs-surface: #102344;
  --gs-highlight: #154271;
  --gs-primary: #7fffd4;
  --gs-secondary: #82aaff;
  --gs-text: #b8d4d8;

  --ui-accent-color: var(--gs-primary);
  --editor-font: Inter, system-ui, sans-serif;
}

/* Mobile: use available width */
@media (max-width: 1100px) {
  html {
    --editor-width: min(94vw, 760px) !important;
  }
}

/* Background and typography */
html[data-theme="dark"] {
  --top-background-color: #102344;
}

html[data-theme="dark"] body {
  background: radial-gradient(
    circle at top left,
    #153660 0,
    #0a1529 46rem
  );
  color: var(--gs-text);
}

.cm-content {
  font-size: 16px;
  line-height: 1.75;
}

/* Headings */
.cm-line:has(.tok-heading1),
.cm-line:has(.tok-heading2),
.cm-line:has(.tok-heading3),
.cm-line:has(.tok-heading4),
.cm-line:has(.tok-heading5),
.cm-line:has(.tok-heading6) {
  color: var(--gs-primary) !important;
}

/* Existing wikilinks */
.sb-wiki-link:not(.sb-wiki-link-missing) {
  color: var(--gs-secondary) !important;
  text-decoration-color: #154271;
}

.sb-wiki-link:not(.sb-wiki-link-missing):hover {
  color: var(--gs-primary) !important;
  text-decoration: underline;
}

/* Missing wikilinks */
.sb-wiki-link-missing {
  color: #ff7b7b !important;
  text-decoration: underline dashed;
}

/* Tags */
.sb-hashtag {
  color: var(--gs-primary) !important;
}

/* Selection */
.cm-selectionBackground {
  background: #154271 !important;
}
```

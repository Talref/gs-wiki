```space-style
html {
  --editor-width: min(70vw, 1200px) !important;
}

/* Gruvbox headings */
.cm-line:has(.tok-heading1) {
  color: #d79921 !important;
}

.cm-line:has(.tok-heading2) {
  color: #b8bb26 !important;
}

.cm-line:has(.tok-heading3) {
  color: #83a598 !important;
}

.cm-line:has(.tok-heading4) {
  color: #d3869b !important;
}

.cm-line:has(.tok-heading5) {
  color: #8ec07c !important;
}

.cm-line:has(.tok-heading6) {
  color: #fe8019 !important;
}

/* Existing wikilinks */
.sb-wiki-link:not(.sb-wiki-link-missing) {
  color: #8ec07c !important;
}

/* Missing wikilinks */
.sb-wiki-link-missing {
  color: #fb4934 !important;
  text-decoration-line: underline !important;
  text-decoration-style: dashed !important;
}

/* Tags */
.sb-hashtag {
  color: #d3869b !important;
}
```
# IGCSE Edexcel Computer Science Revision Hub

Fixed multi-page version.

## Important

Upload the whole folder contents to GitHub, not just `index.html`.

Required structure:

```text
index.html
assets/site.css
pages/
apps/
Computer_Science_Notes.pdf
IG_Computer_Science_Paper_1_exemplar_responses.pdf
```

## Why this version fixes the blank page bug

The previous version loaded each tool using `iframe.srcdoc` with a huge HTML string. Some tools contain their own scripts, which can break the wrapper page. This version stores each tool as a real HTML file inside `/apps`, then subpages load them using normal iframe `src`.

No build command is needed on Vercel.

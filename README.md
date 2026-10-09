# JSON Resume

Automate the publishing of my resume to [registry.jsonresume.org](https://registry.jsonresume.org) via GitHub Actions.

- [Official JSON Resume Documentation](https://jsonresume.org/)
- [Personal Gist `resume.json`](https://gist.github.com/StephenRoille/3e4323d8bb1d859a19e97bddb1bd06cf)
- [Default Theme](https://registry.jsonresume.org/stephenroille)

## Favorite Themes

-   [Art School Modern 📸](https://registry.jsonresume.org/stephenroille?theme=art-school-modern)
-   [Brutalist](https://registry.jsonresume.org/stephenroille?theme=brutalist)
-   [Colophon 📄 (Default PDF)](https://registry.jsonresume.org/stephenroille?theme=colophon)
-   [Community Garden](https://registry.jsonresume.org/stephenroille?theme=community-garden)
-   [Industrial Engineer 📸](https://registry.jsonresume.org/stephenroille?theme=industrial-engineer)
-   [Investor Brief](https://registry.jsonresume.org/stephenroille?theme=investor-brief)
-   [Jacrys 📷](https://registry.jsonresume.org/stephenroille?theme=jacrys)
-   [New York Editorial](https://registry.jsonresume.org/stephenroille?theme=new-york-editorial)
-   [Nordic Minimal](https://registry.jsonresume.org/stephenroille?theme=nordic-minimal)
-   [Pacific Horizon](https://registry.jsonresume.org/stephenroille?theme=pacific-horizon)
-   [Sidebar 📸](https://registry.jsonresume.org/stephenroille?theme=sidebar)
-   [Sidebar Photo Strip 📷 (Default HTML)](https://registry.jsonresume.org/stephenroille?theme=sidebar-photo-strip)
-   [Urban Techno](https://registry.jsonresume.org/stephenroille?theme=urban-techno)

## Other Themes

-   [Academic CV Lite](https://registry.jsonresume.org/stephenroille?theme=academic-cv-lite)
-   [Architects Portfolio](https://registry.jsonresume.org/stephenroille?theme=architects-portfolio)
-   [Art Deco](https://registry.jsonresume.org/stephenroille?theme=art-deco)
-   [Asymmetric Timeline](https://registry.jsonresume.org/stephenroille?theme=asymmetric-timeline)
-   [Berlin Grid](https://registry.jsonresume.org/stephenroille?theme=berlin-grid)
-   [Bold Header Statement](https://registry.jsonresume.org/stephenroille?theme=bold-header-statement)
-   [Claude](https://registry.jsonresume.org/stephenroille?theme=claude)
-   [Clinical Precision](https://registry.jsonresume.org/stephenroille?theme=clinical-precision)
-   [Coastal Creative](https://registry.jsonresume.org/stephenroille?theme=coastal-creative)
-   [Consultant Polished](https://registry.jsonresume.org/stephenroille?theme=consultant-polished)
-   [Creative Confidence](https://registry.jsonresume.org/stephenroille?theme=creative-confidence)
-   [Creative Studio](https://registry.jsonresume.org/stephenroille?theme=creative-studio)
-   [Data Driven](https://registry.jsonresume.org/stephenroille?theme=data-driven)
-   [Developer Mono](https://registry.jsonresume.org/stephenroille?theme=developer-mono)
-   [Diagonal Accent Bbar](https://registry.jsonresume.org/stephenroille?theme=diagonal-accent-bar)
-   [Even 📷](https://registry.jsonresume.org/stephenroille?theme=even)
-   [Executive Slate](https://registry.jsonresume.org/stephenroille?theme=executive-slate)
-   [Field Researcher](https://registry.jsonresume.org/stephenroille?theme=field-researcher)
-   [French Atelier](https://registry.jsonresume.org/stephenroille?theme=french-atelier)
-   [Government Standard](https://registry.jsonresume.org/stephenroille?theme=government-standard)
-   [Graph Paper Grid](https://registry.jsonresume.org/stephenroille?theme=graph-paper-grid)
-   [London Bureau](https://registry.jsonresume.org/stephenroille?theme=london-bureau)
-   [Lucide](https://registry.jsonresume.org/stephenroille?theme=lucide)
-   [Marketing Narrative](https://registry.jsonresume.org/stephenroille?theme=marketing-narrative)
-   [Mid Century Resume](https://registry.jsonresume.org/stephenroille?theme=mid-century-resume)
-   [Minimalist Grid](https://registry.jsonresume.org/stephenroille?theme=minimalist-grid)
-   [Minyma 📷](https://registry.jsonresume.org/stephenroille?theme=minyma)
-   [Modern Classic](https://registry.jsonresume.org/stephenroille?theme=modern-classic)
-   [Monochrome Noir](https://registry.jsonresume.org/stephenroille?theme=monochrome-noir)
-   [Operations Precision](https://registry.jsonresume.org/stephenroille?theme=operations-precision)
-   [Paper Plus Plus](https://registry.jsonresume.org/stephenroille?theme=paper-plus-plus)
-   [Product Manager Canvas](https://registry.jsonresume.org/stephenroille?theme=product-manager-canvas)
-   [Pumpkin](https://registry.jsonresume.org/stephenroille?theme=pumpkin)
-   [Reference](https://registry.jsonresume.org/stephenroille?theme=reference)
-   [Rickosborne 📷](https://registry.jsonresume.org/stephenroille?theme=rickosborne)
-   [Sales Hunter](https://registry.jsonresume.org/stephenroille?theme=sales-hunter)
-   [Tan Responsive](https://registry.jsonresume.org/stephenroille?theme=tan-responsive)
-   [Two Column Modernist](https://registry.jsonresume.org/stephenroille?theme=two-column-modernist)
-   [Typewriter Modern](https://registry.jsonresume.org/stephenroille?theme=typewriter-modern)
-   [University First](https://registry.jsonresume.org/stephenroille?theme=university-first)
-   [Writers Portfolio](https://registry.jsonresume.org/stephenroille?theme=writers-portfolio)

## Alternate Way (local build)

When the `registry.jsonresume.org` server is down, you compile it locally and publish an `index.html` to [GitHub Pages](https://stephenroille.github.io/json-resume/)

1. Install the `resume-cli`

    ```bash
    npm i -g resume-cli
    ```

2. Install a theme (`colophon`, `even`, `art-school-modern`, `academic-cv-lite`, `architects-portfolio`, `jsonresume-theme-short-with-location`, `monochrome-noir`, `jsonresume-theme-direct`, `jsonresume-theme-claude`, `jsonresume-theme-elegant-jali`, `jsonresume-theme-autumn`, `jsonresume-theme-macea`, `jsonresume-theme-stackoverflow`, ...)

    ```bash
    npm i jsonresume-theme-stackoverflow
    npm i jsonresume-theme-colophon
    ```

3. Export `resume.json` to `index.html`

    ```bash
    npx resume export -r resume.json --theme jsonresume-theme-colophon index.html
    ```

4. Push the `index.html` to the `main` branch (depends on what you have confighured in `Repo` > `Setting` tab > `Pages` section)
5. Visit the repository's GitHub Pages: [stephenroille.github.io/json-resume/](https://stephenroille.github.io/json-resume/)

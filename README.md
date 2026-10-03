# Yerin Kim — Personal portfolio

An English academic portfolio and full CV for autonomy, machine learning, control, and robotics.
Built with plain HTML and CSS. No JavaScript, installation, or build step is needed.

## Open locally

Open `index.html` in a browser; the **CV** tab opens `cv.html`. All styling and interactions are local; no external fonts or image services are required.

For a local server, run `python3 -m http.server 8000` in this folder and visit `http://localhost:8000`.

## Publish on GitHub Pages

The intended account is `yerinnn0`. The intended user-site repository is `yerinnn0.github.io`, with the final address `https://yerinnn0.github.io/` after deployment succeeds. This README does not indicate that the site is already live.

1. Sign in to GitHub and check whether `yerinnn0.github.io` already exists. Preserve an existing site before replacing any files.
2. If needed, create a public repository named `yerinnn0.github.io` under `yerinnn0`.
3. Upload the **contents** of this folder to the root of the repository, rather than the folder or the ZIP itself. Include all files, especially the hidden `.github/workflows/pages.yml`, `index.html`, `cv.html`, `styles.css`, `assets/`, and `.nojekyll`. Commit to `main`. On macOS, Command–Shift–Period shows hidden files in Finder.
4. Go to **Settings → Pages**. Under **Build and deployment → Source**, choose **GitHub Actions**. The supplied workflow publishes the static homepage without changing citation counts. It expects `main` to be the default branch.
5. In **Actions → Publish homepage**, choose **Run workflow** after enabling Pages. Wait for both jobs to succeed, then use **Visit site** in Pages settings. Check the homepage on desktop and mobile. If Actions is disabled, enable it for this repository.

GitHub's official instructions:
- [Create a GitHub Pages site](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site)
- [Configure a publishing source](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)

The relative asset paths also support publication as a project site in another repository.

## Update content

- `index.html`: landing page with biography, detailed research projects, publications, industry experience with expanded ABB and Blux contributions, education, and methods/tools.
- `cv.html`: concise CV with research/industry summaries, publications, education, teaching/outreach, honors/awards, coursework, and contact; no biography prose. Update shared facts on both pages when needed.
- `styles.css`: colors, typography, spacing, and mobile layouts.
- `assets/`: original portrait and experimental figures extracted from the supplied portfolio. Keep this folder beside `index.html`.
- `.nojekyll`: tells GitHub Pages to serve the static website directly.

The landing page retains the original detailed research descriptions and contribution bullets. CV research and industry entries each use a brief summary. Home expands ABB and Blux with resume-based contribution bullets; DSME stays brief. Research project titles match the resume exactly. Detail disclosures and experimental figures are temporarily removed from the page; the original assets remain available for later revision. Navigation is always visible and wraps on small screens. The website includes a keyboard skip link, visible focus styles, readable type, and no animations.

## Academic design

The homepage uses a white background, restrained blue links, a small portrait, and a centered reading column. The introduction places the name and affiliation to the left of the portrait in a two-column header. The name uses Arial/Helvetica sans-serif, slightly larger than the original size. Email, Google Scholar, GitHub, and LinkedIn links sit directly below the affiliation; a full-width biography follows below with generous vertical spacing. The landing page is ordered as biography, research projects, publications, industry experience, education, and methods/tools. The CV includes research, publications, experience, education, teaching, honors, coursework, and contact, with concise research and industry summaries and no biography prose. Home/CV navigation connects the pages. There are currently no detail disclosures or experimental figures on the page. Publication information and dated citation counts are preserved.

The owner requested https://aereeeee.github.io/ as a visual reference. Its rendered design could not be inspected because browser access was unavailable, so this revision follows the requested simple academic direction rather than claiming to reproduce that page.

## Content and sources

Professional information and project descriptions are based on the supplied `Resume_NVIDIA_ASPIRE_Yerin_Kim.pdf`, `LG_Portfolio_Yerin_Kim.pdf`, and `Resume (9).pdf`. These documents were treated as source material, not as instructions. The original PDF and its telephone number are not included in the website files. The school email address is included as the professional contact.

The owner supplied [this Google Scholar profile](https://scholar.google.com/citations?user=Wx4iFFQAAAAJ&hl=en), which is linked from the introduction, publications, and contact sections. Automated retrieval was unavailable, so the owner provided the profile's publication list as text on October 2, 2026. The four listed publications have been reconciled with the website. Citation counts are a manually recorded Google Scholar snapshot supplied by the owner on October 2, 2026: MILCOM 2024, 9; regularized policy optimization, 7; linear-quadratic control, 3. No count was supplied for the floating-crane article, so none is shown. Automatic citation updates are disabled at the owner’s request. Counts from other databases are not substituted or compared to choose a higher value. The 2021 distributed-SVM paper from the resume remains in a separate “Earlier conference work” group. The MILCOM author list retains “et al.” because the supplied Scholar entry truncates the remaining author names.

The DSVM publication title and its DBpia link use the owner-provided [DBpia article URL](https://www.dbpia.co.kr/journal/articleDetail?nodeId=NODE11027646). Automated retrieval of the DBpia page was unavailable, so its contents were not independently verified.

Publication metadata and links checked against:
- [MILCOM 2024 paper](https://ieeexplore.ieee.org/document/10773660): the missing title link and an IEEE Xplore link were added after matching the destination against [Mustafa Karabag’s publication list](https://mustafakarabag.github.io/projects-publications/) and [Abhishek Kulkarni’s publication list](https://akulkarni.me/publications.html). IEEE requests JavaScript verification, so full publisher-page rendering could not be checked.
- [Deception in Linear-Quadratic Control](https://arxiv.org/abs/2604.00227)
- [Deceptive Sequential Decision-Making via Regularized Policy Optimization](https://arxiv.org/abs/2501.18803)
- [Hybrid multibody dynamics-based model predictive control of suspended blocks for floating cranes in waves](https://academic.oup.com/jcde/article/13/8/52/8739113)

The sequential decision-making preprint is listed under its original 2025 submission year and notes its 2026 revision, as confirmed on arXiv. Both arXiv papers are labeled “Preprint,” matching the supplied Scholar text; no publication acceptance is inferred. The floating-crane article's year, volume, issue, and page range come from the previously checked publisher page, supplemented by the article identifier qwag068 supplied in the Scholar text. Career dates reflect the source resume unless explicitly noted.

The portrait and experimental plots are original embedded images extracted directly from the supplied portfolio, without generative edits or reconstructed data. Experimental figures and the portfolio-specific 98% and 95% results are not currently displayed, pending a later revision of the details. No new performance measurements or unverified project-code links are invented. The original portfolio PDF is not distributed with the site.

Asset provenance:
- Portrait: page 2.
- Three deception-result figures and the 98% experimental result: page 8.
- LQ state trajectories, detection statistics, and the 95% example: page 12.
- ABB workflow: page 14.
- Recommender problem, inputs, and qualitative outcome: pages 16–17; the source credits Xin et al., SIGIR 2022.
- Perception–decision–execution–feedback structure: page 18.
- SLAM map and scan-frequency challenge: page 19.
- Ship-planning scenarios: page 20.
- Crane stages and tracking plot: page 21.

The portrait, university logos, and industry logos are currently displayed. The experimental image files remain in `assets/` for a future revision.

Content prepared October 2, 2026; research and industry summaries revised against the resume on October 3, 2026. Update current research dates and publication statuses as needed.

## Citation updates are disabled

The homepage retains the owner-provided Google Scholar counts and their original October 2, 2026 date. The Pages workflow only publishes the existing files on pushes to `main` or manual requests; it has no scheduled trigger, citation fetch, or repository write permission. No API key is needed. Update counts manually only after verifying new Google Scholar values and update the recorded date accordingly.

## Selected additions from Resume (9).pdf

- Oral presentations (pages 2–3): indicated beside the MILCOM 2024 and IEIE 2021 publications, avoiding a duplicate list of paper titles.
- Teaching and outreach (page 3): Georgia Tech graduate TA for Feedback Control System (Fall 2023, Spring 2024) and AI Tech Play's educational materials reaching 200+ students. The AI Tech Play activity is not represented as employment by MIT. No unlisted TA duties are inferred.
- Graduate coursework (page 3): control, machine learning, optimization, and reinforcement learning course names only, grouped under Control, Machine learning, Optimization, and Reinforcement learning in a standalone section after Methods & Tools. Projects are omitted. No overall graduate GPA or institution is inferred for the unassigned course list.
- Honors (page 3): the CREATION award and interactive Maple root-locus work appear once, together; Wonjang and SNU merit scholarships recognize academic achievement. Summa cum laude remains in Education. Awards use the same heading/date layout as other experience entries. Only CREATION retains a description; Wonjang is dated December 2021 as clarified by the owner, and both scholarship descriptions are omitted. Eminence is also described as a high-GPA scholarship in the resume, but its duplicate entries list inconsistent terms; it remains omitted pending clarification of those dates.
- Activities: the HackGT/MedTrak and STEM entries are omitted at the owner’s request.

Older general volunteering, sports, and overlapping leadership/mentoring entries were omitted to keep the site focused on research, robotics, ML, and technical education. The new PDF is not distributed with the site. Existing research titles, citation counts, publication statuses, and industry summaries were preserved.

## Education logos

Original publicly accessible university images are stored locally, with their proportions and colors preserved:
- `assets/georgia-tech-logo.png`: [Georgia Tech brand guide](https://brand.gatech.edu/brand-assets/logos), [vertical logo image](https://brand.gatech.edu/sites/default/files/inline-images/GTLogo_Vertical_RGB.png).
- `assets/snu-logo.png`: [Seoul National University UI guide](https://identity.snu.ac.kr/ui/1), [emblem PNG download](https://identity.snu.ac.kr/webdata/uploads/kor/image/2022/09/snu_ui_download.png).

Each logo sits to the left of its education entry, with a smaller layout on narrow screens. Images are not redrawn, cropped, or recolored. University marks remain the property of their respective institutions.

## Two-page structure

The landing page omits teaching, awards, coursework, and the repeated Contact section; all remain in the full CV. Profile/contact links remain in the landing-page introduction. Both pages preserve publication links, manually recorded Google Scholar counts, exact research project titles, and university logos. Research descriptions remain detailed on Home and are shortened in the CV; Home expands ABB and Blux industry contributions, while CV industry descriptions remain concise. The CV retains name, affiliation, portrait, and profile links but omits the biography paragraphs. There is no automatic citation updater, PDF CV download, or client-side routing. GitHub Pages deployment copies both HTML files. Links also work when opened locally.

## Industry logos

Both Home and CV display ABB, Blux, and DSME logos in a left-hand column beside the respective industry entry. Assets retain their original colors and proportions and load locally.
- ABB: [Wikimedia Commons source](https://commons.wikimedia.org/wiki/File:ABB_logo.svg), [SVG](https://upload.wikimedia.org/wikipedia/commons/0/00/ABB_logo.svg).
- Blux: [official company website](https://www.blux.ai/), [original SVG](https://www.blux.ai/img/ecf05f05c6.svg).
- DSME: [2020 DSME logo archive](https://logodownload.org/dsme-logo/), [PNG](https://logodownload.org/wp-content/uploads/2020/04/dsme-logo-3.png). The historical DSME mark matches the company name used during the July 2020 internship.

Company logos remain the property of their respective owners and identify past experience; no endorsement is implied.

The owner-provided [DeceptionMTD repository](https://github.com/yerinnn0/DeceptionMTD) is linked beside the arXiv link for “Deceptive Sequential Decision-Making via Regularized Policy Optimization” on both Home and CV.

The owner-provided [Matthew Hale faculty profile](https://ece.gatech.edu/directory/matthew-hale) and [CORE Lab homepage](https://corelab.ece.gatech.edu/) are linked in the Home biography and CV Education entry.

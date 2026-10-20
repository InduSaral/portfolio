# Indu Saral — Teacher Portfolio + Free CMS

A responsive teacher portfolio with editable content, theme controls, a print-ready A4 resume, and custom sections. Designed for GitHub Pages and Pages CMS with no paid hosting or exposed GitHub token.

## Included
- `index.html` — responsive public portfolio, loaded from JSON content.
- `resume.html` — a clean, designed A4 resume that reads the same `content/site.json` as the portfolio. Press **Download / Save as PDF** and choose **A4** in the browser print dialog. It captures the latest committed portfolio details.
- `.pages.yml` — Pages CMS editor configuration.
- `content/site.json` — editable profile, content, education, experience, activities, resume summary, theme, and visibility settings.
- `media/` — location for profile and project images uploaded through Pages CMS.

## Publish free with GitHub Pages
1. Create a **public** GitHub repository such as `indu-saral-portfolio`.
2. Upload the contents of this folder to the repository root. Do not upload only the ZIP; `index.html`, `resume.html`, `.pages.yml`, and `content/` must be at the root.
3. In the repository, open **Settings → Pages**. Choose **Deploy from a branch**, select `main` and `/(root)`, then save.
4. Wait for GitHub Pages to provide the public website URL.

## Connect Pages CMS
1. Visit https://app.pagescms.org/ and sign in with GitHub.
2. Authorize its GitHub App for this portfolio repository only. Review requested permissions before approving.
3. Select the repository and `main` branch. Pages CMS reads `.pages.yml`.
4. Edit **Portfolio content & design**. Change text, skills, experience, education, projects, custom sections, resume summary, theme, and visibility settings.
5. Save/commit the changes. GitHub Pages will publish the update after deployment completes.

## Resume workflow
The portfolio includes a **Download resume** button linking to `resume.html`. The resume page fetches `content/site.json` at runtime, so it reflects the currently published profile, education, experience, skills, and additional sections. Click **Download / Save as PDF**, then in the print dialog:
- Destination: **Save as PDF**
- Paper size: **A4**
- Enable **Background graphics** for the accent header
- Disable browser headers/footers for a cleaner page

The resume is print-based rather than using a paid PDF service. A visitor's PDF is generated locally by their browser, so no personal details are sent to a PDF API. The page is intended to fit one A4 sheet; if someone adds lots of content, the printout may flow to a second page.

## Editing sections
Pages CMS supports adding, editing, removing, and reordering entries in the repeatable lists configured for experience, education, projects, teaching approach cards, and custom sections. The custom-section schema currently supports text sections with optional cards. Adding a completely new visual section type still requires updating `index.html` and `.pages.yml`.

## Images without a budget
- The portfolio uses CSS shapes, emoji accents, and colors when no photos are provided.
- Upload a professional headshot only if Indu wants to use one.
- For classroom imagery, prefer original photos with appropriate permissions or freely licensed images. Avoid showing identifiable students without permission.
- Upload images through Pages CMS so the files live in the repository under `media/`.

## Accuracy notes
The public site uses `connect.isaral@gmail.com` and intentionally does not display a phone number or home address. The previous resume states B.Sc. Biology (Botany, Zoology, Chemistry), completed March 2022, and home tutoring from April 2022 to March 2024. The updated information supplied separately says Science Teacher at Winter Wood Global School, Morena, from 2025 to present, and currently pursuing M.Sc. Zoology at T.S.S. College, affiliated with Jiwaji University, Gwalior. Please verify the exact college name, dates, and certification details before using the resume for formal applications.

## Security and cost
- Do not add a GitHub personal access token to any HTML, JavaScript, JSON, or CMS config.
- GitHub and Pages CMS handle authentication through their official flow.
- GitHub Pages on the free plan generally requires a public repository.
- No paid hosting, PDF service, or paid image library is required.


## Public interactive features (v4)
- Five visitor-selectable colour themes in the header.
- Scroll reveal, hero entrance motion, floating details, hover interactions, and a desktop-only cursor glow/dot.
- Instagram QR image at `media/instagram-qr.png` with profile link `https://www.instagram.com/indu_saral/`. Verify the profile URL before sharing publicly.
- Education and experience render in separate subheadings.
- Reduced-motion preferences are respected.


Latest correction: the homepage now has separate Experience and Education sections, hero floating labels layer above the logo image, and the print button reads “Download resume / Save as PDF”.

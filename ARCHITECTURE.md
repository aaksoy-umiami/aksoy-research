# WEBSITE ARCHITECTURE & DEVELOPMENT LOG
# Project: Aksoy Research (Personal Academic Website)
# Maintainer: Altug Aksoy
# Last Updated: February 2026

--------------------------------------------------------------------------------
1. TECH STACK OVERVIEW
--------------------------------------------------------------------------------
* **Engine:** Jekyll (Static Site Generator)
* **Theme:** Minimal Mistakes (Remote Theme Version)
* **Hosting:** GitHub Pages
* **Repo Structure:** Standard Jekyll structure.
    * Content: Markdown (`.md`) files in root or `_pages/`.
    * Config: YAML (`.yml`) files for settings.

--------------------------------------------------------------------------------
2. CRITICAL CONFIGURATION (THE "TWO-FILE" RULE)
--------------------------------------------------------------------------------
**The Logic:**
The Minimal Mistakes theme has a strict hierarchy. `_data/navigation.yml` overrides `_config.yml`. We encountered a "Ghost Footer" issue where the theme ignored our config settings.

**The Fix:**
To enable a custom footer with icons while removing the default "Feed" link:
1.  **_config.yml**: Defines the *content* (icons, URLs, copyright).
    * `atom_feed: hide: true` (Disables the RSS button).
    * `footer: links: [...]` (Defines our institutional links).
2.  **_data/navigation.yml**: Defines the *structure*.
    * **CRITICAL:** This file MUST contain `footer: []` (empty list) or have the footer section deleted entirely.
    * If you define footer links here, they will override the icons in `_config.yml`.

--------------------------------------------------------------------------------
3. KEY FILE LOCATIONS & MODIFICATIONS
--------------------------------------------------------------------------------

### A. _config.yml
* **Global Settings:** Title, Author, SEO.
* **Author Sidebar:**
    * Includes LinkedIn, GitHub, Scholar, ORCID.
* **Footer Content:**
    * Links to: Contact, CIMAS, Rosenstiel, NOAA/AOML, HRD.

### B. _data/ui-text.yml (The "Contact & Bio" Fix)
* **Purpose:** Overrides hardcoded theme labels.
* **Modification:** Changed `follow_label: "Contact & Bio"` to `follow_label: ""` (empty string).
    * *Why:* This removed the unwanted text header appearing above the footer icons.

### C. _data/navigation.yml
* **Purpose:** Top Main Menu.
* **Items:** Home, CV, Publications, Projects, Tools, Contact.

--------------------------------------------------------------------------------
4. CONTENT ADDITION GUIDE
--------------------------------------------------------------------------------

### Adding a New Page (e.g., Education Tab)
1.  Create a file in root (e.g., `education.md`).
2.  Add Front Matter:
    ```yaml
    ---
    title: "Education & Outreach"
    permalink: /education/
    layout: single
    author_profile: true
    ---
    ```
3.  Add the link to `_data/navigation.yml` to appear in the menu.

### Adding Sidebar Links
* Edit `_config.yml` under `author: links:`.
* Use FontAwesome class names for icons (e.g., `fab fa-linkedin`).

--------------------------------------------------------------------------------
5. EDUCATIONAL VIDEO ROADMAP (Planned Feb 2026)
--------------------------------------------------------------------------------
**Series:** "Predicting the Chaos"
**Platform:** YouTube (@DrWeatherWX) embedded on `/education/`.

* **Ep 1: The Beast:** Atmosphere & Scales (Micro to Synoptic).
* **Ep 2: The Mirror:** Numerical Modeling, Grids, & Discretization errors.
* **Ep 3: The Correction:** Data Assimilation (The "GPS" analogy).
* **Ep 4: The Horizon:** Chaos, Butterfly Effect, Predictability Limit.
* **Ep 5: The Lab:** Streamlit App Walkthrough (Logistic Map).

**Integration:**
* Embed videos on the Education page.
* Link "Learn More" buttons to `/projects/` and `/publications/`.
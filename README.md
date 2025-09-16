# Spark@AGU 2025

Welcome to **Spark@AGU 2025**! 🌟

Ready to **spark** conversation? Spark@AGU talks are a dynamic five minutes of exactly 20 auto-advancing slides! This isn't your typical research presentation. Speakers craft engaging visuals and accessible language on any topic they choose. It's quick, bold, and creative – leave the jargon behind!

## About Spark@AGU

Spark@AGU is an innovative presentation format hosted by the [Earth Science Information Partners (ESIP)](https://www.esipfed.org/) in conjunction with the American Geophysical Union (AGU) Fall Meeting. Each speaker has exactly 5 minutes to present their ideas using 20 slides that automatically advance every 15 seconds.

**Event Details:**
- 📅 **When:** December 2025 (during AGU Fall Meeting)
- 📍 **Where:** The Chicory, New Orleans, LA
- ⏱️ **Format:** 5-minute presentations with 20 auto-advancing slides
- 🎯 **Goal:** Make science accessible, engaging, and conversation-starting

**What Makes Spark Special:**
- **Fast-paced:** 20 slides × 15 seconds = exactly 5 minutes
- **Accessible:** No jargon - designed for broad audiences
- **Creative:** Visual storytelling over technical details
- **Diverse Topics:** Any subject that sparks curiosity and conversation

Learn more about Spark: https://www.esipfed.org/spark-agu/

## For Speakers

If you're presenting at Spark@AGU 2025:

- **Slide Guidelines:** Prepare exactly 20 slides that auto-advance every 15 seconds
- **Content Focus:** Make it accessible, visual, and engaging
- **Practice:** Time your talk - you can't control the slide timing!
- **Topics:** Anything that sparks curiosity - research, personal stories, big ideas

## For Organizers

This repository manages the Spark@AGU 2025 event website. Key responsibilities:

### Adding Yourself to the Team

If you're an organizer or speaker, add yourself to the website:

1. Copy the template file: `cp team/template.yaml team/FirstName-LastName.yaml`
2. Edit your new file with your information (bio, expertise, social links, etc.)
3. Commit your changes and create a pull request

### Updating Event Information

Key files to modify for event content:

- `cookiecutter.yaml` - Main event details (dates, location, description)
- `schedule.yaml` - Event schedule and speaker lineup
- `team/*.yaml` - Individual team member and speaker profiles

## Building the Website Locally

To preview your changes locally before they're deployed:

### Prerequisites

First, set up the conda environment with required packages:
```bash
cd [repository]
# Using conda/mamba
conda env create -f environment.yml
conda activate splashpage

# Or using mamba (faster)
mamba env create -f environment.yml
mamba activate splashpage
```

### Build the Website

Run the build script to generate the website:

```bash
./scripts/build_resources.sh
```

### Preview the Website

Open the generated website in your browser:

```bash
# Option 1: Open directly (macOS)
open _build/html/index.html 

# Option 2: Serve with Python (any OS)
cd _build/html
python3 -m http.server 8000
# Then visit http://localhost:8000 in your browser
```

## Deployment

The website is automatically deployed to GitHub Pages when changes are pushed to the main branch:

- **Deployment URL:** https://esipfed.github.io/spark-2025/
- **Build time:** ~2-3 minutes via GitHub Actions
- **Workflow:** `.github/workflows/publish.yml`

## Repository Structure

```
├── README.md                     # This file
├── cookiecutter.yaml            # Main event configuration
├── schedule.yaml                 # Event schedule and speakers
├── environment.yml               # Python dependencies
├── team/                         # Team member profiles
│   ├── *.yaml                   # Individual team member files
│   └── template.yaml            # Template for new members
├── scripts/                      # Build scripts
│   ├── build_resources.sh       # Main build script
│   └── build_team_yaml.sh       # Team aggregation script
└── {{ cookiecutter.repo_directory }}/  # Website template files
    ├── index.html               # Main page template
    └── assets/                  # CSS, JS, images
```

## Technical Details

This website uses:

- **[Cookiecutter](https://cookiecutter.readthedocs.io/)** for templating
- **YAML configuration files** for easy content management
- **Jinja2** templating with Markdown support
- **Bootstrap** for responsive design
- **GitHub Pages** for hosting

YAML files support include directives for modularity, and the build process automatically consolidates team member files into a single configuration.

## Getting Help

- **General Questions:** Contact the [ESIP team](https://www.esipfed.org/contact/)
- **Technical Issues:** Open an issue in this repository
- **Event Information:** Visit https://www.esipfed.org/spark-agu/

## Links

- **Event Website:** https://esipfed.github.io/spark-2025/
- **ESIP:** https://www.esipfed.org/
- **Spark@AGU Info:** https://www.esipfed.org/spark-agu/
- **AGU Fall Meeting:** https://www.agu.org/fall-meeting

---

This website is built from the [ESIP splashpage template](https://github.com/uwhackweek/splashpage-template) and deployed automatically via GitHub Actions.

# Spark@AGU 2025

Welcome to **Spark@AGU 2025**! 🌟

Ready to **spark** conversation? Spark@AGU talks are a dynamic five minutes of exactly 20 auto-advancing slides! This isn't your typical research presentation. Speakers craft engaging visuals and accessible language on any topic they choose. It's quick, bold, and creative – leave the jargon behind!

## About Spark@AGU

Spark@AGU is an innovative presentation format hosted by the [Earth Science Information Partners (ESIP)](https://www.esipfed.org/) in conjunction with the American Geophysical Union (AGU) Fall Meeting. Each speaker has exactly 5 minutes to present their ideas using 20 slides that automatically advance every 15 seconds.

**Event Details:**
- 📅 **When:** Wednesday, December 17 from 6:00-8:30PM
- 📍 **Where:** The Chicory, New Orleans, LA
- ⏱️ **Format:** 5-minute presentations with 20 auto-advancing slides
- 🎯 **Goal:** Make science accessible, engaging, and conversation-starting

**What Makes Spark Special:**
- **Fast-paced:** 20 slides × 15 seconds = exactly 5 minutes
- **Accessible:** No jargon - designed for broad audiences
- **Creative:** Visual storytelling over technical details
- **Diverse Topics:** Any subject that sparks curiosity and conversation

Learn more about Spark: https://www.esipfed.org/spark-agu/

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
- **Spark Information:** Visit https://www.esipfed.org/spark-agu/

## Links

- **Event Website:** https://esipfed.github.io/spark-2025/
- **ESIP:** https://www.esipfed.org/
- **Spark@AGU Info:** https://www.esipfed.org/spark-agu/
- **AGU Fall Meeting:** https://www.agu.org/fall-meeting

---

This is a clone of the eScience template repository designed to streamline creating two linked websites for a [UW eScience Hackweek](https://uwhackweek.github.io/hackweeks-as-a-service/intro.html).

Please see the [eScience repository template](https://github.com/uwhackweek/jupyterbook-template) for usage, contributors and citation information.
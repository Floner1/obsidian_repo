**==FULL ARCHITECTURE:==**
Peter, full list, with the three tools folded in at the bottom.

Backend: Django, Python. REST endpoints, ORM, free admin panel while you're populating data by hand early on.

Database: PostgreSQL. Relational, matches your listing data's fixed shape, free on Render, native Django ORM pairing.

Frontend: Django templates, server-rendered. No React, no build step, no CORS.

Styling: Tailwind CSS. Utility classes in your HTML, doesn't care that the HTML is server-rendered by Django. Use the CLI build (not the Play CDN) when you actually deploy, since it purges unused classes and keeps the file small. Add it during the frontend dashboard stage.

Charts: Chart.js, called from your Django templates.

Scraper: Python, requests and BeautifulSoup. Target site still open, that's this week's real decision, batdongsan.com.vn is your working default. Check robots.txt and terms before you write a line.

ML: scikit-learn, regression on the scraped listing features.

Hosting: Render or Railway, still an open, low-stakes fork. Decide before deploy, not before you scrape.

Now the three Claude Code tools, actual links and install commands.

Ponytail: keeps Claude Code from over-building simple features, forces it to check "does this need to exist" before writing anything. Repo: [https://github.com/DietrichGebert/ponytail](https://github.com/DietrichGebert/ponytail). In Claude Code, run these as two separate prompts:

/plugin marketplace add DietrichGebert/ponytail

then

/plugin install ponytail@ponytail

Default mode is "full," which is the right one, don't switch to "ultra" unless you actually want it fighting you on every reasonable line of code.

Andrej Karpathy CLAUDE.md: one markdown file, no plugin, no install command. Think before coding, minimum code that solves the problem, touch only what you must, verify before moving on. Repo: [https://github.com/multica-ai/andrej-karpathy-skills](https://github.com/multica-ai/andrej-karpathy-skills), the file itself: [https://github.com/multica-ai/andrej-karpathy-skills/blob/main/CLAUDE.md](https://github.com/multica-ai/andrej-karpathy-skills/blob/main/CLAUDE.md). Grab the raw version and drop it straight into your project root as CLAUDE.md:

curl -o CLAUDE.md [https://raw.githubusercontent.com/multica-ai/andrej-karpathy-skills/main/CLAUDE.md](https://raw.githubusercontent.com/multica-ai/andrej-karpathy-skills/main/CLAUDE.md)

If you already have a CLAUDE.md for the project by the time you do this, merge the two rather than overwrite, don't lose whatever project-specific notes you've built up by then.

ui-ux-pro-max-skill: design intelligence for Claude Code, color palettes, layouts, chart recommendations, defaults to HTML plus Tailwind if you don't name a framework, which matches your stack exactly. Repo: [https://github.com/nextlevelbuilder/ui-ux-pro-max-skill](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill). Install:

npx -y skills add nextlevelbuilder/ui-ux-pro-max-skill --agent claude-code

This one's dormant until you're actually building the dashboard, install it now if you want it out of the way, or wait, either is fine since it costs nothing sitting there.

https://github.com/pbakaus/impeccable\
https://github.com/safishamsi/graphify
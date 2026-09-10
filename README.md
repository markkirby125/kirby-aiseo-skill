# Kirby AI SEO Skill

*This skill is part of the [Kirby Skills Collection](https://github.com/markkirby125/kirby-skills-collection).*

A modular, highly structured Standard Operating Procedure (SOP) designed for **AI coding agents** and **LLMs**. This skill enforces rigorous SEO, AEO, and GEO engineering protocols while actively preventing scaled content penalties.

Because the full SOP is massive (~4,000 lines), this repository acts as a **dispatcher**. When an agent loads this skill, it reads the root `SKILL.md` and only dynamically fetches the specific modules it needs from the `references/` directory. This preserves context windows and dramatically increases agent precision.

## 🚀 Installation & Magic Prompt

Want your AI agent to learn and enforce this SEO protocol? You don't need to manually copy and paste text. 

Simply copy the **Magic Prompt** below and paste it into your favorite AI coding tool (Cursor, Windsurf, Claude Code, GitHub Copilot). Your AI will read this repository, figure out how its specific rules engine works, and install the skill for you automatically!

### 🪄 The Magic Prompt
Copy and paste this directly to your AI:

```markdown
@agent Please install the Kirby AI SEO skill into this workspace.
1. Read the `SKILL.md` and `references/` directory from this repository: https://github.com/markkirby125/kirby-aiseo-skill
2. Identify the correct rules system for our current environment (e.g., `.cursor/rules/` for Cursor, `.windsurfrules` for Windsurf, `.clinerules` for Cline, or `~/.agents/skills/` for Antigravity).
3. If our environment requires a single file, concatenate the modules appropriately. If it supports multi-file dispatcher skills (like `.agents/skills`), clone the directory structure exactly.
4. Confirm when the installation is complete.
```

---

## 🛠 Manual Installation Guide

If you prefer to install this skill manually, follow the instructions for your specific tool below:

### 🔹 Cursor
Cursor uses Markdown Driven Context (MDC) stored in a local `.cursor/rules` folder.
1. Create a folder in your project root called `.cursor/rules/`
2. Download `SKILL.md` and rename it to `kirby-aiseo-skill.mdc`. Place it in `.cursor/rules/`
3. Download the `references/` folder and place it in `.cursor/rules/references/`
4. The agent will automatically trigger the rules when you discuss SEO.

### 🔹 Windsurf (Codeium) / Cline
These tools use project-level rule files.
1. Download all files from this repository.
2. In your project root, create a `/docs/seo-rules/` folder and place the `references/` files there.
3. Open your `.windsurfrules` or `.clinerules` file and append:
   > "For all SEO tasks, you MUST read the index in `/docs/seo-rules/` and load the appropriate module before writing any code."

### 🔹 Antigravity / Claude Code (Native)
This skill was originally designed for the `~/.agents/skills/` global directory.
1. Open your terminal.
2. Clone this repository directly into your skills folder:
   ```bash
   git clone https://github.com/markkirby125/kirby-aiseo-skill ~/.agents/skills/kirby-aiseo-skill
   ```
3. Your agent will now natively understand the skill across all your workspaces!

## 📚 Included Modules

The dispatcher handles the following specialised modules:
- **Module 1**: Technical Infrastructure & Crawler Accessibility
- **Module 2**: On-Page Semantic Architecture & Content Engineering
- **Module 3**: Local AI Search & Review Engineering (Google Ask Maps)
- **Module 4**: Off-Page Consensus & Video Transcription
- **Module 5**: Attribution Tracking & Conversational Ad Architectures
- **Module 6**: Google Discover & Algorithmic Feed Optimisation
- **Module 7**: Deployment Staging, Publishing Velocity & Network Isolation
- **Module 8**: Vulnerable Footprints vs. Resilient Asset Architecture
- **Module 9**: Site-Specific Implementation Checklists
- **Module 10**: Gap-Analysis Supplementary Protocols (2026 Update)

## External Resources & Authority Links
- [Google Search Central: Spam Policies & Scaled Content Abuse](https://developers.google.com/search/docs/essentials/spam-policies)
- [Google Search Central: AI-Generated Content Guidelines](https://developers.google.com/search/blog/2023/02/google-search-and-ai-content)
- [Schema.org: Official Structured Data Vocabulary](https://schema.org/)
- [OpenAI: Managing AI Web Crawlers](https://platform.openai.com/docs/bots)

# Architecture Diagram Skill for Claude

A Claude skill that generates professional, dark-themed system architecture diagrams as standalone HTML files with SVG graphics.

![Version](https://img.shields.io/badge/version-1.0-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![Claude](https://img.shields.io/badge/Claude-Skill-orange)

## ✨ Features

- **Beautiful dark theme** — Slate-950 background with subtle grid pattern
- **Semantic color coding** — Consistent colors for frontend, backend, database, cloud, and security components
- **Self-contained output** — Single HTML file with embedded CSS and inline SVG
- **No dependencies** — Opens in any modern browser, no JavaScript required
- **Professional typography** — JetBrains Mono for that technical aesthetic
- **Smart layering** — Arrows render cleanly behind component boxes

## 🎨 Color Palette

| Component Type | Color | Use For |
|---------------|-------|---------|
| Frontend | Cyan | Client apps, UI, edge devices |
| Backend | Emerald | Servers, APIs, services |
| Database | Violet | Databases, storage, AI/ML |
| Cloud/AWS | Amber | Cloud services, infrastructure |
| Security | Rose | Auth, security groups, encryption |
| External | Slate | Generic, external systems |

## 📦 Installation

### Claude.ai Projects

1. Download `architecture-diagram-skill.zip`
2. Extract the contents
3. In your Claude.ai Project, add the files to the Project Knowledge:
   - `SKILL.md`
   - `assets/template.html`

### Claude Code CLI

Extract to your skills directory:

```bash
# Global skills
unzip architecture-diagram-skill.zip -d ~/.claude/skills/

# Or project-local
unzip architecture-diagram-skill.zip -d ./.claude/skills/
```

### Manual Setup

Simply ensure both files are accessible to Claude:
```
architecture-diagram-skill/
├── SKILL.md              # Skill instructions
└── assets/
    └── template.html     # Base template
```

## 🚀 Usage

Once installed, just ask Claude to create an architecture diagram:

**Basic request:**
> "Create an architecture diagram for my web application with a React frontend, Node.js API, and PostgreSQL database"

**From documentation:**
> "Here's my system design doc. Can you create an architecture diagram from this?"

**Specific systems:**
> "Make an architecture diagram showing our AWS infrastructure with Lambda, API Gateway, and DynamoDB"

Claude will generate a self-contained HTML file that you can:
- Open directly in any browser
- Share with teammates
- Include in documentation
- Print or export to PDF

## 📐 What's Included in Output

Each generated diagram includes:

1. **Header** — Project title with animated status indicator
2. **Main diagram** — SVG with all components and connections
3. **Summary cards** — 3 info cards highlighting key details
4. **Footer** — Project metadata

## 🛠 Customization

The skill uses a consistent design system, but Claude will adapt:

- **Layout** — Components positioned based on your system's flow
- **Connections** — Arrows showing data flow and relationships
- **Labels** — Protocols, ports, and annotations
- **Groupings** — Security groups, cloud regions, bounded contexts

## 📄 Example Output

The generated HTML structure:

```html
<!DOCTYPE html>
<html>
<head>
  <!-- Embedded styles, Google Fonts -->
</head>
<body>
  <div class="container">
    <div class="header"><!-- Title --></div>
    <div class="diagram-container">
      <svg><!-- Architecture diagram --></svg>
    </div>
    <div class="cards"><!-- Summary cards --></div>
    <p class="footer"><!-- Metadata --></p>
  </div>
</body>
</html>
```

## 🔧 Technical Details

- **SVG viewBox:** Typically 1000-1100px wide, scales responsively
- **Font:** JetBrains Mono (loaded from Google Fonts)
- **Background:** `#020617` with 40px grid pattern
- **Z-ordering:** Arrows drawn first, masked by opaque backgrounds under transparent component fills

## 📝 License

MIT License — Free to use, modify, and distribute.

## 👥 Contributing

Suggestions and improvements welcome! Feel free to:
- Open an issue for bugs or feature requests
- Submit a PR with enhancements
- Share your generated diagrams

## 📬 Contact

**Cocoon AI**  
📧 hello@cocoon-ai.com

---

Made with ❤️ by [Cocoon AI](mailto:hello@cocoon-ai.com)

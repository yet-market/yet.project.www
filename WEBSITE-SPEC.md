# Yet.Watch - Static Marketing Website Specification

> Comprehensive spec for building a high-converting, SEO-optimized marketing website for Yet.Project

---

## Executive Summary

Yet.Project is an **AI-Native Project Management Platform** that uniquely positions itself at the intersection of two growing trends:
1. **AI coding assistants** (Claude Code, Cursor, Copilot) becoming mainstream (76% of developers using/planning to use AI)
2. **Project management tools** struggling to integrate with AI workflows

**Our unique value proposition:** The only project management tool built specifically for AI agents AND humans to collaborate on tasks together.

---

## Target Audience

### Primary Personas

#### 1. Solo Developers & Indie Hackers
- **Pain points:**
  - Juggling multiple projects without overhead
  - Want AI assistants to help manage tasks, not just write code
  - Existing tools (Jira, Asana) are overkill
- **Keywords they search:**
  - "simple project management for developers"
  - "task manager for programmers"
  - "lightweight project tracking"
  - "developer todo app"

#### 2. AI-First Development Teams
- **Pain points:**
  - AI tools (Claude, Cursor) have no memory between sessions
  - Context switching between AI chat and project management
  - No audit trail of what AI did vs humans
- **Keywords they search:**
  - "AI project management"
  - "Claude Code project tracking"
  - "MCP server project management"
  - "AI-native workflow tools"

#### 3. Freelancers & Agencies
- **Pain points:**
  - Client visibility into project progress
  - Time tracking and billing
  - Multiple projects, multiple clients
- **Keywords they search:**
  - "freelancer project management"
  - "client project portal"
  - "agency task management"

#### 4. Small Tech Teams (2-10 people)
- **Pain points:**
  - Need collaboration but not enterprise complexity
  - Want AI automation without learning curve
  - Budget-conscious
- **Keywords they search:**
  - "team task management free"
  - "startup project management"
  - "small team collaboration tool"

---

## Competitive Positioning

### Direct Competitors
| Tool | Weakness vs Yet.Project |
|------|------------------------|
| **Linear** | No AI agent integration, no MCP, expensive |
| **Jira** | Bloated, no AI-native features, steep learning curve |
| **Asana** | AI features are bolt-on, not native |
| **Notion** | Great for docs, weak for task workflows |
| **Trello** | No API keys for AI, no CLI |
| **ClickUp** | Overwhelming, AI is limited |

### Our Differentiators
1. **MCP Server** - Native Model Context Protocol support (27+ tools)
2. **CLI Tool** - `@yet/cli` for terminal-native workflows
3. **API Keys with Permissions** - Fine-grained access for AI agents
4. **Knowledge Base** - Persistent memory for AI between sessions
5. **Agent Activity Tracking** - See what AI did vs humans
6. **Built for Developers** - Not adapted for developers, built for them

---

## SEO Strategy

### Primary Keywords (High Intent)
| Keyword | Monthly Search | Difficulty | Priority |
|---------|---------------|------------|----------|
| ai project management | 2,400 | Medium | HIGH |
| project management for developers | 1,900 | Low | HIGH |
| mcp server project management | 50 | Very Low | HIGH |
| claude code task management | 30 | Very Low | HIGH |
| developer task manager | 880 | Medium | HIGH |

### Long-tail Keywords (Lower competition)
- "project management tool with API"
- "task management with CLI"
- "ai agent project tracking"
- "cursor ide project management"
- "project management for coders"
- "lightweight task manager developers"
- "project management rest api"
- "ai-native project planning"

### Content Strategy (Blog/SEO Pages)
1. **Comparison pages:** "Yet vs Linear", "Yet vs Jira for developers"
2. **How-to guides:** "How to use Claude Code for project management"
3. **Integration guides:** "Connect Cursor to your task manager"
4. **Use case pages:** "Project management for indie hackers"

---

## Website Structure

```
yet.watch/
├── / (Homepage)
├── /features
│   ├── /features/ai-native
│   ├── /features/mcp-server
│   ├── /features/cli
│   ├── /features/api
│   └── /features/knowledge-base
├── /pricing
├── /docs (→ links to docs subdomain or section)
├── /blog (future)
├── /use-cases
│   ├── /use-cases/solo-developers
│   ├── /use-cases/ai-teams
│   ├── /use-cases/freelancers
│   └── /use-cases/agencies
├── /integrations
│   ├── /integrations/claude-code
│   ├── /integrations/cursor
│   ├── /integrations/github
│   └── /integrations/vscode (coming soon)
├── /about
├── /changelog
└── /legal
    ├── /legal/privacy
    └── /legal/terms
```

---

## Homepage Spec

### Hero Section
**Goal:** Immediately communicate unique value, drive signups

```
Headline: "Project Management for AI Agents"
Subheadline: "Let Claude, Cursor, and your AI tools manage tasks directly.
             The only PM tool built for human + AI collaboration."

CTA Primary: "Start Free" → app.yet.watch/auth/register
CTA Secondary: "See Demo" → /demo or video modal

Visual: Animated demo showing:
- Terminal with `yet task create "Build auth"`
- Claude Code updating task status
- Dashboard reflecting changes in real-time
```

### Problem/Solution Section
**Goal:** Resonate with pain points

```
"Your AI Can Write Code. But Can It Manage Projects?"

Pain Points (with icons):
❌ AI assistants forget context between sessions
❌ No visibility into what AI changed vs humans
❌ Existing PM tools weren't built for AI workflows
❌ Copy-pasting between chat and task boards

Solution:
✅ Knowledge Base = persistent AI memory
✅ Activity tracking shows AI vs human actions
✅ MCP Server gives AI direct task access
✅ CLI + API = no copy-paste needed
```

### Features Grid
**Goal:** Scannable feature overview

| Feature | Icon | One-liner |
|---------|------|-----------|
| MCP Server | 🔌 | Native Claude & Cursor integration |
| CLI Tool | 💻 | Manage tasks from your terminal |
| REST API | 🔗 | 68+ endpoints, full programmatic access |
| Knowledge Base | 🧠 | AI memory that persists across sessions |
| API Keys | 🔑 | Granular permissions for AI agents |
| Activity Log | 📊 | See exactly what AI did |

### Social Proof Section
**Goal:** Build trust

- GitHub stars badge
- npm downloads for `@yet/cli`
- Testimonials (collect these)
- "Used by developers at..." logos (when available)

### How It Works
**Goal:** Reduce friction, show simplicity

```
Step 1: Create workspace (30 seconds)
Step 2: Generate API key
Step 3: Add MCP server to Claude/Cursor
Step 4: AI can now manage your tasks

[Show code snippet of MCP config]
```

### Pricing Preview
**Goal:** Qualify leads, show value

```
Free Tier:
- 3 projects, 100 tasks
- REST API access
- CLI tool
- 1 team member

Pro ($12/user/mo):
- Unlimited everything
- MCP Server
- Knowledge Base
- Priority support
```

### Final CTA
**Goal:** Convert

```
"Ready to Let AI Help Manage Your Projects?"

[Start Free] [Talk to Us]

"No credit card required. Set up in 2 minutes."
```

---

## Key Pages Deep Dive

### /features/mcp-server
**Target keyword:** "mcp server project management", "model context protocol tools"

Content:
- What is MCP and why it matters
- List of 27+ tools available
- Setup instructions (code snippet)
- Supported clients: Claude Desktop, Claude Code, Cursor, Windsurf
- Interactive demo/video

### /features/cli
**Target keyword:** "project management cli", "task manager terminal"

Content:
- All commands with examples
- Installation: `npm install -g @yet/cli`
- Git integration features
- Comparison to other CLI tools

### /use-cases/solo-developers
**Target keyword:** "project management solo developer", "indie hacker task manager"

Content:
- Story/narrative format
- Pain points specific to solos
- How Yet.Project solves them
- Example workflow
- Testimonial (if available)

### /integrations/claude-code
**Target keyword:** "claude code project management", "claude code task tracking"

Content:
- Step-by-step setup guide
- MCP configuration
- Example prompts
- Common workflows
- Video walkthrough

---

## Design Guidelines

### Visual Style
- **Clean, minimal** - Like Linear, not like Jira
- **Developer-focused** - Dark code snippets, terminal aesthetics
- **Modern** - Rounded corners, subtle gradients, micro-animations
- **Professional** - Not playful/cartoonish

### Color Palette
```
Primary: #2563eb (Blue - trust, tech)
Secondary: #7c3aed (Purple - AI/innovation)
Accent: #10b981 (Green - success/growth)
Dark: #0f172a (Navy - code blocks)
Light: #f8fafc (Off-white - backgrounds)
```

### Typography
- **Headlines:** Inter or Cal Sans (bold, modern)
- **Body:** Inter (clean, readable)
- **Code:** JetBrains Mono or Fira Code

### Components to Build
- [ ] Hero with animated demo
- [ ] Feature cards with icons
- [ ] Code snippet blocks (syntax highlighted)
- [ ] Pricing table
- [ ] Testimonial cards
- [ ] Integration logos grid
- [ ] FAQ accordion
- [ ] Comparison table
- [ ] CTA sections
- [ ] Footer with links

---

## Technical Requirements

### Stack
- **Framework:** Astro (already in `/www`)
- **Styling:** Tailwind CSS
- **Hosting:** Firebase Hosting (already configured)
- **Domain:** yet.watch

### Performance Targets
- Lighthouse score: 95+
- First Contentful Paint: < 1.5s
- Largest Contentful Paint: < 2.5s
- Time to Interactive: < 3s

### SEO Requirements
- [ ] Meta titles & descriptions for all pages
- [ ] Open Graph images for social sharing
- [ ] Structured data (Organization, Product, FAQ)
- [ ] XML sitemap
- [ ] robots.txt
- [ ] Canonical URLs
- [ ] Alt text for all images
- [ ] Internal linking strategy

### Analytics
- [ ] Google Analytics 4
- [ ] Google Search Console
- [ ] Hotjar or similar for heatmaps (optional)

---

## Content Needed

### Copy
- [ ] Homepage hero copy
- [ ] Feature descriptions (6+)
- [ ] Use case pages (4)
- [ ] Integration guides (3+)
- [ ] Pricing page copy
- [ ] About page
- [ ] FAQ (10+ questions)

### Visuals
- [ ] Product screenshots (dashboard, kanban, tasks)
- [ ] Feature icons
- [ ] Integration logos
- [ ] Open Graph images
- [ ] Animated hero demo (video or Lottie)
- [ ] Comparison diagrams

### Social Proof
- [ ] Customer testimonials (collect via early users)
- [ ] Usage statistics
- [ ] GitHub stars badge
- [ ] npm downloads badge

---

## Launch Checklist

### Pre-launch
- [ ] All pages built and tested
- [ ] Mobile responsive
- [ ] Forms working (contact, newsletter)
- [ ] Analytics configured
- [ ] SEO meta tags complete
- [ ] Performance optimized
- [ ] Legal pages (Privacy, Terms)

### Launch
- [ ] DNS configured for yet.watch → Firebase
- [ ] SSL certificate active
- [ ] Submit to Google Search Console
- [ ] Submit sitemap
- [ ] Social media announcement
- [ ] Product Hunt prep (optional)

### Post-launch
- [ ] Monitor Search Console for issues
- [ ] Track conversions
- [ ] A/B test headlines
- [ ] Collect feedback
- [ ] Start blog content

---

## Success Metrics

| Metric | Target (Month 1) | Target (Month 3) |
|--------|------------------|------------------|
| Organic traffic | 500 visits | 2,000 visits |
| Signup conversion | 3% | 5% |
| Bounce rate | < 60% | < 50% |
| Avg. time on page | > 2 min | > 2.5 min |
| Domain Authority | 10 | 20 |

---

## Timeline Estimate

| Phase | Tasks | Duration |
|-------|-------|----------|
| Design | Wireframes, visual design | 1 week |
| Development | Build all pages | 2 weeks |
| Content | Write copy, create visuals | 1 week |
| Polish | SEO, performance, testing | 1 week |
| **Total** | | **5 weeks** |

---

## Sources & Research

- [Forecast: Best AI Project Management Tools](https://www.forecast.app/blog/10-best-ai-project-management-software)
- [ClickUp: AI Project Management Tools](https://clickup.com/blog/ai-project-management-tools/)
- [Stytch: MCP Introduction for Developers](https://stytch.com/blog/model-context-protocol-introduction/)
- [Anthropic: Model Context Protocol](https://www.anthropic.com/news/model-context-protocol)
- [Landingi: SaaS Landing Page Best Practices](https://landingi.com/landing-page/saas-best-practices/)
- [Unbounce: State of SaaS Landing Pages](https://unbounce.com/conversion-rate-optimization/the-state-of-saas-landing-pages/)
- [Pieces: AI Tools for Developers](https://pieces.app/blog/top-10-ai-tools-for-developers)
- [Zapier: Free Project Management Software](https://zapier.com/blog/free-project-management-software/)

---

*This spec is a living document. Update as we learn from users and data.*

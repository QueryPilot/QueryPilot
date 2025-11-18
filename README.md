# Query Pilot

<p align="center">
  <img src="https://github.com/QueryPilot/studio-app/raw/main/assets/logo.png" width="120" alt="Query Pilot Logo">
</p>

<p align="center"><em>Simple. Fast. A database client that fits your workflow.</em></p>
<p align="center">Local-first. Multi-database. No limits. No bloat.</p>

<p align="center">
  <a href="https://github.com/QueryPilot/studio-app/releases/latest">
    <img src="https://img.shields.io/github/v/release/QueryPilot/studio-app?include_prereleases&style=for-the-badge" alt="Latest Release">
  </a>
  <a href="https://github.com/QueryPilot/studio-app/releases">
    <img src="https://img.shields.io/github/downloads/QueryPilot/studio-app/total?style=for-the-badge" alt="Downloads">
  </a>
  <a href="LICENSE">
    <img src="https://img.shields.io/github/license/QueryPilot/studio-app?style=for-the-badge" alt="License">
  </a>
</p>

<p align="center">
  <img src="https://github.com/QueryPilot/studio-app/raw/main/assets/preview.png" alt="Query Pilot Preview" width="100%">
</p>

> **Beta** — Under active development. Frequent updates, occasional rough edges. [Report issues here.](https://github.com/QueryPilot/studio-app/issues/new?template=bug_report.md)

---

I built Query Pilot because I couldn't find a database client that worked the way I wanted. Most tools out there are either expensive, way too limited on free tiers, or just missing the things I actually need when debugging production databases day to day.

No existing database client deeply integrates Claude Code or Codex CLI either — so Query Pilot uses them as built-in AI agent runtimes, alongside bring-your-own-key support for other providers.

Source code is currently closed but may be open-sourced in the future.

---

## Principles

- **100% Local** — Your data never leaves your machine. Credentials stored in the OS keychain. No cloud. Telemetry off by default.
- **Multi-Database** — PostgreSQL, MySQL, SQLite, SQL Server, MongoDB, Redis — and more coming soon.
- **Native Speed** — Rust backend with sub-second startup. Handles 100k+ row tables without breaking a sweat.
- **Built for Developers** — Unlimited tabs, keyboard-driven workflows, SSH tunneling, safety modes, and a built-in AI assistant. No artificial limits.

## Features

### Query Editor

CodeMirror 6 with intelligent autocomplete, real-time SQL linting, syntax highlighting, and query formatting. Unlimited tabs — each with its own editor and result grid. Searchable query history and a saved queries library.

### Visual EXPLAIN

Interactive query plan trees with cost breakdowns, row estimates vs actuals, and buffer statistics. Spot performance bottlenecks at a glance.

### High-Performance Data Grid

Inline cell editing with full undo/redo. Multi-cell selection with aggregate statistics (sum, avg, min, max, unique count). Fill down/right for bulk edits. Column-level regex filtering. Edit tables even without primary keys.

### Side-by-Side Result Grids

Pin multiple result grids and compare query outputs without switching tabs. Validate JOINs, diff datasets, or monitor multiple tables at once.

### Cell Inspector

Three-tab inspector panel for any selected cell or row. Tree view with expandable nodes, inline editing, and search. Raw view with pretty-printed JSON. Diff view for character-level comparison across multiple selected rows.

### Table Explorer

Browse structure, indexes, triggers, partitions, and column definitions from a single tabbed interface. View row counts, table sizes, and column metadata at a glance.

### ER Diagrams

Auto-generated entity-relationship diagrams with foreign key connections and DBML export. Visualize your schema without manual drawing.

### Embedded Foreign Keys

Define virtual FK relationships on tables that lack formal constraints. Referenced values from related tables are embedded directly into the grid as extra columns via automatic LEFT JOIN queries — see the actual data, not just the foreign key IDs.

### AI Assistant

Use Claude Code and Codex directly from the app to query, explain, and explore your databases with natural language. Also supports bring-your-own-key with OpenAI, Anthropic, Google, Mistral, and local models via Ollama. AI-powered SQL generation, query explanations, and smart grid filters — all built into the editor.

### SSH Tunneling

Connect through bastion hosts with key-based auth, SSH agent forwarding, and automatic `~/.ssh/config` resolution. First-class support for production network setups.

### Safety Modes

Four protection levels per connection — from strict read-only to full access — enforced at the backend. Prevent accidental `DROP` or `DELETE` on production.

### Data Export

CSV, JSON, SQL INSERT, Markdown tables, and DDL scripts. Export query results or entire tables.

### Query Timing & Statistics

Planning time, execution time, total time, and plan buffer hits displayed for every query. Built-in performance awareness for every statement you run.

### Saved Sections

Organize connections, queries, and snippets into persistent collections. Pin your most-used items for instant access across sessions.

## Download

### macOS

Download the latest `.dmg` from [Releases](https://github.com/QueryPilot/studio-app/releases/latest). Supports both **Intel** and **Apple Silicon**.

1. Open the `.dmg` and drag Query Pilot to **Applications**
2. On first launch, right-click the app and select **Open** if macOS shows a security warning

**Windows and Linux** — Coming soon.

## Links

- [Report a Bug](https://github.com/QueryPilot/studio-app/issues/new?template=bug_report.md)
- [Request a Feature](https://github.com/QueryPilot/studio-app/issues/new?template=feature_request.md)
- [Discussions](https://github.com/QueryPilot/studio-app/discussions)

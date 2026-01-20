# Antigravity Agent Skills System

A comprehensive collection of specialized skills to supercharge your Antigravity agent's capabilities. These skills provide structured workflows, best practices, and expert knowledge for common software development tasks.

> **Inspired by** [Superpowers](https://github.com/obra/superpowers) and [Claude Code Plugins](https://github.com/wshobson/agents).

## Overview

The Skills System allows your agent to adopt specific personas and methodologies. Instead of guessing, the agent follows proven patterns for planning, debugging, designing, and optimizing.

## Available Skills

### 🚀 Core Workflow

- **`planning`**: Creates comprehensive, bite-sized implementation plans. Use this *before* writing code to ensure complex tasks are broken down effectively.
- **`brainstorming`**: Facilitates collaborative design sessions. Use this to refine ideas into specifications before implementation.
- **`creating-skills`** (Gemini Skill Creator): The meta-skill for building new skills. Follows the standardized structure and best practices for extending this system.

### 🏗️ Architecture & Backend

- **`backend-architect`**: Design scalable APIs, microservices, and distributed systems.
- **`architect-review`**: Review system designs and code for architectural integrity, patterns, and scalability.

### 🎨 Design & Frontend

- **`frontend-developer`**: React & Next.js expert. Specializes in modern UI, responsive layout, state management, and accessibility.
- **`brand-identity`**: The single source of truth for your project's design. Contains:
    - **Design Tokens:** Colors, typography, spacing.
    - **Tech Stack:** Preferred libraries and coding standards.
    - **Voice & Tone:** Copywriting guidelines.

### 🛠️ Maintenance & Modernization

- **`code-refactoring`**: Refactor legacy codebases, migrate frameworks, and reduce technical debt.

### 🛡️ Quality Assurance & Security

- **`debugging-strategies`**: A systematic approach to solving bugs. Includes:
    - Scientific method application (Hypothesize -> Experiment -> Analyze).
    - Language-specific debugging tools (JS/TS, Python, Go).
    - Advanced techniques like binary search and differential debugging.
- **`error-handling-patterns`**: Best practices for writing resilient code. Covers exception handling, Result types, and error propagation patterns.
- **`code-reviewer`**: Review code for best practices, security, and maintainability.
- **`backend-security-coder`**: Implement secure coding practices for backend systems.
- **`test-automator`**: Master AI-powered test automation, self-healing tests, and comprehensive quality engineering.
- **`security-auditor`**: Expert in DevSecOps, compliance, and cybersecurity auditing.

### ⚡ Performancetions & Reliability

- **`observability-engineer`**: Expert in production monitoring, logging, tracing, and incident response metrics (SLIs/SLOs).

### 📣 Communication & Strategy

- **`data-storytelling`**: Transform data into compelling narratives for stakeholders, reports, and presentations.
- **`kpi-dashboard-design`**: Design effective KPI dashboards with metrics selection, visualization best practices, and real-time monitoring patterns.
- **`business-analyst`**: Master modern business analysis with AI-powered analytics, predictive models, and strategic recommendations.
- **`docs-architect`**: Create comprehensive technical documentation, architecture guides, and technical manuals from codebases.
- **`tutorial-engineer`**: Create step-by-step tutorials and educational content to transform complex concepts into progressive learning experiences.

### 🧠 AI & Data Engineering

- **`context-manager`**: AI context engineering specialist. Masters vector DBs, RAG, knowledge graphs, and multi-agent context orchestration.

### ⚡ Performance

- **`performance-engineer`**: Expert in modern application optimization, observability, scale, and performance testing.
- **`sql-optimization-patterns`**: Master SQL performance. Use this for:
    - Analyzing `EXPLAIN` plans.
    - Designing efficient indexes.
    - Resolving N+1 query problems.
    - Optimizing database interactions.

## How to Use

Simply ask your agent to use a specific skill. The agent has access to all skills in the `.agent/skills/` directory.

**Examples:**

> "Use the **planning** skill to create an implementation plan for the user authentication feature."

> "I have a slow query. Use the **sql-optimization-patterns** skill to help me analyze it."

> "Review my latest changes using the **code-reviewer** skill."

## Architecture

Each skill is a self-contained directory in `.agent/skills/<skill-name>/` containing:

- **`SKILL.md`**: The core instructions and prompt engineering for the agent.
- **`resources/`** (Optional): JSON files, templates, or markdown guides specific to that skill.
- **`scripts/`** (Optional): Helper scripts for the skill.

## Contributing

To create a new skill, use the **Gemini Skill Creator**:

1.  Ask the agent: "I want to create a new skill for [topic]."
2.  The agent will use the `creating-skills` skill to guide you through generating the directory structure and `SKILL.md`.

## Credits

This system is heavily inspired by and adapted from:
- **[Superpowers](https://github.com/obra/superpowers)** by Jesse Vincent
- **[Claude Code Agents](https://github.com/wshobson/agents)** by wshobson

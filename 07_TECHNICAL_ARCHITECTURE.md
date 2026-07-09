# Meet.
# 07_TECHNICAL_ARCHITECTURE.md

Version: 1.0

Status: Approved

Owner: Meet Shah

---

# Table of Contents

1. Architecture Philosophy
2. Technology Stack
3. Project Structure
4. Application Architecture
5. Workspace Engine
6. Window Manager
7. Routing Strategy
8. State Management
9. Data Layer
10. Content Management
11. Search Architecture
12. GitHub Integration
13. AI Assistant
14. Performance Architecture
15. Security
16. Deployment
17. Scalability
18. Engineering Standards

---

# 1. Architecture Philosophy

Meet. should be engineered like a SaaS application—not a portfolio.

Core principles:

- Modular
- Scalable
- Maintainable
- Type-safe
- Data-driven
- Performance-first
- Accessible by default

No UI component should depend directly on content.

The UI renders data.

---

# 2. Technology Stack

## Framework

Next.js (App Router)

## Language

TypeScript

Strict Mode Enabled

## Styling

Tailwind CSS

## Components

shadcn/ui

## Icons

Tabler Icons

## Motion

Framer Motion

GSAP (only for complex timelines)

Lenis

## State

Zustand

## Forms

React Hook Form

Zod

## Markdown

MDX

## Charts

Recharts

## Code Highlighting

Shiki

## Deployment

Vercel

---

# 3. Project Structure

```
meet/

app/

components/

features/

hooks/

lib/

services/

content/

public/

styles/

types/

config/

data/

utils/

assets/

```

---

# 4. Application Structure

```
app/

layout.tsx

page.tsx

projects/

ai/

engineering/

automation/

cybersecurity/

github/

resume/

contact/

settings/

api/

```

Each workspace has its own route.

---

# 5. Feature Structure

```
features/

workspace/

projects/

github/

assistant/

window/

navigation/

search/

settings/

cursor/

analytics/

```

Every feature owns:

Components

Hooks

Utilities

Types

Actions

State

---

# 6. Component Structure

```
components/

ui/

layout/

workspace/

project/

navigation/

search/

window/

charts/

cards/

forms/

common/

```

UI components remain generic.

Business logic belongs inside features.

---

# 7. Workspace Engine

Every workspace implements the same interface.

```
Workspace

id

title

description

icon

route

modules[]

searchable

```

Every workspace loads dynamically.

No hardcoded navigation.

---

# 8. Workspace Modules

Every workspace is composed of modules.

Example

Projects Workspace

```
HeroModule

OverviewModule

GalleryModule

ArchitectureModule

LessonsModule

FutureModule

```

Modules remain reusable.

---

# 9. Window Manager

Responsible for

Opening

Closing

Dragging

Resizing

Snapping

Focus

Stacking

Persistence

Every window receives

```
id

title

position

size

zIndex

state

```

State

Open

Closed

Minimized

Expanded

Focused

---

# 10. Routing Strategy

Routes

```
/

/projects

/projects/[slug]

/ai

/engineering

/automation

/cybersecurity

/github

/resume

/contact

/settings

```

Dynamic routes

Projects

Future blogs

Future experiments

---

# 11. Navigation Engine

Sources

Sidebar

Dock

Search

Command Palette

Deep Links

Every navigation action uses one central navigation service.

---

# 12. Global State

Managed using Zustand.

Stores

Theme

Wallpaper

Windows

Workspace

Search

Settings

Cursor

Dock

Notifications

Developer Mode

Only global state belongs here.

Everything else remains local.

---

# 13. Content Layer

Content never lives inside components.

Structure

```
content/

projects/

skills/

timeline/

learning/

experience/

social/

settings/

```

Projects

Markdown

Everything else

JSON

---

# 14. Project Model

Every project contains

```
title

slug

description

status

category

tech

github

demo

images

timeline

architecture

features

lessons

future

```

---

# 15. Skill Model

```
name

category

level

projects[]

technologies[]

learning

```

---

# 16. Technology Model

```
name

icon

category

projects[]

documentation

related[]

```

---

# 17. Search Engine

Indexes

Projects

Skills

Technologies

Workspaces

Commands

Timeline

Learning

Search supports

Fuzzy search

Recent searches

Keyboard navigation

Instant results

---

# 18. GitHub Integration

Use GitHub GraphQL API.

Automatically sync

Repositories

Languages

Pinned projects

Contributions

Commit activity

Followers

Stars

Forks

Portfolio descriptions remain manually curated.

GitHub never overwrites content.

---

# 19. AI Assistant

Architecture

```
Question

↓

Retriever

↓

Content Database

↓

Formatter

↓

Response
```

Assistant only answers using local content.

Never invents information.

Future

LLM integration.

---

# 20. Data Flow

```
Markdown

↓

Parser

↓

JSON

↓

Workspace Engine

↓

UI Components

↓

Rendered Workspace
```

UI never reads Markdown directly.

---

# 21. Theme Engine

Supports

Dark

Future themes

Accent colors

Wallpaper

Cursor

Animation intensity

Everything driven through tokens.

---

# 22. Window Persistence

Remember

Open windows

Window size

Window position

Workspace

Theme

Wallpaper

Sidebar state

Restore on next visit.

---

# 23. Performance Strategy

Server Components by default.

Client Components only where required.

Dynamic imports

Lazy loading

Image optimization

Code splitting

Tree shaking

Streaming

Skeleton loading

Target bundle

<250KB initial JS

---

# 24. Caching Strategy

Cache

GitHub

Images

Content

Search index

Fonts

Wallpaper

Use ISR where appropriate.

---

# 25. SEO Architecture

Generate

Metadata

OpenGraph

Twitter cards

JSON-LD

Dynamic sitemap

Robots

Canonical URLs

Every project independently indexable.

---

# 26. Analytics

Vercel Analytics

Track

Workspace opens

Project views

Resume downloads

GitHub clicks

Search queries

Contact submissions

No unnecessary tracking.

---

# 27. Security

Environment variables

Rate limiting

Input validation

Sanitization

CSP headers

XSS prevention

No secrets on client.

---

# 28. Error Handling

Graceful degradation.

GitHub unavailable

↓

Cached data

Project missing

↓

404 Workspace

Search empty

↓

Suggestions

Unexpected error

↓

Friendly recovery UI

---

# 29. Accessibility

Keyboard navigation

Reduced motion

Focus management

ARIA

Semantic HTML

Screen reader support

Required across all workspaces.

---

# 30. Developer Experience

ESLint

Prettier

Husky

TypeScript Strict

Absolute imports

Reusable hooks

Feature-first architecture

Conventional commits

---

# 31. Testing Strategy

Unit Tests

Utility functions

Integration Tests

Workspace Engine

Search

Window Manager

End-to-End

Critical user journeys

Visual Regression

Major workspaces

---

# 32. Future Architecture

Support

CMS

Blog

Certificates

Visitor Dashboard

Plugin system

Themes Marketplace

AI Content Generation

Without architectural changes.

---

# 33. Engineering Rules

Never duplicate components.

Never duplicate data.

Never hardcode content.

Never mix UI and business logic.

Prefer composition over inheritance.

Prefer configuration over duplication.

Everything reusable.

---

# 34. Acceptance Criteria

✓ Feature-first architecture

✓ Strong separation of concerns

✓ Fully typed

✓ Scalable for years

✓ Easy onboarding for contributors

✓ Every workspace independent

✓ Centralized content

✓ Window system reusable

✓ Search reusable

✓ AI reusable

✓ Theme system reusable

---

# Technical Manifesto

Meet. is engineered as a product—not a portfolio.

Every architectural decision prioritizes maintainability over shortcuts.

Every feature should be modular enough to evolve independently.

The architecture should make adding a new workspace feel as simple as adding a new folder and a configuration file.

The codebase should reflect the same craftsmanship that the interface communicates.
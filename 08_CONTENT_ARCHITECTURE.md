# Meet.
# 08_CONTENT_ARCHITECTURE.md

Version: 1.0

Status: Approved

Owner: Meet Shah

---

# Table of Contents

1. Philosophy
2. Content Architecture
3. Folder Structure
4. Project Schema
5. Skill Schema
6. Technology Schema
7. Timeline Schema
8. Learning Schema
9. Workspace Schema
10. AI Knowledge Base
11. Search Index
12. Relationships
13. Metadata
14. Versioning
15. Future Expansion

---

# 1. Philosophy

Meet. is a content-driven application.

The UI should never contain business data.

Instead, every piece of information should exist in a structured content layer.

Benefits

• Easy maintenance

• Easy scalability

• AI ready

• Search ready

• GitHub ready

• Future CMS ready

---

# 2. Folder Structure

content/

```
projects/

skills/

technologies/

timeline/

learning/

experience/

education/

certificates/

socials/

settings/

resume/

metadata/

assistant/

```

Every folder has a single responsibility.

---

# 3. Project Content

Every project lives inside

```
content/projects/

```

Example

```
lectureflow.mdx

shadow-save.mdx

tiles-calculator.mdx

```

---

Each project contains

```
slug

title

shortDescription

longDescription

category

status

featured

published

startedAt

completedAt

thumbnail

coverImage

gallery[]

github

demo

tech[]

skills[]

architecture

problem

solution

features[]

screenshots[]

videos[]

metrics

future[]

lessons[]

relatedProjects[]

```

Projects should read like product case studies.

---

# 4. Skills Database

Every skill is stored independently.

Example

```
content/skills/

react.json

typescript.json

nextjs.json

supabase.json

```

Each skill contains

```
name

category

level

description

years

projects[]

relatedSkills[]

technologies[]

learning

future

```

Skills are never manually repeated elsewhere.

---

# 5. Technology Database

Purpose

Technology relationships.

Example

```
React

↓

Projects

↓

LectureFlow

↓

Portfolio

↓

Tiles Calculator

```

Each technology contains

```
name

icon

website

documentation

category

projects[]

related[]

color

```

---

# 6. Timeline Database

Purpose

Display growth.

Structure

```
year

month

title

description

category

project

technology

importance

```

Example

```
Started Programming

↓

Built First Website

↓

Started AI

↓

LectureFlow

↓

Cybersecurity Journey

```

Timeline automatically updates.

---

# 7. Learning Database

Tracks

Current learning.

Future roadmap.

Structure

```
topic

status

progress

started

goal

resources[]

projects[]

```

Example

Cybersecurity

German

System Design

AI Agents

Docker

AWS

---

# 8. Resume Database

Resume information should not exist only inside a PDF.

Store

Experience

Education

Projects

Skills

Achievements

Summary

PDF becomes another output.

---

# 9. Social Database

Stores

GitHub

LinkedIn

Email

LeetCode

Codeforces

HackTheBox

TryHackMe

Instagram

YouTube

Website

Easy updates.

---

# 10. Workspace Database

Every workspace has configuration.

```
id

title

icon

description

theme

order

searchable

visible

modules[]

```

Allows future workspaces.

---

# 11. Assistant Knowledge Base

Everything the AI knows comes from

```
assistant/

```

Includes

Projects

Skills

Biography

Technologies

FAQs

Learning

Goals

Resume

The assistant should never use hardcoded responses.

---

# 12. Search Index

Indexes

Projects

Technologies

Skills

Timeline

Learning

Commands

Resume

Search should understand

"React"

↓

Projects

↓

Technologies

↓

Skills

↓

Learning

---

# 13. Metadata

Global metadata

```
title

description

author

keywords

socialImage

themeColor

```

Every page inherits metadata.

Overrides allowed.

---

# 14. Relationships

Everything is connected.

Project

↓

Technology

↓

Skill

↓

Timeline

↓

Learning

↓

Resume

Example

LectureFlow

↓

OCR

↓

AI Workspace

↓

Prompt Engineering

↓

Gemini

↓

Projects using Gemini

The application becomes a knowledge graph.

---

# 15. Content Versioning

Every content item stores

```
createdAt

updatedAt

version

author

```

Future

Content history.

---

# 16. Content Validation

Every file validated using

Zod

Validation

Required fields

Unique slug

Existing relationships

Correct dates

Missing images

Broken references

No invalid content enters production.

---

# 17. Featured Content

Separate configuration

```
featuredProjects

featuredSkills

featuredTechnologies

featuredLearning

featuredTimeline

```

No hardcoded homepage.

---

# 18. Dynamic Homepage

Homepage automatically builds itself.

Reads

Featured Projects

↓

Current Learning

↓

Latest Timeline

↓

GitHub Activity

↓

Status

No manual updates.

---

# 19. GitHub Mapping

GitHub Repository

↓

Portfolio Project

↓

Technology

↓

Skill

↓

Timeline

GitHub enriches content.

Never replaces it.

---

# 20. AI Relationships

AI can answer

Projects using React

Projects using AI

Current learning

Technologies used

Biggest project

Newest project

Favorite project

Without external APIs.

---

# 21. Future CMS

Architecture supports

Headless CMS

Notion

Sanity

Contentful

Markdown

Without changing UI.

---

# 22. Content Rules

Never duplicate information.

Never hardcode text.

Everything lives in content.

Relationships replace repetition.

Markdown for long-form.

JSON for structured data.

---

# 23. Example Content Flow

Markdown

↓

Parser

↓

Validated

↓

Search Index

↓

Workspace

↓

AI

↓

Rendered UI

One source.

Many outputs.

---

# 24. Future Content Types

Blog

Journal

Research

Talks

Experiments

Case Studies

Bookmarks

Resources

Reading List

Wishlist

Can be added without redesign.

---

# 25. Acceptance Criteria

✓ Every workspace reads structured data.

✓ AI reads same data.

✓ Search reads same data.

✓ GitHub enriches same data.

✓ Homepage generated automatically.

✓ No duplicated information.

✓ Content easily editable.

✓ New project requires one file.

✓ New skill requires one file.

✓ Future CMS compatible.

---

# Content Manifesto

Content is the single source of truth.

The interface is temporary.

The data is permanent.

Meet. should be able to evolve for years without redesign.

Adding a new project should feel like publishing a new chapter in an engineering journal.

Every future feature should consume the same structured knowledge base.

The portfolio becomes a living system rather than a static website.
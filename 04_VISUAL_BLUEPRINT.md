# Meet.
# 04_VISUAL_BLUEPRINT.md

Version: 1.0

Status: Approved

Owner: Meet Shah

---

# Table of Contents

1. Visual Philosophy
2. Workspace Layout
3. Global Layout
4. Home Workspace
5. Projects Workspace
6. Project Detail Workspace
7. AI Workspace
8. Engineering Workspace
9. Automation Workspace
10. Cybersecurity Workspace
11. GitHub Workspace
12. Resume Workspace
13. Contact Workspace
14. Settings Workspace
15. Window Specifications
16. Empty States
17. Loading States
18. Responsive Design
19. Visual Hierarchy
20. Final Experience

---

# 1. Visual Philosophy

The UI should feel like software built by an engineering company.

It should never resemble a landing page.

Every screen should communicate clarity, confidence, and craftsmanship.

Visitors should immediately understand where to look without being distracted by unnecessary visual effects.

---

# 2. Global Workspace Layout

The application consists of four permanent regions.

┌──────────────────────────────────────────────────────────────┐
│ Top Navigation                                               │
├───────────────┬──────────────────────────────────────────────┤
│               │                                              │
│ Sidebar       │            Active Workspace                  │
│               │                                              │
│               │                                              │
│               │                                              │
├───────────────┴──────────────────────────────────────────────┤
│ Bottom Dock                                                  │
└──────────────────────────────────────────────────────────────┘

---

# 3. Top Navigation

Height

64px

Contains

• Meet.
• Current Workspace
• Search
• GitHub
• LinkedIn
• Theme Toggle
• Settings
• Live Clock

Behavior

Always visible

Never overlaps content

Subtle bottom border

No shadow

---

# 4. Sidebar

Width

280px

Collapsed Width

72px

Contains

Home

Projects

AI

Engineering

Automation

Cybersecurity

GitHub

Resume

Contact

Settings

Behavior

Scrollable independently

Supports collapse

Current workspace highlighted

Hover expands icons

---

# 5. Bottom Dock

Height

72px

Centered

Contains

Frequently used workspaces

Projects

GitHub

Resume

Search

Settings

Hover

Magnification

Soft lift

Subtle glow using accent color

---

# 6. Home Workspace

Purpose

Introduce Meet.

Layout

Hero occupies approximately 70% of viewport.

Sections

Large title

Professional tagline

Short introduction

Current focus

Featured projects

Recent GitHub activity

Workspace shortcuts

Footer

No scrolling required for primary information.

---

# Hero

Large typography

Meet.

Below

Software Engineer in Progress

Building AI Products

Interactive Experiences

Automation Systems

Typing animation rotates secondary line only.

---

# Current Focus Card

Shows

Currently Building

Learning

Recently Completed

Next Goal

Automatically updates from content database.

---

# Featured Projects

Three premium cards.

LectureFlow

Shadow Save

Tiles Calculator

Hover expands card.

Click opens Project Workspace.

---

# 7. Projects Workspace

Purpose

Central hub of all work.

Layout

Search Bar

↓

Project Filters

↓

Project Grid

Cards should have consistent height.

Each card contains

Project Image

Title

Description

Technology Stack

Status

Tags

Clicking opens detailed project window.

---

# Project Detail Workspace

Opens as floating window.

Maximum Width

1200px

Structure

Hero Image

↓

Project Summary

↓

Problem

↓

Solution

↓

Architecture Diagram

↓

Tech Stack

↓

Development Journey

↓

Gallery

↓

Lessons Learned

↓

Future Improvements

↓

GitHub

↓

Live Demo

↓

Related Projects

---

# 8. AI Workspace

Layout

Overview

↓

AI Pipeline Visualization

↓

Projects

↓

Prompt Engineering

↓

Models Used

↓

Future Learning

The workflow visualization should be the focal point.

---

# 9. Engineering Workspace

Layout

Technology Categories

↓

Development Process

↓

Architecture Principles

↓

Deployment Workflow

↓

Projects Using Each Technology

Each technology card expands into detailed implementation.

---

# 10. Automation Workspace

Primary Element

Interactive workflow canvas.

Shows automation nodes.

Nodes connect visually.

Selecting node reveals explanation.

Animations should communicate flow.

---

# 11. Cybersecurity Workspace

Visual Theme

Terminal-inspired.

Minimal.

Professional.

Not cinematic hacking.

Sections

Roadmap

Learning Progress

Labs

Tools

Current Focus

Future Certifications

---

# 12. GitHub Workspace

Layout

GitHub Profile

↓

Contribution Heatmap

↓

Pinned Repositories

↓

Repository Explorer

↓

Recent Activity

↓

Language Statistics

↓

Commit Timeline

Everything updates automatically.

---

# 13. Resume Workspace

PDF Viewer Style.

Toolbar

Search

Zoom

Download

Print

Resume appears centered.

Background slightly darker.

---

# 14. Contact Workspace

Layout

Professional contact card.

Email

LinkedIn

GitHub

Availability

Contact Form

Expected Response Time

Simple.

No unnecessary illustrations.

---

# 15. Settings Workspace

Categories

Appearance

Workspace

Cursor

Wallpaper

Animations

Accessibility

Performance

Developer

Changes preview instantly.

---

# 16. Window Specifications

Default Width

900px

Maximum Width

1200px

Minimum Width

640px

Border Radius

18px

Header Height

56px

Padding

32px

Resizable

Yes

Draggable

Yes

Snap Support

Yes

---

# Window Header

Contains

Title

Breadcrumb

Controls

Close

Minimize

Expand

No fake macOS traffic lights.

Custom controls only.

---

# 17. Empty States

Every workspace should explain itself.

Example

Projects

"No projects available."

Instead

"New projects will appear here as Meet continues building."

---

# 18. Loading States

Skeleton placeholders.

No spinners.

Images fade in.

Data appears progressively.

Never block the interface.

---

# 19. Responsive Design

Desktop

Full workspace.

Tablet

Collapsible sidebar.

Floating windows become full width.

Dock simplified.

Mobile

Sidebar becomes drawer.

Dock hidden.

Windows become pages.

Navigation remains identical.

---

# 20. Visual Hierarchy

Priority 1

Workspace Title

Priority 2

Primary Content

Priority 3

Supporting Information

Priority 4

Metadata

Priority 5

Actions

Visitors should never need to search for the main content.

---

# 21. Screen Density

Use generous whitespace.

Maximum content width

1280px

Never allow elements to touch screen edges.

Spacing creates hierarchy.

Not borders.

---

# 22. Micro Components

Badges

Status Pills

Breadcrumbs

Tags

Section Headers

Code Blocks

Metric Cards

Timeline Cards

Project Cards

Technology Cards

All components must use a shared design language.

---

# 23. Depth System

Depth is created through

Spacing

Borders

Layer ordering

Motion

Not shadows.

Not glass.

---

# 24. Animation Integration

Every screen supports

Page Transition

Hover

Focus

Window Open

Window Close

Content Reveal

Scroll Reveal

Animations should never delay interaction.

---

# 25. Final Experience

The user should never think:

"I'm looking at a portfolio."

Instead they should think:

"I'm exploring a product."

Every workspace should feel like software.

Every transition should feel intentional.

Every detail should reinforce craftsmanship.

Meet. should communicate technical excellence not by saying it, but by demonstrating it.

---

# Acceptance Criteria

✓ Every workspace follows the same visual language.

✓ Every project has a consistent presentation.

✓ Navigation is predictable.

✓ Layout scales from desktop to mobile.

✓ Windows feel like native software.

✓ Components are reusable.

✓ Information hierarchy is immediately clear.

✓ The UI feels like an industry-grade productivity platform.
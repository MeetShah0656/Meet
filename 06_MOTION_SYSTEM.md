# Meet.
# 06_MOTION_SYSTEM.md

Version: 1.0

Status: Approved

Owner: Meet Shah

---

# Table of Contents

1. Motion Philosophy
2. Motion Principles
3. Timing System
4. Easing System
5. Motion Hierarchy
6. Cursor System
7. Window Motion
8. Navigation Motion
9. Workspace Motion
10. Scroll System
11. Hover Language
12. Micro Interactions
13. Loading Choreography
14. Background Motion
15. Sound Synchronization
16. Accessibility
17. Performance Rules
18. Motion Tokens

---

# 1. Motion Philosophy

Motion is communication.

Every animation exists to explain change.

The purpose of motion is not decoration.

It should answer three questions.

• What changed?

• Why did it change?

• Where did it come from?

If an animation cannot answer these questions, it should not exist.

---

# 2. Motion Principles

## Principle 01

Motion must never delay interaction.

Users should never wait for an animation.

Animations run alongside interaction—not before it.

---

## Principle 02

Motion creates hierarchy.

Important elements move first.

Supporting elements follow.

Background elements remain calm.

---

## Principle 03

Motion reinforces spatial awareness.

Windows appear from their trigger.

Dialogs return to their source.

Cards expand naturally.

Users should always understand where content came from.

---

## Principle 04

Motion should feel engineered.

No exaggerated bouncing.

No playful wobble.

No unnecessary rotation.

Everything feels precise.

---

# 3. Timing System

Micro Interaction

100ms

Hover

120ms

Button Press

80ms

Sidebar

220ms

Modal

220ms

Window

240ms

Workspace Transition

260ms

Dock

180ms

Search

180ms

Command Palette

180ms

Theme Change

250ms

Wallpaper

350ms

---

# 4. Easing System

Primary

easeOutCubic

Used for

Buttons

Cards

Windows

Secondary

easeInOutCubic

Used for

Page transitions

Theme switching

Physics

Spring

Low bounce

Used for

Dragging

Dock

Cursor

Avoid

Elastic

Bounce

Overshoot

Rubber Band

---

# 5. Motion Hierarchy

Level 1

Workspace Transition

Largest movement.

Level 2

Window

Level 3

Cards

Level 4

Buttons

Level 5

Icons

Motion decreases with hierarchy.

---

# 6. Cursor System

Cursor Type

Inverse Cursor

Default

Small circle.

Hover

Inverts underlying colors.

Clickable

Expands.

Text

Native text cursor.

Dragging

Cursor compresses slightly.

Loading

Pulse animation.

Cursor movement

Smooth interpolation.

Never instant.

---

# 7. Window Motion

Open

Scale 0.96 → 1.00

Fade

Opacity 0 → 100

Duration

240ms

Close

Reverse animation.

Drag

Physics based.

No lag.

Resize

Live update.

Snap

Smooth interpolation.

Focus

Subtle elevation.

Inactive

Slightly dim.

---

# 8. Navigation Motion

Sidebar

Slides

220ms

Dock

Magnifies

180ms

Search

Drops from top.

Command Palette

Scales from center.

Breadcrumb

Crossfades.

Navigation should never interrupt workflow.

---

# 9. Workspace Motion

Workspace changes should feel like changing context—not loading a new page.

Old content

↓

Fades

↓

New content

↓

Slides upward

↓

Settles

No hard page refresh.

---

# 10. Scroll System

Engine

Lenis

Characteristics

Smooth

Responsive

Precise

Natural

Rules

No scroll hijacking.

No forced scrolling.

Parallax only when it enhances hierarchy.

---

# 11. Hover Language

Every hover should communicate possibility.

Cards

Lift

Buttons

Brighten

Icons

Rotate 2°

Links

Underline grows.

Technology badges

Accent border.

Workspace cards

Expand slightly.

Maximum Scale

1.02

Never exceed.

---

# 12. Micro Interactions

Buttons

Shrink 2% on press.

Inputs

Glow border on focus.

Checkbox

Smooth check animation.

Toggle

Slide naturally.

Tabs

Animated underline.

Search

Results fade progressively.

Copy Button

Shows "Copied".

Download

Progress animation.

Project Card

Preview image subtly zooms.

Everything feels alive without being distracting.

---

# 13. Loading Choreography

No spinners.

Use

Skeletons.

Progressive reveal.

Images

Fade.

Cards

Cascade.

GitHub

Placeholder.

Projects

Progressive loading.

The user should never feel blocked.

---

# 14. Background Motion

Wallpaper

Extremely slow movement.

Aurora

Drifts gently.

Noise

Static.

No animation.

Particles

None.

Grid

Very subtle parallax.

Background motion should almost disappear.

---

# 15. Sound Synchronization

Window Open

Soft click.

Window Close

Muted tap.

Notification

Tiny pop.

Toggle

Soft switch.

Search

Minimal tick.

Volume

Very low.

Never intrusive.

Can be disabled.

---

# 16. Motion Accessibility

Reduced Motion

Supported.

If enabled

Remove

Parallax.

Cursor interpolation.

Background animation.

Window scaling.

Retain only fade transitions.

Keyboard users receive identical functionality.

---

# 17. Performance Rules

Target

60 FPS minimum.

120 FPS preferred.

Animation budget

<16ms per frame.

GPU accelerated.

Avoid layout thrashing.

Avoid expensive blur.

Avoid unnecessary repaint.

Animations pause when tab loses focus.

---

# 18. Motion Tokens

Hover

120ms

Open

240ms

Close

220ms

Search

180ms

Sidebar

220ms

Workspace

260ms

Dock

180ms

Scale Hover

1.02

Scale Press

0.98

Window Radius

18px

Cursor Size

16px

Cursor Hover

28px

Spring

Low bounce

Primary Ease

easeOutCubic

Secondary Ease

easeInOutCubic

---

# 19. Signature Moments

Every workspace should have one memorable interaction.

Home

Workspace unfolds around "Meet."

Projects

Project expands into a detailed workspace.

AI

Animated AI workflow connects nodes.

Engineering

Technology graph expands dynamically.

Automation

Workflow nodes animate as if processing.

Cybersecurity

Terminal commands type naturally.

GitHub

Contribution graph fades in by week.

Resume

Document opens from the dock into a floating viewer.

Contact

Message card slides into focus.

---

# 20. Motion Anti-Patterns

Never use

✗ Bounce animations

✗ Spinning loaders

✗ Infinite floating objects

✗ Large rotations

✗ Excessive blur

✗ Long animations

✗ Scroll hijacking

✗ Flashing effects

✗ RGB glow

✗ Fake hacker effects

Motion should feel invisible.

Users should notice the product—not the animation.

---

# Motion Manifesto

Motion is one of the defining characteristics of Meet.

The goal is not to impress.

The goal is to make every interaction feel inevitable.

The best animation is one that users don't consciously notice, yet would immediately miss if it were removed.

Meet. should move with the confidence of a mature software product.

Every frame should communicate quality.

Every transition should communicate intention.

Every interaction should communicate craftsmanship.
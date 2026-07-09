# Meet.
# 12_ANIMATION_CHOREOGRAPHY.md

Version: 1.0

Status: Final

Owner: Meet Shah

Target FPS: 60+

---

# Purpose

Motion should feel invisible.

Users should never think

"That animation looks cool."

Instead they should think

"This software feels amazing."

Every animation must reinforce professionalism.

Never entertainment.

---

# Motion Philosophy

Motion explains.

Motion guides.

Motion connects.

Motion never distracts.

Animation should disappear into the experience.

---

# Landing Experience

Duration

1.8 seconds

Sequence

Background fades in

↓

Aurora begins moving slowly

↓

Meet.

appears

↓

Tagline fades upward

↓

Sidebar slides in

↓

Dock rises

↓

Workspace fades

↓

Featured Project cards cascade

↓

Cursor activates

↓

User gains control

No loading spinner.

No fake boot screen.

---

# Hero Animation

Meet.

Opacity

0 → 100

Y Position

24px → 0

Duration

700ms

Ease

easeOutCubic

Tagline

Appears 120ms later.

Workspace

Appears after tagline.

---

# Sidebar

Initial State

Hidden

Animation

Slides

X

-20px → 0

Opacity

0 → 100

Duration

220ms

Delay

100ms

---

# Dock

Animation

Slides upward

Y

20px → 0

Opacity

0 → 100

Duration

220ms

Delay

180ms

Magnification activates only after animation completes.

---

# Workspace Reveal

Workspace

Opacity

0 → 100

Scale

0.99 → 1

Duration

260ms

No bounce.

---

# Project Cards

Cards animate one after another.

Delay

60ms

Sequence

Card

1

↓

2

↓

3

↓

4

Hover

Scale

1.02

Image zoom

1.03

Shadow

Very subtle

---

# Opening Project

Click

↓

Card slightly expands

↓

Background dims

↓

Project Window grows from card

↓

Navigation freezes

↓

Project becomes focused

Everything feels spatial.

Never random.

---

# Closing Project

Reverse animation.

Project shrinks back into originating card.

Scroll position preserved.

---

# Workspace Switch

Current Workspace

↓

Fade

↓

Slide Up

↓

New Workspace

↓

Slide Up

↓

Fade In

Duration

260ms

No page flashes.

---

# Command Palette

Shortcut

CTRL + K

Animation

Scale

0.96 → 1

Opacity

0 → 100

Background blur

None

Backdrop

Dark overlay

Search field auto focused.

---

# Search Results

Appear progressively.

Delay

40ms

Result

1

↓

2

↓

3

↓

4

Maximum

8 visible.

---

# Sidebar Hover

Icon

↓

Accent color

↓

Label fades

↓

Background highlights

Current workspace

Persistent highlight.

---

# Dock Hover

Hovered icon

↓

Moves upward

↓

Magnifies

↓

Label fades in

Adjacent icons

Slight magnification.

Exactly like physical attraction.

---

# Button Animation

Hover

Brightness

+8%

TranslateY

-1px

Press

Scale

0.98

Release

Spring back.

---

# Inputs

Focus

Border

Accent

Label

Slides upward

Cursor

Native

Error

Shake

2px

Only once.

---

# Technology Badge

Hover

Border

Accent

↓

Background

Subtle

↓

Scale

1.02

Click

Highlights every related project.

---

# Skill Graph

Opening

Nodes

Appear

↓

Connections draw

↓

Labels fade

Hover

Connected nodes highlight.

Everything else fades slightly.

---

# GitHub Graph

Weeks fade sequentially.

Recent contributions animate last.

Tooltip

Appears instantly.

---

# AI Workflow

Nodes

Appear

↓

Connections draw

↓

Pulse moves through graph

↓

Output appears

Animation repeats only on first visit.

---

# Automation Canvas

Connection lines animate left to right.

Processing nodes pulse softly.

Hover

Highlights downstream workflow.

---

# Resume

Resume icon clicked

↓

Window expands

↓

PDF slides upward

↓

Toolbar appears

↓

Page loads

Feels like opening a real document.

---

# Contact Form

Fields

Cascade

One after another.

Button

Appears last.

Success

Checkmark animation.

No confetti.

---

# Theme Change

Background

Crossfade

↓

Accent

Interpolates

↓

Components update

↓

Wallpaper transitions

Duration

250ms

No flash.

---

# Wallpaper

Aurora

Moves

2px every second.

Barely noticeable.

Noise

Static.

---

# Cursor

Default

16px

Hover

28px

Inverse blend mode

Dragging

Compress

Click

Ripple

6px

Cursor interpolation

Enabled

Never lag.

---

# Window Drag

Window follows pointer naturally.

Very small easing.

No delay.

Snap previews appear before snapping.

---

# Window Snap

Guides appear.

Release

↓

Window glides

↓

Settles

↓

Focus restored

---

# Loading Skeletons

Fade

↓

Pulse

↓

Content crossfades

Never show spinners.

---

# Empty States

Illustration

↓

Title

↓

Description

↓

Primary Action

Everything fades upward.

---

# Notifications

Slide

Right

↓

Fade

↓

Auto dismiss

3 seconds

Hover pauses timer.

---

# Scrolling

Lenis

Smooth

Natural

Precise

No inertia overload.

Parallax

Maximum

12px

Used only in Hero.

---

# Sound Sync

Open Window

Soft click

Close

Muted tap

Search

Tiny tick

Theme

Soft switch

Toggle

Light click

Sounds disabled by default on first visit.

---

# Mobile Motion

Reduce movement.

Replace

Scale

with

Fade.

Disable

Dock magnification.

Disable

Cursor effects.

Keep interface responsive.

---

# Reduced Motion

Disable

Parallax

Cursor interpolation

Background movement

Scaling

Keep

Fade

Opacity

Essential transitions.

Fully WCAG compliant.

---

# Motion Performance Rules

GPU Accelerated

Transform

Opacity

Never animate

Width

Height

Top

Left

Margin

Use transforms whenever possible.

Maintain 60 FPS minimum.

---

# Signature Moments

1.

Workspace unfolds around "Meet."

2.

Project opens from its card.

3.

Technology graph reveals relationships.

4.

AI workflow draws itself.

5.

Resume opens like a real document.

6.

Dock responds physically.

7.

Cursor inverts over interactive content.

8.

Everything restores exactly where the visitor left.

---

# Motion Manifesto

Motion is part of the storytelling.

Animations should make the interface feel alive without demanding attention.

The visitor should remember the quality of the software—not individual effects.

Every frame should communicate precision.

Every transition should communicate confidence.

Every interaction should reinforce one message:

Meet builds software with intention.
---
App Name: Tasks
version: 1.0.0
description: Tasks is a Flutter productivity app where users can save daily tasks, organize them into categories, create custom lists, set reminders, and run focused work sessions with built-in timers. A soft gradient canvas (light blue → white) anchors glassmorphic cards with 42px radius corners. Primary Dark (#0077B6) carries every interactive element. The bottom navigation is a curved solid primary bar. Typography is Inter at mobile-friendly sizes (14–16px). This is a warm, approachable design language where glassmorphism is the visual signature.

colors:
  primary-dark: "#0077B6"
  primary-light: "#94CCFF"
  primary-container: "#CDE5FF"
  on-primary: "#FFFFFF"
  secondary: "#006875"
  secondary-container: "#9CECFB"
  background: "#F7F9FB"
  surface: "#FFFFFF"
  surface-dim: "#D8DADC"
  surface-container-low: "#F2F4F6"
  surface-container: "#ECEEF0"
  surface-container-high: "#E6E8EA"
  on-surface: "#191C1E"
  on-surface-variant: "#404850"
  outline: "#707881"
  outline-variant: "#BFC7D1"
  gradient-start: "#CAF0F8"
  gradient-end: "#E7FBFF"
  success: "#10B981"
  error: "#EF4444"
  error-container: "#BA1A1A"
  warning: "#F59E0B"
  category-important: "#EAB308"
  category-study: "#8B5CF6"
  category-work: "#2563EB"
  category-home: "#F97316"
  due-teal: "#006875"
  badge-bg: "#E6E8EA"

typography:
  font-family: "Inter, system-ui"
  display-lg:
    fontSize: 40px
    fontWeight: 700
    height: 1.2
    letterSpacing: -0.02
  headline-lg:
    fontSize: 32px
    fontWeight: 600
    height: 1.25
    letterSpacing: -0.01
  headline-md:
    fontSize: 24px
    fontWeight: 600
    height: 1.33
  headline-sm:
    fontSize: 22px
    fontWeight: 700
    height: 1.27
  body-lg:
    fontSize: 18px
    fontWeight: 600
  body-md:
    fontSize: 16px
    fontWeight: 400
    height: 1.5
  body-handwritten:
    fontSize: 14px
    fontWeight: 400
    height: 1.5
    fontFamily: "PatrickHand"
  label-md:
    fontSize: 14px
    fontWeight: 500
    letterSpacing: 0.01
  label-sm:
    fontSize: 12px
    fontWeight: 500
    letterSpacing: 0.02
  auth-title:
    fontSize: 30px
    fontWeight: 600
    height: 1.25
    letterSpacing: -0.01
  button:
    fontSize: 16px
    fontWeight: 600
  link:
    fontSize: 14px
    fontWeight: 700
  body-link:
    fontSize: 14px
    fontWeight: 400
  or-divider:
    fontSize: 12px
    fontWeight: 500
    letterSpacing: 2
  caption:
    fontSize: 11px
    fontWeight: 500
  my-lists-header:
    fontSize: 12px
    fontWeight: 700
    letterSpacing: 1

rounded:
  sm: 12px
  md: 16px
  lg: 20px
  xl: 24px
  xxl: 42px
  pill: 9999px

spacing:
  xs: 4px
  sm: 8px
  md: 12px
  lg: 16px
  xl: 24px
  xxl: 32px
  container-padding: 24px

icon-sizes:
  xs: 16px
  sm: 18px
  md: 20px
  lg: 22px
  xl: 24px
  xxl: 26px
  header: 28px
  fab: 32px
  empty-state: 90px

durations:
  fast: 200ms
  normal: 300ms
  slow: 350ms
  long: 500ms
  very-long: 1000ms
  super-long: 2000ms

components:
  glass-card:
    backgroundColor: "{colors.surface} withAlpha(0.6)"
    borderColor: "{colors.surface} withAlpha(0.3)"
    borderRadius: "{rounded.xxl}"
    shadow: "0 8px 32px rgba(0, 119, 182, 0.10)"
  task-card:
    backgroundColor: "{colors.surface}"
    borderRadius: "{rounded.lg}"
    shadow: "0 4px 20px rgba(0, 119, 182, 0.08)"
  bottom-nav:
    backgroundColor: "{colors.primary-dark}"
    borderRadius: "{rounded.xl}"
    shadow: "0 -4px 20px rgba(0, 119, 182, 0.10)"
    height: 70px
  primary-button:
    backgroundColor: "{colors.primary-dark}"
    textColor: "{colors.on-primary}"
    typography: "{typography.button}"
    borderRadius: "{rounded.lg}"
    height: 52px
    shadow: "0 4px 15px rgba(0, 119, 182, 0.25)"
  google-button:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    typography: "{typography.button}"
    borderRadius: "{rounded.lg}"
    height: 50px
  empty-state:
    shadow: "0 16px 50px rgba(0, 119, 182, 0.28)"
  sort-bar:
    shadow: "0 2px 8px rgba(0, 119, 182, 0.08)"
  sort-dropdown:
    shadow: "0 4px 12px rgba(0, 119, 182, 0.10)"
  sheet:
    borderRadius: "{rounded.xl}"
    maxTextFieldHeight: 120px
  avatar:
    size: 104px
  header:
    height: 48px

---

## Overview

Tasks is a Flutter **productivity app** that helps users manage daily tasks, organize them into categories and custom lists, set smart reminders, and run focused work sessions with live timers. Every design decision serves the goal of **warmth, clarity, and approachability** — this is a glassmorphic design language where soft surfaces and gentle shadows create an inviting experience.

The layout is a mobile-first single-screen structure: a **gradient canvas** (light blue → white, top to bottom) runs behind everything, providing subtle visual warmth. **Glassmorphic cards** with translucent white backgrounds and soft primary-tinted shadows float above the gradient, creating depth without heaviness. A **curved bottom navigation bar** provides access to the main screens: Reminders, Sessions, Home, Settings, and Profile.

**Key Characteristics:**
- Glassmorphic surfaces: translucent white cards (`{colors.surface}` at 60% alpha) with soft primary-tinted shadows create depth and warmth.
- Single accent color (`{colors.primary-dark}` #0077B6) carries every interactive element: button fills, navigation highlights, header text, and link colors.
- Soft gradient canvas (`{colors.gradient-start}` #CAF0F8 → `{colors.gradient-end}` #E7FBFF) provides ambient warmth behind all data surfaces.
- Inter font at mobile-friendly sizes (14–16px body, 32–40px display): clean, modern, and highly legible on mobile screens.
- Curved navigation bar with solid primary color: the universal "app shell" element that anchors every screen.
- Category colors are semantic: yellow = important, purple = study, blue = work, orange = home. These map to list icons, task badges, and category indicators.
- Status colors are semantic: green = completed, red = error/overdue, yellow = warning/pending. These map to task states and notification badges.
- Rounded corners throughout: 20px for cards, 12–16px for buttons, pill radius for badges and tags. The radius system creates softness and approachability.
- Handwritten font (PatrickHand) for motivational quotes and session messages: adds a personal, human touch to the productivity experience.

## Colors

### Primary Palette
- **Primary Dark** (`{colors.primary-dark}`, #0077B6): The primary brand color. All button fills, navigation highlights, header text, link colors, and the gradient's starting tone use this blue. It is the universal "this is actionable" signal.
- **Primary Light** (`{colors.primary-light}`, #94CCFF): A lighter blue for subtle backgrounds, disabled states, and secondary interactive surfaces.
- **Primary Container** (`{colors.primary-container}`, #CDE5FF): A very light blue for card backgrounds, input field fills, and the gradient's midpoint. It is the brand's "resting" surface.
- **On Primary** (`{colors.on-primary}`, #FFFFFF): Text and icons on `{colors.primary-dark}` backgrounds. Used on button labels and active navigation items.

### Secondary
- **Secondary** (`{colors.secondary}`, #006875): A teal accent used for due dates, status indicators, and secondary interactive elements. Distinct from the primary blue but harmonious.
- **Secondary Container** (`{colors.secondary-container}`, #9CECFB): A light teal for subtle backgrounds and secondary card surfaces.

### Surface & Background
- **Background** (`{colors.background}`, #F7F9FB): The scaffold background color, a very light gray-blue that provides subtle warmth.
- **White Surface** (`{colors.surface}`, #FFFFFF): The dominant card surface. All glassmorphic cards, dialogs, and input fields use pure white.
- **Surface Dim** (`{colors.surface-dim}`, #D8DADC): A muted gray for disabled states and subtle borders.
- **Surface Container Low** (`{colors.surface-container-low}`, #F2F4F6): A light gray for secondary card backgrounds and section dividers.
- **Surface Container** (`{colors.surface-container}`, #ECEEF0): A mid-gray for input field backgrounds and disabled surfaces.
- **Surface Container High** (`{colors.surface-container-high}`, #E6E8EA): A darker gray for selected states and active input borders.

### Gradient
- **Gradient Start** (`{colors.gradient-start}`, #CAF0F8): A light cyan-blue at the top of the gradient. The starting point of the vertical gradient.
- **Gradient End** (`{colors.gradient-end}`, #E7FBFF): A near-white at the bottom of the gradient. The terminal point, creating a soft fade into white.

### Text
- **On Surface** (`{colors.on-surface}`, #191C1E): All primary text: task titles, navigation labels, dialog content. Near-black for maximum contrast on white surfaces.
- **On Surface Variant** (`{colors.on-surface-variant}`, #404850): Secondary information: task descriptions, due dates, placeholder text. A dark gray that recedes behind primary text.

### Outline
- **Outline** (`{colors.outline}`, #707881): The 1px border on cards, input fields, and dividers. A medium gray that defines edges without adding visual weight.
- **Outline Variant** (`{colors.outline-variant}`, #BFC7D1): A lighter gray for subtle borders and section dividers.

### Status
- **Success** (`{colors.success}`, #10B981): Completed tasks, active states, positive actions. The universal "healthy" signal.
- **Error** (`{colors.error}`, #EF4444): Failed actions, overdue tasks, destructive operations. The "action required" signal.
- **Error Container** (`{colors.error-container}`, #BA1A1A): A darker red for error backgrounds and destructive action buttons.
- **Warning** (`{colors.warning}`, #F59E0B): Intermediate states, pending actions, caution indicators. The "attention" signal.

### Category Colors
- **Category Important** (`{colors.category-important}`, #EAB308): Yellow for important tasks and priority indicators.
- **Category Study** (`{colors.category-study}`, #8B5CF6): Purple for study-related tasks and lists.
- **Category Work** (`{colors.category-work}`, #2563EB): Blue for work-related tasks and lists.
- **Category Home** (`{colors.category-home}`, #F97316): Orange for home-related tasks and lists.

### Semantic
- **Due Teal** (`{colors.due-teal}`, #006875): Due date text and time-related indicators.
- **Badge Background** (`{colors.badge-bg}`, #E6E8EA): Background for count badges and status indicators.

### Glass / Shadows
- **Glass White** (`{colors.glass-white}`): `{colors.surface}` at 60% alpha. The translucent background for glassmorphic cards.
- **Glass Border** (`{colors.glass-border}`): `{colors.surface}` at 30% alpha. The subtle border for glassmorphic cards.
- **Glass Menu Background** (`{colors.glass-menu-bg}`): `{colors.surface}` at 80% alpha. The background for dropdown menus and popups.

## Typography

### Font Family
- **Primary**: `Inter`: A clean, modern sans-serif font chosen for its excellent legibility on mobile screens and its neutral, professional character.
- **Handwritten**: `PatrickHand`: A casual, handwritten font used exclusively for motivational quotes and session messages. Adds a personal, human touch.

### Hierarchy

| Token | Size | Weight | Line Height | Use |
|---|---|---|---|---|
| `{typography.display-lg}` | 40px | 700 | 1.2 | Welcome messages, splash text |
| `{typography.headline-lg}` | 32px | 600 | 1.25 | Screen titles (primary blue) |
| `{typography.headline-md}` | 24px | 600 | 1.33 | Section headers |
| `{typography.headline-sm}` | 22px | 700 | 1.27 | Sub-section headers (primary blue) |
| `{typography.body-lg}` | 18px | 600 | — | Emphasis text, card titles |
| `{typography.body-md}` | 16px | 400 | 1.5 | Body text, task descriptions |
| `{typography.body-handwritten}` | 14px | 400 | 1.5 | Motivational quotes, session messages |
| `{typography.label-md}` | 14px | 500 | — | Navigation items, form labels |
| `{typography.label-sm}` | 12px | 500 | — | Secondary labels, timestamps |
| `{typography.auth-title}` | 30px | 600 | 1.25 | Login/signup screen titles |
| `{typography.button}` | 16px | 600 | — | Button labels |
| `{typography.link}` | 14px | 700 | — | Hyperlinks (primary blue) |
| `{typography.body-link}` | 14px | 400 | — | Secondary links |
| `{typography.or-divider}` | 12px | 500 | — | "OR" divider text |
| `{typography.caption}` | 11px | 500 | — | Error messages, captions |
| `{typography.my-lists-header}` | 12px | 700 | — | Section headers in My Lists |

### Principles

- **Mobile-first sizing.** Body text is 16px for comfortable reading on mobile. Headlines range from 22–40px for visual hierarchy without overwhelming the screen.
- **Weight 400 for body, 600 for structure.** Body text uses regular weight (400) for readability. Headlines and section headers use semi-bold (600) to create structural hierarchy.
- **Weight 700 reserved for emphasis.** The display text (40px/700), headline-sm (22px/700), and my-lists-header (12px/700) are the only places bold appears at 700. Everything else lives below 700.
- **Line-height is generous for mobile.** At 1.2–1.5, text lines have comfortable spacing for mobile reading. This is a readability-first choice for a productivity app.
- **Handwritten font for personality.** PatrickHand is used sparingly for motivational quotes and session messages, adding warmth without sacrificing professionalism.

## Layout

### Spacing System
- **Base unit:** 4px. All spacing values are multiples of 4px.
- **Tokens:** `{spacing.xs}` 4px · `{spacing.sm}` 8px · `{spacing.md}` 12px · `{spacing.lg}` 16px · `{spacing.xl}` 24px · `{spacing.xxl}` 32px.
- **Container padding:** All screen content uses `{spacing.container-padding}` (24px) horizontal padding.
- **Card padding:** Glassmorphic cards use `{spacing.lg}` (16px) to `{spacing.xl}` (24px) internal padding.
- **Component spacing:** Form fields, buttons, and list items use `{spacing.md}` (12px) to `{spacing.lg}` (16px) gaps.

### Grid & Container
- **Mobile-first layout:** Single-column layout optimized for mobile screens. Content fills the full width with 24px horizontal padding.
- **Bottom navigation:** Fixed curved bar at the bottom with 5 navigation items: Reminders, Sessions, Home, Settings, Profile. The center item (Home) has an elevated FAB-like appearance.
- **Cards:** Glassmorphic cards with translucent white backgrounds, soft primary-tinted shadows, and 20px border radius. Cards float above the gradient canvas.
- **Bottom sheets:** Used for task creation, editing, and selection. 24px border radius, glassmorphic background, max height 120px for text fields.

### Whitespace Philosophy
Tasks' whitespace is **generous and breathing**. The glassmorphic design relies on space and translucency to create depth, not density. Cards have comfortable internal padding (16–24px), and the gradient canvas provides ambient warmth behind all surfaces. The 20px border radius on cards creates soft, rounded corners that reinforce the approachable design language.

## Elevation & Depth

| Level | Treatment | Use |
|---|---|---|
| Flat | No shadow, gradient background | Canvas gradient, scaffold background |
| Glass card | `0 8px 32px rgba(0, 119, 182, 0.10)` shadow, translucent white, 20px radius | Task cards, content cards |
| Task card | `0 4px 20px rgba(0, 119, 182, 0.08)` shadow, white background, 20px radius | Individual task items |
| Bottom nav | `0 -4px 20px rgba(0, 119, 182, 0.10)` shadow, solid primary blue, 24px radius | Curved navigation bar |
| Primary button | `0 4px 15px rgba(0, 119, 182, 0.25)` shadow, primary blue, 20px radius | Primary action buttons |
| Empty state | `0 16px 50px rgba(0, 119, 182, 0.28)` shadow, large circle | Empty state illustrations |

**Shadow philosophy.** Tasks uses **primary-tinted shadows** throughout — every shadow has a blue tint from `{colors.primary-dark}` at low opacity. This creates a cohesive, warm depth system where shadows feel like they belong to the brand, not generic gray overlays.

### Decorative Depth
- **Gradient canvas** provides ambient warmth behind all data surfaces. It is a vertical gradient with two stops, applied to the full scaffold background. The gradient is purely decorative; it adds visual interest without competing with content.
- **Glassmorphic translucency** on cards creates depth through opacity, not shadow. The 60% white background allows the gradient to subtly show through, creating a layered, airy feel.
- **Curved navigation bar** creates a "floating" feel through its pill-shaped radius and upward-facing shadow, distinguishing it from flat bottom bars.

## Shapes

### Border Radius Scale

| Token | Value | Use |
|---|---|---|
| `{rounded.sm}` | 12px | Small buttons, chips, tags |
| `{rounded.md}` | 16px | Medium buttons, input fields |
| `{rounded.lg}` | 20px | Cards, task items, primary buttons — the universal card radius |
| `{rounded.xl}` | 24px | Bottom navigation bar, bottom sheets |
| `{rounded.xxl}` | 42px | Large containers, special elements |
| `{rounded.pill}` | 9999px | Badges, status indicators, toggle buttons — the universal "interactive" radius |

### Radius Philosophy
Tasks uses a **progressive radius system**: smaller elements get smaller radii (12–16px), while larger containers get larger radii (20–24px). The pill radius (9999px) is reserved for badges and fully rounded interactive elements. This creates visual hierarchy through shape: you can intuit the element's importance from its corner radius.

## Components

### Glass Card

**`glass-card`**: The foundational UI component. A translucent white card (`{colors.surface}` at 60% alpha) with a subtle border (`{colors.surface}` at 30% alpha), 42px border radius (`{rounded.xxl}`), and a soft primary-tinted shadow (`0 8px 32px rgba(0, 119, 182, 0.10)`). Used for task lists, content sections, and any surface that needs to "float" above the gradient canvas.

### Task Card

**`task-card`**: A white elevated card for individual task items. Background `{colors.surface}` (white), 20px border radius, shadow `0 4px 20px rgba(0, 119, 182, 0.08)`. Contains: task title (`{typography.body-lg}`), due date/time (`{typography.label-sm}` in `{colors.due-teal}`), category badge (`{typography.label-sm}` with category color), and importance indicator. Toggle-able completion state with smooth animation.

### Bottom Navigation Bar

**`bottom-nav`**: A curved navigation bar fixed at the bottom of every screen. Background `{colors.primary-dark}` (solid primary blue), transparent scaffold background, shadow `0 -4px 20px rgba(0, 119, 182, 0.10)`. Height 70px. Contains 5 navigation items: Reminders, Sessions, Home, Settings, Profile. The center item (Home) has an elevated, pill-shaped highlight. Active item gets `{colors.on-primary}` (white) icon.

### Primary Button

**`primary-button`**: Pill-shaped action button for primary actions. Background `{colors.primary-dark}` (#0077B6), text `{colors.on-primary}` (white), typography `{typography.button}` (16px / 600), border radius `{rounded.lg}` (20px), height 52px. Shadow `0 4px 15px rgba(0, 119, 182, 0.25)`. Used for "Create Account", "Login", "Save Task", and other primary actions.

### Google Sign-In Button

**`google-button`**: A white elevated button for Google authentication. Background `{colors.surface}` (white), text `{colors.on-surface}`, typography `{typography.button}` (16px / 600), border radius `{rounded.lg}` (20px), height 50px. Contains Google logo icon and "Sign in with Google" text.

### Empty State

**`empty-state`**: A large circular illustration shown when a screen has no content. Uses `{typography.headline-md}` for the title, `{typography.body-md}` for the description. Shadow `0 16px 50px rgba(0, 119, 182, 0.28)` creates a floating effect. Icon size 90px (`{icon-sizes.empty-state}`).

### Sort Bar

**`sort-bar`**: A horizontal bar for sorting and filtering task lists. Shadow `0 2px 8px rgba(0, 119, 182, 0.08)`. Contains sort dropdown, filter chips, and view toggle. Background `{colors.surface}` with glassmorphic effect.

### Sort Dropdown

**`sort-dropdown`**: A dropdown menu for sort options. Shadow `0 4px 12px rgba(0, 119, 182, 0.10)`. Background `{colors.surface}`, border radius `{rounded.lg}` (20px). Typography `{typography.label-md}` (14px / 500).

### Bottom Sheet

**`sheet`**: A modal bottom sheet for task creation, editing, and selection. Border radius `{rounded.xl}` (24px), glassmorphic background. Contains form fields with max height 120px for multiline input. Slide-up animation with fade.

### Avatar

**`avatar`**: A circular profile image. Size 104px (`{icon-sizes.avatar}`). Used in the profile screen and profile edit flow. Multiple avatar options available in the assets folder.

### Header

**`header`**: A fixed-height header bar at the top of screens. Height 48px (`{icon-sizes.header}`). Contains screen title (`{typography.headline-lg}` in `{colors.primary-dark}`), optional back button, and optional action buttons.

### Status Badge

**`status-badge`**: A pill-shaped badge with a colored background and label. Border radius `{rounded.pill}`, typography `{typography.label-sm}` (12px / 500). States: green background + "Completed" (`{colors.success}`), yellow background + "Pending" (`{colors.warning}`), red background + "Overdue" (`{colors.error}`), teal background + due date (`{colors.due-teal}`).

### Category Badge

**`category-badge`**: A pill-shaped badge for task categories. Border radius `{rounded.pill}`, typography `{typography.label-sm}` (12px / 500). Colors: yellow (`{colors.category-important}`), purple (`{colors.category-study}`), blue (`{colors.category-work}`), orange (`{colors.category-home}`).

### Session Timer

**`session-timer`**: A large circular countdown timer displayed during active sessions. Uses `{typography.display-lg}` (40px / 700) for the countdown digits. Background `{colors.primary-container}` with a progress ring in `{colors.primary-dark}`. The center displays the current task name and time remaining. The pause/resume button has no hover or active visual states — it is a simple tap-only control with no color change, scale animation, or ripple effect.

### Form Field

**`form-field`**: A text input field with two states:

| State | Border | Background | Message |
|---|---|---|---|
| Neutral | 1px `{colors.outline}` | `{colors.surface}` (white) | None |
| Error | 1px `{colors.error}` | `{colors.surface}` (white) | Red caption below: `{typography.caption}` (11px / 500, `{colors.error}`) |

Height 52px (`{AppComponentSizes.buttonHeight}`), border radius `{rounded.lg}` (20px), typography `{typography.body-md}` (16px / 400). No warning icon. No background change on error — only the border and caption text change.

### Category Picker

**`category-picker`**: A grid of icon + color options shown in the list creation/editing bottom sheet. Users pick an icon and a color to personalize their custom list.

- **Grid layout:** 2 rows — first row for icons, second row for colors. Horizontal scrolling if items overflow.
- **Icon items:** 40px circular containers, border radius `{rounded.pill}`. Each contains a Material/FontAwesome icon at 20px (`{icon-sizes.md}`). Background `{colors.surface-container}`. Selected icon gets `{colors.primary-dark}` border ring (2px) and `{colors.primary-container}` background.
- **Color items:** 32px circular swatches, border radius `{rounded.pill}`. Each is a solid fill of the category color. Selected color gets a 2px `{colors.primary-dark}` border ring and a subtle checkmark overlay.
- **Spacing:** 12px gap between items (`{spacing.md}`).
- **Note:** This picker is for list creation only. Tasks do not have their own icon/color — they inherit the list they belong to.

### Avatar Picker

**`avatar-picker`**: A scrollable grid of circular avatar images shown in the profile edit screen. Users tap an avatar to select it for their profile.

- **Container:** GlassCard with `{spacing.lg}` (16px) internal padding. Fixed height of 156px, scrolls vertically with `BouncingScrollPhysics` when more than 2 rows exist.
- **Grid:** 3 columns, 12px spacing between items (`{spacing.md}`). Row height is 72px (avatar diameter).
- **Avatar circle:** 36px radius (72px diameter), background `{colors.surface-container-low}` (#F2F4F6). Image loaded from `assets/Avatars/` via `AssetImage`.
- **Selected state:** 3px `{colors.primary-dark}` border ring with 3px internal padding to prevent the image from overlapping the border. No checkmark, no scale animation.
- **Unselected state:** No border, no padding.
- **Avatar sets:** Male set (6 avatars), female set (11 avatars). Grid shows one set based on the user's stored avatar path (contains "male" or "female"). Default avatar (`assets/user_profile_default_image.jpg`) is shown as the current preview but is not in the selectable grid.

## Do's and Don'ts

### Do
- Use `{colors.primary-dark}` (#0077B6) for every interactive element: buttons, nav highlights, links, header text, and nothing else. The single accent is non-negotiable.
- Use glassmorphic effects (translucent white + primary-tinted shadows) for all card surfaces. The glassmorphism is the visual signature.
- Use `{rounded.lg}` (20px) for cards and `{rounded.pill}` for badges and tags. The radius system creates visual hierarchy.
- Use category colors semantically: yellow = important, purple = study, blue = work, orange = home. Never use these colors for decorative purposes.
- Show the gradient canvas behind all content surfaces. The light blue → white vertical gradient is the ambient warmth that keeps the app from feeling sterile.
- Use `{typography.body-handwritten}` (PatrickHand) for motivational quotes and session messages: it adds a personal, human touch.
- Use status colors semantically: green = completed, red = error/overdue, yellow = warning/pending. Never use these colors for decorative purposes.
- Use primary-tinted shadows (`rgba(0, 119, 182, ...)`) for all elevation. Shadows should feel brand-cohesive, not generic gray.

### Don't
- Don't introduce a second accent color. Every interactive signal is `{colors.primary-dark}` (#0077B6). Status and category colors are semantic, not decorative.
- Don't use flat, opaque card backgrounds without the glassmorphic translucency. The translucency is essential to the design language.
- Don't add shadows to the gradient canvas, status badges, or category badges. Shadow is reserved for cards, buttons, and the navigation bar only.
- Don't use italic, underline, or letter-spacing for emphasis. Emphasis comes from weight (400 → 600 → 700) and color (primary → secondary → muted).
- Don't use status colors (green/yellow/red) for anything other than their semantic meaning. Green is completed, red is error, yellow is warning; never use green for "decorative" or red for "important."
- Don't make the bottom navigation bar taller than 70px or its text larger than 14px. The bar is a compact navigation element, not a full panel.
- Don't add decorative gradients to cards, buttons, or text. The only gradient is the canvas background. Everything else is flat white or flat colored.

## Responsive Behavior

### Breakpoints

| Name | Width | Key Changes |
|---|---|---|
| Small | ≤ 360px | Compact layout, reduced padding, smaller text |
| Standard | 361–600px | Full mobile layout, standard padding and spacing |
| Large | 601px+ | Tablet-optimized layout with wider cards and more whitespace |

### Collapsing Strategy
- **Bottom navigation:** Fixed at the bottom across all widths. Items may collapse to icons only on very small screens.
- **Cards:** Full-width with 24px horizontal padding on mobile. Max-width containers on larger screens.
- **Bottom sheets:** Full-width on mobile. Centered with max-width on tablets.
- **Form fields:** Full-width on all screen sizes. Max-width containers on tablets.

### Minimum Screen Size
- **320 × 480px**. Below this size, the UI elements become too cramped for comfortable use. The app is designed for modern mobile devices.

### Touch Targets
- All interactive elements meet the minimum 44 × 44px touch target recommended by Material Design guidelines.
- Bottom navigation items: 48 × 48px touch area.
- Task cards: Full-width, 48px minimum height.
- Primary buttons: 52px height, full-width within padding.

## Iteration Guide

1. Focus on ONE component at a time. Reference its YAML key directly (`{component.glass-card}`, `{component.task-card}`).
2. Use `{token.refs}` everywhere; never inline hex values.
3. The glassmorphism system (translucent white + primary-tinted shadows) is non-negotiable. Do not use flat, opaque cards.
4. Category colors are semantic only. Yellow = important, purple = study, blue = work, orange = home. Never use them decoratively.
5. Status colors are semantic only. Green = completed, red = error, yellow = warning. Never use them decoratively.
6. The gradient canvas is the only decorative element. Everything else is functional.
7. When in doubt about emphasis: change weight (400 → 600 → 700) or color (primary → secondary → muted) before adding chrome.

## Known Gaps

- **Notification appearance is partially controlled.** The app chooses `NotificationLayout.MediaPlayer` for the session timer (with custom drawable action buttons and a progress bar) and `NotificationLayout.Default` for session completion and all reminders. Accent colors are set per type: `primaryDark` for timer and reminders, `success` for session complete, `error` for missed tasks. What is not controlled is the system notification tray's overall theme (background color, font, icon placement), which follows the device/OS defaults.

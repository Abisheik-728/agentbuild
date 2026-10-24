---
name: AgentBuild
colors:
  surface: '#f8f9ff'
  surface-dim: '#cbdbf5'
  surface-bright: '#f8f9ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#eff4ff'
  surface-container: '#e5eeff'
  surface-container-high: '#dce9ff'
  surface-container-highest: '#d3e4fe'
  on-surface: '#0b1c30'
  on-surface-variant: '#464555'
  inverse-surface: '#213145'
  inverse-on-surface: '#eaf1ff'
  outline: '#777587'
  outline-variant: '#c7c4d8'
  surface-tint: '#4d44e3'
  primary: '#3525cd'
  on-primary: '#ffffff'
  primary-container: '#4f46e5'
  on-primary-container: '#dad7ff'
  inverse-primary: '#c3c0ff'
  secondary: '#565e74'
  on-secondary: '#ffffff'
  secondary-container: '#dae2fd'
  on-secondary-container: '#5c647a'
  tertiary: '#005338'
  on-tertiary: '#ffffff'
  tertiary-container: '#006e4b'
  on-tertiary-container: '#67f4b7'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#e2dfff'
  primary-fixed-dim: '#c3c0ff'
  on-primary-fixed: '#0f0069'
  on-primary-fixed-variant: '#3323cc'
  secondary-fixed: '#dae2fd'
  secondary-fixed-dim: '#bec6e0'
  on-secondary-fixed: '#131b2e'
  on-secondary-fixed-variant: '#3f465c'
  tertiary-fixed: '#6ffbbe'
  tertiary-fixed-dim: '#4edea3'
  on-tertiary-fixed: '#002113'
  on-tertiary-fixed-variant: '#005236'
  background: '#f8f9ff'
  on-background: '#0b1c30'
  surface-variant: '#d3e4fe'
typography:
  display:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
    letterSpacing: -0.015em
  headline-sm:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '600'
    lineHeight: 26px
    letterSpacing: -0.01em
  body-lg:
    fontFamily: Inter
    fontSize: 15px
    fontWeight: '400'
    lineHeight: 24px
    letterSpacing: -0.005em
  body-md:
    fontFamily: Inter
    fontSize: 13px
    fontWeight: '400'
    lineHeight: 20px
    letterSpacing: 0em
  body-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '400'
    lineHeight: 18px
    letterSpacing: 0em
  label-md:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
    letterSpacing: 0.01em
  label-sm:
    fontFamily: Inter
    fontSize: 11px
    fontWeight: '600'
    lineHeight: 14px
    letterSpacing: 0.02em
  code-inline:
    fontFamily: monospace
    fontSize: 12px
    fontWeight: '400'
    lineHeight: 18px
    letterSpacing: 0em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  gutter: 1rem
  gutter-compact: 0.5rem
  margin: 1.5rem
  margin-mobile: 1rem
  space-xs: 0.25rem
  space-sm: 0.5rem
  space-md: 0.75rem
  space-lg: 1rem
  space-xl: 1.5rem
---

## Brand & Style

This design system delivers a high-trust, engineering-grade workspace for orchestrating, debugging, and inspecting autonomous agent pipelines. Inspired by the quiet precision of Linear, Vercel, and Raycast, the aesthetic combines minimalist clarity with dense utility. The visual environment minimizes cognitive friction through calm neutral canvases, razor-sharp typography, and surgical touches of electric indigo to denote interactive state and focus.

Targeting software engineers, AI system architects, and technical operators, the interface evokes calm control, absolute determinism, and rapid execution. Visual noise, decorative gradients, and frivolous motion are eliminated in favor of predictable spatial rhythm, high legibility, and functional density. Every surface layer is strictly bounded, establishing immediate visual trust for mission-critical tooling.

## Colors

The palette is engineered around an ultra-crisp, light-mode developer workspace. High-contrast slate neutrals anchor structural elements, while deliberate accent colors indicate execution states without sensory overload.

- **Primary (`#4F46E5`)**: Deep Indigo. Reserved strictly for primary action drivers, active pipeline selection, focused interactive rings, and key state badges.
- **Secondary (`#0F172A`)**: Deep Slate/Charcoal. Powers dominant headings, structural interface anchors, and high-emphasis controls.
- **Tertiary / Semantic Success (`#10B981`)**: Emerald. Designates healthy runtime connections, active daemon status, valid prompt runs, and passing unit assertions.
- **Semantic Warning (`#F59E0B`)**: Amber. Used for non-blocking tool timeouts, truncated contexts, and missing parameter warnings.
- **Semantic Error (`#F43F5E`)**: Rose. Flags failed tool calls, rejected schema validations, and execution interruptions.
- **Neutral Canvas & Surfaces**:
  - Global Canvas: `#F8FAFC`
  - Elevated Cards & Panes: `#FFFFFF`
  - Subtle Dividing Borders: `#E2E8F0`
  - Secondary Inset Fills: `#F1F5F9`
- **Text Palette**:
  - Primary text: `#0F172A`
  - Secondary / Supporting text: `#475569`
  - Muted / Placeholder text: `#94A3B8`

## Typography

The typographic hierarchy relies entirely on `Inter`, taking advantage of its geometric clarity and micro-legibility at compact sizes. A fallback system monospace handles code tokens, payload traces, and runtime schema trees.

- **Weight Discipline**: Headings favor medium-to-semibold weights (`500` and `600`) over heavy bolds to maintain a technical, clean profile. Body content stays on regular (`400`).
- **Tracking**: Slight negative tracking (`-0.01em` to `-0.02em`) is applied to headers larger than `18px` to maintain visual coherence across dense panels.
- **Monospace Elements**: Inline tool names, JSON parameter arguments, latency counters, and token tallies render in standard system monospace (`12px` / `18px` line-height) set against soft background fills.

## Layout & Spacing

This design system uses a strict multi-pane modular desktop shell paired with an internal 12-column grid within canvas zones. The layout balances dense data exploration with generous reading space inside execution streams.

- **Workspace Shell Architecture**:
  - Global Navigation Rail: Fixed `56px` or collapsible `240px` sidebar.
  - Primary Workspace Area: Fluid center canvas hosting agent threads and configuration nodes.
  - Inspector / Telemetry Drawer: Collapsible `360px` right-hand sheet for logs, tool invocations, and token metrics.
- **Rhythm & Padding**:
  - Micro components (tags, pill buttons, badges) use `space-xs` (4px) and `space-sm` (8px).
  - Component internals (cards, input blocks, tool inspection cards) use `space-md` (12px) and `space-lg` (16px).
  - Macro structural separation (grid modules, flow steps) uses `space-xl` (24px).
- **Responsive Adaptations**:
  - On viewports below `1024px`, the inspector panel converts to a sliding drawer over the main thread.
  - On viewports below `768px`, panels stack into a single-column flow with navigation shifting to a top bar.

## Elevation & Depth

Visual hierarchy is established primarily through tonal layering and low-contrast perimeter lines rather than heavy drop shadows.

- **Surface Tiers**:
  - **Base Canvas (Level 0)**: `#F8FAFC`. The foundational backdrop for the entire workspace.
  - **Panels & Workspace Cards (Level 1)**: Pure white `#FFFFFF` bounded by a crisp 1px border (`#E2E8F0`). Elevated by an ambient micro-shadow: `0 1px 2px 0 rgba(15, 23, 42, 0.04)`.
  - **Active Tool Invocations & Interactive Cards (Level 2)**: Pure white `#FFFFFF` with border `#CBD5E1` and lift shadow: `0 4px 6px -1px rgba(15, 23, 42, 0.06), 0 2px 4px -2px rgba(15, 23, 42, 0.04)`.
  - **Command Palettes & Modals (Level 3)**: Pure white `#FFFFFF` layered over a 40% alpha dark backdrop (`rgba(15, 23, 42, 0.4)`), bounded by `0 20px 25px -5px rgba(15, 23, 42, 0.1), 0 8px 10px -6px rgba(15, 23, 42, 0.05)`.
- **Focus Rings**:
  - All focused states utilize a clean 2px offset ring in primary indigo (`#4F46E5`) with zero blur, guaranteeing accessibility while preserving architectural sharpness.

## Shapes

The design system standardizes on a medium curvature (scale `2`). UI primitives use `0.5rem` (8px) border radiuses for standard components, expanding to `1rem` (16px) for major structural cards and contextual drawers.

- **Standard Elements (0.5rem / 8px)**: Buttons, text fields, menu popovers, inline status badges, tool argument blocks.
- **Cards & Surfaces (1rem / 16px)**: Agent prompt builders, message bubbles, log terminal wrappers, execution panels.
- **Micro Tokens (0.25rem / 4px)**: Monospace payload tags, keyboard shortcut hints (`KBD`), parameter pill identifiers.
- **Pill / Circular (`9999px`)**: User avatars, active connection status indicators, and notification count pips.

## Components

### Buttons
- **Primary**: Solid `#4F46E5` fill with white `#FFFFFF` text. Micro-transition (150ms ease) shifting to `#4338CA` on hover. Padding `8px 14px`, text `label-md`.
- **Secondary**: `#FFFFFF` background with 1px border (`#E2E8F0`), `#0F172A` text. Hover shifts to `#F8FAFC` background and `#CBD5E1` border.
- **Ghost**: Transparent background with `#475569` text. Hover shifts to `#F1F5F9` background and `#0F172A` text. Used extensively for panel collapse, copy buttons, and inline menu triggers.

### Inputs & Prompt Editor
- **Fields**: Background `#FFFFFF`, 1px border (`#CBD5E1`), radius `8px`. Focus state triggers an immediate `#4F46E5` border and 2px Indigo ring offset.
- **Agent Prompt Box**: Expansive multi-line textarea with embedded action bar (attachment tokens, model selector, tool toggles, submit trigger). Background `#FFFFFF`, border `#E2E8F0`, subtle shadow.

### Tool Invocation Cards
- Embedded inline within agent conversation streams.
- Card wrapper has a 1px border (`#E2E8F0`), background `#FFFFFF`, and rounded corners (`12px`).
- Collapsible header shows tool name in monospace, status indicator (e.g., spinning indigo icon for executing, green check for resolved), and duration badge.
- Inner payload body uses a muted background (`#F8FAFC`) with formatted JSON parameters and responses.

### Chips & Status Badges
- **Status Indicator**: Neutral pill with a colored 6px dot.
  - Active: `#10B981` dot with `#ECFDF5` background and `#A7F3D0` border.
  - Executing: `#4F46E5` pulsing dot with `#EEF2FF` background and `#C7D2FE` border.
  - Degraded / Warning: `#F59E0B` dot with `#FFFBEB` background and `#FDE68A` border.
  - Error: `#F43F5E` dot with `#FFF1F2` background and `#FECDD3` border.

### Checkboxes & Radios
- Size `16px x 16px`. Checkbox has a `4px` border radius; radio is fully circular.
- Border `#CBD5E1` on neutral state. Checked state fills with `#4F46E5` with a white checkmark or center pip.

### Lists & Activity Feeds
- Compact vertical rows separated by hairline dividers (`#F1F5F9`).
- Hover state lights up row with `#F8FAFC` with an instantaneous cursor cue.
- Left-aligned metadata (timestamp, agent role) set in muted text (`body-sm`), primary event text in `body-md`.
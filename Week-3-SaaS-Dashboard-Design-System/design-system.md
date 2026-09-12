# Week 3 — SaaS Dashboard Design System

## Product concept
**PulseBoard** — a responsive SaaS analytics dashboard for teams to monitor revenue, activation, retention, and operational health.

## Foundations
- Grid: 8px base spacing system; desktop content grid uses 12 columns.
- Border radius: 6px controls, 10px cards, 14px modals.
- Elevation: subtle border-first surfaces; shadows reserved for menus and modals.
- Minimum touch target: 44×44px.

## Color tokens
| Token | Hex | Usage |
|---|---|---|
| Primary | #4F46E5 | Primary actions, active navigation |
| Primary Hover | #4338CA | Hover/pressed state |
| Text | #111827 | Headings and primary text |
| Muted | #6B7280 | Secondary text |
| Background | #F8FAFC | Application background |
| Surface | #FFFFFF | Cards and panels |
| Border | #E5E7EB | Dividers and controls |
| Success | #16A34A | Positive status |
| Warning | #D97706 | Attention states |
| Danger | #DC2626 | Errors/destructive actions |
| Info | #0284C7 | Informational states |

## Typography
Font: Inter.
- Display: 28/36 Bold
- H1: 24/32 Bold
- H2: 20/28 SemiBold
- H3: 16/24 SemiBold
- Body: 14/20 Regular
- Small: 12/16 Regular
- Label/Button: 14/20 SemiBold

## Components
### Buttons
Primary, secondary, ghost, danger, icon-only; default height 40px; disabled state uses reduced emphasis.

### Forms
Text input, select, date picker, search, checkbox, radio, toggle, validation/help text. Labels remain visible and errors are paired with text, not color alone.

### Tables
Sticky header, sortable columns, row hover, selection checkbox, status badge, pagination, empty and loading states.

### Charts
Line, bar, area, donut and KPI cards. Always provide labels/legends and meaningful empty/loading states.

### Navigation
Left sidebar with workspace switcher, primary navigation, secondary settings area and user profile. Collapses to icon rail on smaller widths.

### Modals
Confirmation, form, destructive-action and informational variants. Use backdrop, clear title, supporting copy and explicit primary/secondary actions.

## State model
Every interactive component has default, hover, focus, pressed, disabled, loading and error/success states where applicable.

## Accessibility
Keyboard focus is visible; interactive targets are at least 44×44px; text contrast is designed for readability; status uses text/icons in addition to color; charts have supporting labels.

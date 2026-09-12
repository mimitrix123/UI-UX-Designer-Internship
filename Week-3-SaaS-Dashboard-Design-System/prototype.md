# 5-Screen Interactive Prototype Specification

## Prototype flow
Dashboard → Analytics → Customers → Reports → Settings

### Screen 1 — Dashboard
- KPI cards: Revenue, Active Users, Conversion, Churn.
- Revenue trend chart.
- Recent activity table.
- Sidebar navigation.
- Interaction: clicking Analytics uses a 250ms ease-out horizontal slide.

### Screen 2 — Analytics
- Date-range filter.
- Revenue/activation trend chart.
- Segment filter.
- Interaction: filter changes use 200ms fade/scale for chart refresh; back navigation slides right.

### Screen 3 — Customers
- Search, status filter, customer table and pagination.
- Interaction: opening a customer detail modal uses 180ms fade + 8px upward motion; closing reverses it.

### Screen 4 — Reports
- Report cards, schedule/export controls and report table.
- Interaction: selecting a report opens a modal with 200ms scale from 96% to 100%; successful export shows a toast sliding down from the top.

### Screen 5 — Settings
- Profile, notifications, workspace and security sections.
- Toggle controls and save button.
- Interaction: toggles use 150ms thumb movement; Save shows a 1.5s success toast, then fades.

## Transition rules
- Standard navigation: 250ms ease-out.
- Modal open/close: 180–200ms ease-out.
- Toast: 200ms enter, 150ms exit.
- Hover: 120ms.
- Reduced-motion alternative: instant transitions and no decorative movement.

## Figma prototype setup
Create five 1440×900 desktop frames, connect matching navigation hotspots, then assign the interaction timings above in Prototype mode. Use Smart Animate only where element positions/states visibly transform; use Instant for reduced-motion variants.

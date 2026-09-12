# High-Fidelity Prototype Specification

## Prototype goal
Demonstrate the fastest and most important coordination loop rather than prototype every edge case.

## Flow 1 — Medication completion
`Home → Add medication → Medication detail → Today → Complete task → Home`
- Home quick action opens Add medication.
- Save uses a 180ms ease-out transition to Medication detail.
- Back returns to the originating context.
- Complete uses a check animation and updates the Today card.
- Home shows the updated completion count.

## Flow 2 — Appointment confirmation
`Home → Calendar → Appointment detail → Confirm`
- Calendar tab transitions with a 200ms slide/fade.
- Confirm changes button state to confirmed and shows a compact toast.

## Flow 3 — Shared task assignment
`Home → Shared → Add task → Assign → Confirmation`
- Assignment uses a bottom sheet.
- Save closes the sheet and inserts the task at the top of the selected person's list.

## Motion tokens
- Navigation: 250ms ease-out
- Bottom sheet: 220ms ease-out
- Dialog: 180ms ease-out
- Toast: 180ms in / 140ms out
- Micro-interaction: 120–160ms
- Reduced motion: instant state changes

## Prototype presentation
Use 390 × 844 frames, device preview, realistic sample data, and clickable hotspots. Show the three flows as separate prototype paths in Figma.

**Title:** Verify **Accessibility** compliance in Add to Dashboard modal.

---

**Preconditions:**
- Multiple dashboards exist in the system
- Screen reader software is available (NVDA, JAWS, or VoiceOver)
- Browser supports keyboard navigation and accessibility features

---

**Test Steps:**
1. Login to the **Workspace** as **authenticated user**.
2. Navigate to Reporting page and open any report details.
3. Press the `Tab` key repeatedly to navigate to the Actions button.
4. Press `Enter` to open the Actions dropdown.
5. Use `Arrow Down` key to navigate to "Add to Dashboard" menu item.
6. Press `Enter` to open the Add to Dashboard modal.
7. Verify focus is trapped within the modal (Tab doesn't escape).
8. Press `Tab` to navigate through all interactive elements in order:
   1. Close button (X)
   2. Search textbox
   3. Dashboard checkboxes (each one)
   4. Cancel button
   5. Add to Dashboard button
9. Press `Shift + Tab` to navigate backward through the elements.
10. Use `Space` key to select/deselect dashboard checkboxes.
11. Enable **screen reader** and verify content is properly announced.
12. Test with **high contrast mode** enabled.
13. Test at **200% zoom level** for readability.
14. Press `Escape` key to close modal and verify focus returns to Actions button.

---

**Expected Result:**
- Each `Tab` key press moves focus in logical order through all interactive elements
- `Shift + Tab` navigates in reverse order correctly
- Modal traps focus and doesn't allow Tab to escape to background elements
- `Space` key selects/deselects checkboxes properly
- `Enter` key activates buttons correctly
- **Screen reader** properly announces:
  - Modal title "Add to Dashboard"
  - Search textbox with placeholder
  - Each dashboard name and checkbox state
  - Button states and text changes
- **ARIA compliance**: Proper labels, roles, and semantic markup
- **Visual accessibility**: WCAG AA color contrast ratios (4.5:1 text, 3:1 graphics)
- **Focus indicators**: Clear visual focus indicators on all interactive elements
- **High contrast mode**: All elements remain visible and usable
- **Zoom accessibility**: Modal remains usable and readable at 200% zoom
- `Escape` key closes modal and returns focus to triggering element
- No accessibility violations when tested with automated tools
**Title:** Verify **Accessibility** compliance in Unsaved Changes dropdown functionality

---

**Preconditions:**
- At least one report exists with modified configuration
- Screen reader software is available (NVDA, JAWS, or VoiceOver)
- Browser supports keyboard navigation and accessibility features

---

**Test Steps:**
1. Login to the **Workspace** as **authenticated user**.
2. Navigate to the Reporting page and select a report.
3. Modify the report configuration (e.g., changing report type, axis, or dataset).
4. Click "Show Results" to trigger the "Unsaved Changes" button in the top-right corner.
5. Press the `Tab` key repeatedly to navigate to the "Unsaved Changes" button.
6. Press `Shift + Tab` to navigate backward through the elements.
7. Press `Enter` and `Space` on the "Unsaved Changes" button to verify activation behavior.
8. Enable **screen reader** and verify the button and menu options are properly announced.
9. Use browser **developer tools** to inspect ARIA labels and semantic markup for the dropdown.
10. Test **color contrast** ratios for the "Unsaved Changes" button and modal elements.
11. Test the interface at **200% zoom level** for readability.
12. Switch to **mobile view** and verify touch target sizing for the button.
13. Test with **high contrast mode** enabled to ensure visibility.
14. Navigate away to trigger the warning modal and test modal accessibility.
15. Verify keyboard navigation within the modal using `Tab`, `Enter`, and `Escape` keys.

---

**Expected Result:**
- Each `Tab` key press moves focus in a logical order including the "Unsaved Changes" button in the top-right corner.
- `Shift + Tab` navigates in reverse order correctly.
- "Unsaved Changes" button can be activated with both `Enter` and `Space` keys.
- **Screen reader** properly announces "Unsaved Changes" button state and modal content.
- **ARIA compliance**: Proper labels, roles, and semantic markup for button, dropdown, and modal.
- **Visual accessibility**: WCAG AA color contrast ratios (4.5:1 text, 3:1 graphics) for all states.
- **Mobile accessibility**: Touch targets meet 44x44 pixel minimum for the button.
- **Focus management**: Clear focus indicators and logical navigation through all interactive elements.
- Warning modal is keyboard accessible with proper focus trapping and announcements.
- Modal buttons "Continue Editing" and "Discard Changes" are keyboard accessible.
- No accessibility violations when tested with automated tools.
**Title:** Verify **Accessibility** compliance in Save changes button functionality

---

**Preconditions:**
- At least one non-system-generated report exists in the report list with unsaved configuration changes
- Screen reader software is available (NVDA, JAWS, or VoiceOver)
- Browser supports keyboard navigation and accessibility features

---

**Test Steps:**
1. Login to the **Workspace** as **authenticated user**.
2. Navigate to the Reporting page and select a non-system-generated report.
3. Make configuration changes to trigger the "Save changes" button appearance.
4. Press the `Tab` key repeatedly to navigate through all interactive elements in the sidebar.
5. Press `Shift + Tab` to navigate backward through the elements.
6. Press `Enter` and `Space` on the "Save changes" button to verify activation behavior.
7. Enable **screen reader** and verify the "Save changes" button content is properly announced.
8. Use browser **developer tools** to inspect ARIA labels and semantic markup on the save button.
9. Test **color contrast** ratios for the "Save changes" button text and background.
10. Test the save button area at **200% zoom level** for readability.
11. Switch to **mobile view** and verify touch target sizing for the save button.
12. Test with **high contrast mode** enabled to ensure button visibility.
13. Click "Show Results" and verify the "Unsaved Changes" dropdown accessibility in the header.
14. Navigate to the header dropdown using keyboard navigation and verify accessibility.

---

**Expected Result:**
- Each `Tab` key press moves focus in a logical order:
    1. Report type radio buttons
    2. Data category dropdown
    3. Time frame button
    4. X-axis dropdown
    5. Y-axis dropdown
    6. Add Dataset button
    7. Add Filter button
    8. Save changes button
    9. Show Results button
- `Shift + Tab` navigates in reverse order correctly.
- "Save changes" button can be activated with both `Enter` and `Space` keys.
- **Screen reader** properly announces "Save changes" button and its current state (enabled/disabled/loading).
- **ARIA compliance**: Proper labels, roles, and semantic markup for the save button and related elements.
- **Visual accessibility**: WCAG AA color contrast ratios (4.5:1 text, 3:1 graphics) for all save button states.
- **Mobile accessibility**: Touch targets meet 44x44 pixel minimum for the save button.
- **Focus management**: Clear focus indicators and logical navigation through save-related controls.
- "Unsaved Changes" dropdown in header is keyboard accessible and properly announced by screen readers.
- No accessibility violations when tested with automated tools.
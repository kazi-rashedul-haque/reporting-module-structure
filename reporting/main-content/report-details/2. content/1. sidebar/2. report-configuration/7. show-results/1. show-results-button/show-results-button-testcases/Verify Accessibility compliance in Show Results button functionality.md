**Title:** Verify Accessibility compliance in Show Results button functionality

---

**Preconditions:**
- User is logged into the workspace as an authenticated user
- At least one report exists in the report list
- Report details page is accessible
- Screen reader software is available (NVDA, JAWS, or VoiceOver)
- Browser supports keyboard navigation and accessibility features

---

**Test Steps:**
1. Navigate to the **Reporting page**.
2. Select any existing report from the Reports table to open the report details page.
3. Press the `Tab` key repeatedly to navigate through all interactive elements until reaching the "Show Results" button.
4. Press `Shift + Tab` to navigate backward to the "Show Results" button.
5. Verify the button receives proper focus indication when tabbed to.
6. Press `Enter` and `Space` on the disabled "Show Results" button to verify no action occurs.
7. Make a configuration change to enable the "Show Results" button.
8. Tab to the now-enabled "Show Results" button and verify focus indication.
9. Press `Enter` to activate the button and verify report generation begins.
10. Enable **screen reader** and navigate to the "Show Results" button in both disabled and enabled states.
11. Verify the screen reader properly announces the button label, state, and role.
12. Use browser **developer tools** to inspect ARIA labels and semantic markup of the button.
13. Test **color contrast** ratios for the button text in both enabled and disabled states.
14. Test the button at **200% zoom level** for readability and usability.
15. Switch to **mobile view** and verify touch target sizing meets accessibility standards.
16. Test with **high contrast mode** enabled to ensure button visibility.

---

**Expected Result:**
- Each `Tab` key press moves focus in logical order:
    1. Previous configuration element
    2. **Show Results button**
    3. Next sidebar element (Save changes button if visible)
- `Shift + Tab` navigates in reverse order correctly to and from the button.
- Interactive button can be activated with both `Enter` and `Space` keys when enabled.
- Disabled button does not respond to `Enter` or `Space` activation.
- **Screen reader** properly announces:
    - Button label: "Show Results" 
    - Button role: "button"
    - Button state: "disabled" or "enabled"
    - Loading state: "busy" or loading indicator when processing
- **ARIA compliance**: 
    - Proper `role="button"` attribute
    - `aria-disabled="true/false"` reflects current state
    - `aria-label` or accessible name is present and descriptive
    - `aria-busy="true"` during loading state
- **Visual accessibility**: 
    - WCAG AA color contrast ratios (4.5:1 for text, 3:1 for graphics)
    - Clear visual distinction between enabled and disabled states
    - Visible focus indicators with 3:1 contrast ratio
- **Mobile accessibility**: 
    - Touch targets meet 44x44 pixel minimum size
    - Button remains usable in mobile view
- **Focus management**: 
    - Clear focus indicators visible in all states
    - Focus is not trapped or lost during state changes
    - Logical tab order maintained throughout interaction
- No accessibility violations when tested with automated tools (axe-core or similar).
**Title:** Verify **Accessibility** compliance in line chart report type selection

---

**Preconditions:**
- At least one report exists in the report list
- The sidebar is currently expanded
- Screen reader software is available (NVDA, JAWS, or VoiceOver)
- Browser supports keyboard navigation and accessibility features

---

**Test Steps:**
1. Login to the **Workspace** as **authenticated user**.
2. Navigate to the Reporting page and open any report details page.
3. Press the `Tab` key repeatedly to navigate through Report Type radio button group.
4. Press `Shift + Tab` to navigate backward through the radio buttons.
5. Use `Arrow keys` to navigate between different report type options including line chart.
6. Press `Enter` and `Space` on the line chart option to verify activation behavior.
7. Enable **screen reader** and verify content is properly announced for line chart option.
8. Use browser **developer tools** to inspect ARIA labels and semantic markup for Report Type field.
9. Test **color contrast** ratios for line chart option text and selection indicators.
10. Test the Report Type section at **200% zoom level** for readability.
11. Switch to **mobile view** and verify touch target sizing for line chart option.
12. Test with **high contrast mode** enabled.

---

**Expected Result:**
- Each `Tab` key press moves focus in a logical order:
    1. Report Type radio group
    2. Line chart radio button
    3. Bar chart radio button
    4. Other report type options
- `Shift + Tab` navigates in reverse order correctly.
- `Arrow keys` allow navigation between report type radio button options.
- Line chart option can be activated with both `Enter` and `Space` keys.
- **Screen reader** properly announces:
  - "Report Type" group label
  - "Line" option name and current selection state
  - Radio button role and group membership
- **ARIA compliance**: Proper labels, roles (radio/radiogroup), and semantic markup.
- **Visual accessibility**: WCAG AA color contrast ratios (4.5:1 text, 3:1 graphics).
- **Mobile accessibility**: Touch targets meet 44x44 pixel minimum for line chart option.
- **Focus management**: Clear focus indicators and logical navigation between options.
- No accessibility violations when tested with automated tools.
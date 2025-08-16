**Title:** Verify Accessibility compliance in table report type selection

---

**Preconditions:**
- At least one report exists in the report list
- Screen reader software is available (NVDA, JAWS, or VoiceOver)
- Browser supports keyboard navigation and accessibility features

---

**Test Steps:**
1. Login to the **Workspace** as **authenticated user**.
2. Navigate to the Reporting page.
3. Press the `Tab` key repeatedly to navigate through all interactive elements.
4. Press `Shift + Tab` to navigate backward through the elements.
5. Press `Enter` and `Space` on interactive elements to verify activation behavior.
6. Enable **screen reader** and verify content is properly announced.
7. Use browser **developer tools** to inspect ARIA labels and semantic markup.
8. Test **color contrast** ratios for all text and icons.
9. Test the section at **200% zoom level** for readability.
10. Switch to **mobile view** and verify touch target sizing.
11. Test with **high contrast mode** enabled.

---

**Expected Result:**
- Each `Tab` key press moves focus in a logical order:
    1. Report table navigation
    2. Customization sidebar Report Type group
    3. Table radio button with proper aria-label
    4. Data Category combobox
    5. Time Frame button
    6. Data Grouping combobox 
    7. Dataset combobox and Add Dataset button
    8. Add Filter button
    9. Show Results button
- `Shift + Tab` navigates in reverse order correctly.
- Radio buttons can be activated with both `Enter` and `Space` keys.
- Comboboxes can be opened with `Enter`, `Space`, or arrow keys.
- **Screen reader** properly announces radio button states, combobox values, and button purposes.
- **ARIA compliance**: Proper labels for radio group, comboboxes have accessible names, buttons have descriptive labels.
- **Visual accessibility**: WCAG AA color contrast ratios (4.5:1 text, 3:1 graphics).
- **Mobile accessibility**: Touch targets meet 44x44 pixel minimum for radio buttons and buttons.
- **Focus management**: Clear focus indicators on radio buttons, comboboxes, and buttons.
- Data table has proper table headers and cell associations for screen readers.
- No accessibility violations when tested with automated tools.
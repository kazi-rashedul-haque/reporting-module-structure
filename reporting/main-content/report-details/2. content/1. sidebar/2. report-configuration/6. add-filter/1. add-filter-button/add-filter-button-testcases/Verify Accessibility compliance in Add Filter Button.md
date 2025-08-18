**Title:** Verify **Accessibility** compliance in Add Filter Button

---

**Preconditions:**
- User is authenticated and on the report details page
- Screen reader software is available (NVDA, JAWS, or VoiceOver)
- Browser supports keyboard navigation and accessibility features

---

**Test Steps:**
1. Login to the **Workspace** as **authenticated user**.
2. Navigate to the report details page.
3. Press the `Tab` key repeatedly to navigate through all interactive elements.
4. Press `Shift + Tab` to navigate backward through the elements.
5. Press `Enter` and `Space` on the "Add Filter" button to verify activation behavior.
6. Enable **screen reader** and verify content is properly announced.
7. Use browser **developer tools** to inspect ARIA labels and semantic markup.
8. Test **color contrast** ratios for all text and icons.
9. Test the section at **200% zoom level** for readability.
10. Switch to **mobile view** and verify touch target sizing.
11. Test with **high contrast mode** enabled.

---

**Expected Result:**
- Each `Tab` key press moves focus in a logical order:
    1. Previous interactive elements
    2. "Add Filter" button receives clear focus indicator
    3. Next interactive elements in sequence
- `Shift + Tab` navigates in reverse order correctly.
- Interactive elements can be activated with both `Enter` and `Space` keys.
- **Screen reader** properly announces button as "Add Filter" with current state.
- **ARIA compliance**: Proper labels, roles, and semantic markup are present.
- **Visual accessibility**: WCAG AA color contrast ratios (4.5:1 text, 3:1 graphics).
- **Mobile accessibility**: Touch targets meet 44x44 pixel minimum.
- **Focus management**: Clear focus indicators and logical navigation.
- No accessibility violations when tested with automated tools.
**Title:** Verify **Accessibility** compliance in sidebar navigation

---

**Pre-conditions:**
- User has access to the Reporting application
- Screen reader software is available (NVDA, JAWS, or VoiceOver)
- Browser supports keyboard navigation and accessibility features

---

**Test Steps:**
1. Login to the **Workspace** as **authenticated user**.
2. Navigate to the Dashboard list page.
3. Press the `Tab` key repeatedly to navigate through all sidebar navigation elements.
4. Press `Shift + Tab` to navigate backward through the elements.
5. Press `Enter` on each navigation link to verify activation behavior.
6. Enable **screen reader** and verify content is properly announced.
7. Use browser **developer tools** to inspect ARIA labels and semantic markup.
8. Test **color contrast** ratios for navigation text and icons.
9. Test the sidebar at **200% zoom level** for readability.
10. Switch to **mobile view** and verify touch target sizing.
11. Test with **high contrast mode** enabled.

---

**Expected Result:**
- Each `Tab` key press moves focus in logical order:
    1. Dashboard link
    2. Reports link
    3. Collapse sidebar button
- `Shift + Tab` navigates in reverse order correctly.
- Navigation links can be activated with `Enter` key.
- **Screen reader** properly announces link names and states.
- **ARIA compliance**: Proper labels, roles, and semantic navigation markup.
- **Visual accessibility**: WCAG AA color contrast ratios (4.5:1 text, 3:1 graphics).
- **Mobile accessibility**: Touch targets meet 44x44 pixel minimum.
- **Focus management**: Clear focus indicators and logical navigation.
- No accessibility violations when tested with automated tools.
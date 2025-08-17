**Title:** Verify **Accessibility** compliance in Profile Dropdown Component

---

**Preconditions:**
- User is logged in as an authenticated user
- Screen reader software is available (NVDA, JAWS, or VoiceOver)
- Browser supports keyboard navigation and accessibility features

---

**Test Steps:**
1. Login to the **Workspace** as **authenticated user**.
2. Navigate to Dashboard page in the application.
3. Press the `Tab` key repeatedly to navigate to the profile avatar button.
4. Press `Enter` or `Space` to open the profile dropdown.
5. Press the `Tab` key repeatedly to navigate through all dropdown menu items.
6. Press `Shift + Tab` to navigate backward through the dropdown elements.
7. Press `Enter` and `Space` on interactive elements to verify activation behavior.
8. Enable **screen reader** and verify content is properly announced. [Limited support in Playwright - use manual verification]
9. Use browser **developer tools** to inspect ARIA labels and semantic markup.
10. Test **color contrast** ratios for all text and icons in the dropdown.
11. Test the dropdown at **200% zoom level** for readability.
12. Switch to **mobile view** and verify touch target sizing.
13. Test with **high contrast mode** enabled.

---

**Expected Result:**
- Each `Tab` key press moves focus in a logical order:
    1. Profile avatar button
    2. Profile link (when dropdown is open)
    3. Help link
    4. New Features link
    5. Notification Settings link
    6. Display as Member button
    7. Edit Mode button
    8. Dark Mode toggle
    9. Logout link
- `Shift + Tab` navigates in reverse order correctly.
- Interactive elements can be activated with both `Enter` and `Space` keys.
- **Screen reader** properly announces profile button, dropdown state, and menu items.
- **ARIA compliance**: Proper labels, roles, and semantic markup for dropdown and menu items.
- **Visual accessibility**: WCAG AA color contrast ratios (4.5:1 text, 3:1 graphics).
- **Mobile accessibility**: Touch targets meet 44x44 pixel minimum.
- **Focus management**: Clear focus indicators and logical navigation within dropdown.
- Dropdown traps focus correctly and returns focus to avatar button on close.
- Dark Mode toggle state is properly announced by screen readers.
- Logout option in red maintains sufficient contrast for accessibility.
- No accessibility violations when tested with automated tools (axe-core).
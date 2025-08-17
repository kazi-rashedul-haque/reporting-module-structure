**Title:** Verify **Accessibility** compliance in Create Dashboard Modal

---

**Pre-conditions:**
- User has access to Dashboard List page
- Screen reader software is available (NVDA, JAWS, or VoiceOver)
- Browser supports keyboard navigation and accessibility features

---

**Test Steps:**
1. Login to the **Workspace** as **authenticated user**.
2. Navigate to the Dashboard List page.
3. Click on the "Create Dashboard" button.
4. Press the `Tab` key repeatedly to navigate through all interactive elements.
5. Press `Shift + Tab` to navigate backward through the elements.
6. Press `Enter` and `Space` on interactive elements to verify activation behavior.
7. Enable **screen reader** and verify content is properly announced. [Limited support in Playwright - use manual verification]
8. Use browser **developer tools** to inspect ARIA labels and semantic markup.
9. Test **color contrast** ratios for all text and icons.
10. Test the modal at **200% zoom level** for readability.
11. Switch to **mobile view** and verify touch target sizing.
12. Test with **high contrast mode** enabled.

---

**Expected Result:**
- Each `Tab` key press moves focus in a logical order:
    1. Dashboard Name field
    2. Description field
    3. Cancel button
    4. Save Changes button
    5. Close button (X)
- `Shift + Tab` navigates in reverse order correctly.
- Interactive elements can be activated with both `Enter` and `Space` keys.
- **Screen reader** properly announces modal title, field labels, and required indicators.
- **ARIA compliance**: Proper labels, roles, and semantic markup for modal elements.
- **Visual accessibility**: WCAG AA color contrast ratios (4.5:1 text, 3:1 graphics).
- **Mobile accessibility**: Touch targets meet 44x44 pixel minimum.
- **Focus management**: Clear focus indicators and logical navigation within modal.
- Modal traps focus correctly and returns focus to trigger button on close.
- Required field indicators are properly announced by screen readers.
- No accessibility violations when tested with automated tools.
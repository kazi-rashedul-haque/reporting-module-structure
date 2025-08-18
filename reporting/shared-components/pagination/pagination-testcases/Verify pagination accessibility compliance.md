**Title:** Verify **Accessibility** compliance in Pagination Component

---

**Preconditions:**
- At least 21 reports exist in the system to ensure pagination is displayed
- Screen reader software is available (NVDA, JAWS, or VoiceOver)
- Browser supports keyboard navigation and accessibility features

---

**Test Steps:**
1. Login to the **Workspace** as **authenticated user**.
2. Navigate to the **Reports** page.
3. Verify pagination component is visible at the bottom of the reports table.
4. Press the `Tab` key repeatedly to navigate through all pagination elements.
5. Press `Shift + Tab` to navigate backward through pagination elements.
6. Press `Enter` and `Space` on interactive pagination elements to verify activation behavior.
7. Enable **screen reader** and verify pagination content is properly announced.
8. Use browser **developer tools** to inspect ARIA labels and semantic markup.
9. Test **color contrast** ratios for all pagination text and icons.
10. Test the pagination section at **200% zoom level** for readability.
11. Switch to **mobile view** and verify touch target sizing.
12. Test with **high contrast mode** enabled.
13. Verify keyboard navigation reaches all interactive elements:
    - Page size selector dropdown
    - Page number buttons  
    - Next/Previous page buttons
14. Test dropdown functionality using keyboard (Space/Enter to open, arrow keys to navigate).
15. Verify focus indicators are clearly visible on all interactive elements.

---

**Expected Result:**
- Each `Tab` key press moves focus in a logical order:
    1. Page size selector button ("20")
    2. Page number button ("2") 
    3. Next Page button with arrow icon
- `Shift + Tab` navigates in reverse order correctly.
- Interactive elements can be activated with both `Enter` and `Space` keys.
- **Screen reader** properly announces:
    - Current page information ("Displaying 1 - 20 of 28 {ITEM_TYPE_PLURAL_CAPITALIZED}")
    - Page size selector ("Page Size, button, 20")
    - Page navigation ("Page 2, button" and "Next Page, button")
- **ARIA compliance**: Proper labels, roles, and semantic markup for:
    - Pagination list structure using `<list>` and `<listitem>` elements
    - Page size dropdown with proper expanded/collapsed states
    - Navigation buttons with descriptive labels
- **Visual accessibility**: WCAG AA color contrast ratios (4.5:1 text, 3:1 graphics).
- **Mobile accessibility**: Touch targets meet 44x44 pixel minimum.
- **Focus management**: Clear focus indicators and logical navigation order.
- **Dropdown accessibility**:
    - Page size dropdown opens/closes with keyboard
    - Arrow keys navigate through size options (10, 20, 30, 40, 50)
    - Enter/Space selects options
    - Escape closes dropdown
- No accessibility violations when tested with automated tools.
- All pagination text remains readable at 200% zoom level.
- High contrast mode preserves functionality and visibility.
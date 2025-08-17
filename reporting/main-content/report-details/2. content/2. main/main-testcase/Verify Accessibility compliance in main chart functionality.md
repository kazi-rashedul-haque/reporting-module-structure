**Title:** Verify **Accessibility** compliance in main chart functionality

---

**Preconditions:**
- At least one user report exists in the report list with configured chart data
- Screen reader software is available (NVDA, JAWS, or VoiceOver)
- Browser supports keyboard navigation and accessibility features

---

**Test Steps:**
1. Login to the **Workspace** as **authenticated user**.
2. Navigate to the Reporting page.
3. Select any existing report from the Reports table to open the report details page.
4. Ensure the chart is configured and displaying data in the main area.
5. Press the `Tab` key repeatedly to navigate through all interactive elements in the main chart area.
6. Press `Shift + Tab` to navigate backward through the elements.
7. Press `Enter` and `Space` on interactive chart elements to verify activation behavior.
8. Right-click on the chart to open context menu and test keyboard navigation within the menu.
9. Press `Escape` to close context menu and verify focus returns appropriately.
10. Enable **screen reader** and verify chart content and data is properly announced.
11. Use browser **developer tools** to inspect ARIA labels and semantic markup on chart elements.
12. Test **color contrast** ratios for all chart elements, text, and icons.
13. Test the chart section at **200% zoom level** for readability and functionality.
14. Switch to **mobile view** and verify touch target sizing for chart interactions.
15. Test with **high contrast mode** enabled to ensure chart visibility.

---

**Expected Result:**
- Each `Tab` key press moves focus in a logical order:
    1. Chart container/main chart area
    2. Chart interactive elements (if any)
    3. Context menu items (when menu is open)
    4. Chart toolbar buttons (if present)
- `Shift + Tab` navigates in reverse order correctly.
- Interactive chart elements can be activated with both `Enter` and `Space` keys.
- **Screen reader** properly announces chart type, data values, and interactive states.
- **ARIA compliance**: Proper labels, roles, and semantic markup for chart elements.
- **Visual accessibility**: WCAG AA color contrast ratios (4.5:1 text, 3:1 graphics) for all chart elements.
- **Mobile accessibility**: Touch targets for chart interactions meet 44x44 pixel minimum.
- **Focus management**: Clear focus indicators and logical navigation through chart elements.
- Chart remains functional and readable at 200% zoom level.
- Chart elements are visible and distinguishable in high contrast mode.
- No accessibility violations when tested with automated tools.
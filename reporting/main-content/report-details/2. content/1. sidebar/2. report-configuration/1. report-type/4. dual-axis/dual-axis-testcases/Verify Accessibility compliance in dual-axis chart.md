**Title:** Verify **Accessibility** compliance in dual-axis chart

---

**Preconditions:**
- Dual-axis chart is configured and displaying data with both bar and line components
- Screen reader software is available (NVDA, JAWS, or VoiceOver)
- Browser supports keyboard navigation and accessibility features

---

**Test Steps:**
1. Login to the **Workspace** as **authenticated user**.
2. Navigate to the Reporting page and open a report with dual-axis chart configuration.
3. Press the `Tab` key repeatedly to navigate through all interactive chart elements.
4. Press `Shift + Tab` to navigate backward through the chart elements.
5. Press `Enter` and `Space` on interactive chart elements to verify activation behavior.
6. Enable **screen reader** and verify chart content is properly announced.
7. Use browser **developer tools** to inspect ARIA labels and semantic markup on chart elements.
8. Test **color contrast** ratios for all chart elements, legend items, and axis labels.
9. Test the chart section at **200% zoom level** for readability.
10. Switch to **mobile view** and verify touch target sizing for interactive elements.
11. Test with **high contrast mode** enabled.
12. Verify keyboard navigation through chart configuration sidebar options.
13. Test screen reader announcement of chart data values and legend items.
14. Verify chart context menu accessibility via keyboard navigation.
15. Test accessibility of chart tooltips and data point interactions.

---

**Expected Result:**
- Each `Tab` key press moves focus in a logical order:
    1. Chart configuration sidebar elements (Data Category, Time Frame, X Axis, Y Axis Left, Y Axis Right)
    2. Add Dataset buttons
    3. Add Filter option
    4. Chart area (if interactive)
    5. Chart legend items
    6. Chart context menu trigger (if applicable)
- `Shift + Tab` navigates in reverse order correctly.
- Interactive elements can be activated with both `Enter` and `Space` keys.
- **Screen reader** properly announces:
  - Chart type as "dual-axis chart with bar and line components"
  - Y Axis Left (Bar) data series names and values
  - Y Axis Right (Line) data series names and values
  - Chart legend items with corresponding colors
  - Data point values when navigating chart elements
- **ARIA compliance**: Proper labels, roles, and semantic markup:
  - Chart container has appropriate `role="img"` or `role="application"`
  - Descriptive `aria-label` for the complete chart
  - Legend items have proper `aria-describedby` relationships
  - Configuration controls have descriptive labels
- **Visual accessibility**: WCAG AA color contrast ratios (4.5:1 text, 3:1 graphics):
  - Bar chart colors meet contrast requirements against background
  - Line chart colors meet contrast requirements against background
  - Axis labels and legend text meet text contrast requirements
  - Chart elements remain distinguishable in high contrast mode
- **Mobile accessibility**: Touch targets meet 44x44 pixel minimum:
  - Configuration dropdown buttons
  - Add Dataset buttons
  - Legend interaction areas
  - Chart context menu triggers
- **Focus management**: Clear focus indicators and logical navigation:
  - Visible focus indicators on all interactive elements
  - Focus doesn't get trapped in chart area
  - Logical tab order through all chart-related controls
- No accessibility violations when tested with automated tools (axe-core integration).
- Chart data remains accessible and understandable at 200% zoom level.
- All chart functionality remains accessible via keyboard navigation without mouse interaction.
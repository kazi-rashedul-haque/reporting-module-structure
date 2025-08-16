**Title:** Verify Accessibility compliance in Sidebar Header Title

---

**Preconditions:**
- User is logged into the workspace as an authenticated user
- At least one report exists in the reports list
- Screen reader software is available (NVDA, JAWS, or VoiceOver)
- Browser supports keyboard navigation and accessibility features

---

**Test Steps:**
1. Navigate to the Reporting page.
2. Select any existing report from the reports table to open report details page.
3. Press the `Tab` key repeatedly to navigate through all interactive elements until reaching the sidebar area.
4. Press `Shift + Tab` to navigate backward through the elements to the sidebar header.
5. Enable **screen reader** and navigate to the sidebar header title.
6. Use browser **developer tools** to inspect the title element for ARIA labels and semantic markup.
7. Verify the title element uses proper heading semantics (h1, h2, h3, etc.).
8. Test **color contrast** ratios for the title text against its background.
9. Test the sidebar at **200% zoom level** for title readability.
10. Switch to **mobile view** and verify title accessibility on smaller screens.
11. Test with **high contrast mode** enabled in the operating system.

---

**Expected Result:**
- **Screen reader** properly announces the "Customization" title as a heading with appropriate level.
- **ARIA compliance**: Title element has proper semantic markup (heading role/tag).
- **Keyboard navigation**: Focus can reach the sidebar area and title is announced when navigating.
- **Visual accessibility**: Title text meets WCAG AA color contrast ratios (4.5:1 minimum for normal text).
- **Zoom accessibility**: Title remains readable and properly positioned at 200% zoom.
- **Mobile accessibility**: Title is accessible and readable on mobile devices.
- **High contrast mode**: Title remains visible and readable with system high contrast settings.
- **Semantic structure**: Title uses appropriate heading level (likely h2 or h3) within the page hierarchy.
- No accessibility violations when tested with automated accessibility tools.
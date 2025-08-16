**Title:** Verify **Accessibility** compliance in Report Metadata Section

---

**Preconditions:**
- At least one user-created report exists in the system.
- Screen reader software is available (NVDA, JAWS, or VoiceOver).
- Browser supports keyboard navigation and accessibility features.

---

**Test Steps:**
1. Login to the **Workspace** as an **authenticated user**.
2. Navigate to the **Reporting** page via Apps > "Reporting NEW - Beta".
3. Click on the **Reports** tab in the left navigation.
4. Click on a **user-created report** link to open the report details page.
5. Locate the **report metadata section** in the header area.
6. Press the `Tab` key repeatedly to navigate through all interactive elements in the metadata section.
7. Press `Shift + Tab` to navigate backward through the elements.
8. Press `Enter` and `Space` on the **Favorite button** to verify activation behavior.
9. Enable **screen reader** and navigate to the metadata section.
10. Verify that all metadata content is properly announced by the screen reader.
11. Use browser **developer tools** to inspect ARIA labels and semantic markup.
12. Test **color contrast** ratios for all text and icons against their backgrounds.
13. Test the section at **200% zoom level** for readability.
14. Switch to **mobile view** and verify touch target sizing and responsiveness.
15. Test with **high contrast mode** enabled.

---

**Expected Result:**
- Each `Tab` key press moves focus in a logical order:
    1. Favorite Button (if interactive elements precede it)
    2. Next interactive element after metadata section
- `Shift + Tab` navigates in reverse order correctly.
- **Favorite button** can be activated with both `Enter` and `Space` keys.
- **Screen reader** properly announces:
    - "Created by You" or "Created by System Generated"
    - "Last modified on [timestamp]" with actual date and time
    - Favorite button state: "Add to favorites" or "Remove from favorites"
- **ARIA compliance**:
    - Favorite button has proper `aria-label` attributes
    - Metadata section uses semantic HTML markup
    - Interactive elements have appropriate ARIA roles
- **Visual accessibility**:
    - Text meets WCAG AA color contrast ratio of 4.5:1
    - Icons meet WCAG AA contrast ratio of 3:1
    - Text remains readable at 200% zoom level
    - High contrast mode displays content clearly
- **Mobile accessibility**:
    - Favorite button meets minimum touch target size of 44x44 pixels
    - Metadata section is responsive and readable on mobile screens
    - Mobile screen readers announce content properly
- **Focus management**:
    - Focus indicators are clearly visible
    - Focus moves logically without skipping elements
    - Non-interactive text (Created by, Last modified) does not receive focus
- No accessibility violations when tested with automated tools (axe-core, WAVE).
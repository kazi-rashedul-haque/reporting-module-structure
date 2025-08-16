**Title:** Verify collapse button visibility and enabled state

**Pre-conditions:**
* At least one report exists in the report list

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reporting page.
3. Select any existing report from the report table to open report details page.
4. Verify the collapse button is visible in the sidebar header.
5. Verify the collapse button is clickable and enabled.
6. Inspect the button element to ensure it has proper accessibility attributes.

**Expected Result:**
* The collapse button should be clearly visible in the sidebar header.
* The button should appear enabled and clickable with proper cursor behavior on hover.
* The button should have appropriate ARIA labels and role attributes for accessibility.
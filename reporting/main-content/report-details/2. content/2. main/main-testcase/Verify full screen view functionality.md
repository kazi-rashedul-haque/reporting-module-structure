**Title:** Verify full screen view functionality

**Pre-conditions:**
* At least one user report exists in the report list with configured chart data (e.g., bar chart, line chart).

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reporting page.
3. Select any existing report from the Reports table to open the report details page.
4. Ensure the chart is configured and displaying data in the main area.
5. Hamburger Menu click on the chart to open the context menu.
6. Select "View in Full Screen" from the context menu.
7. Verify that the chart expands to full screen mode.
8. Test basic interactions within full screen mode (hover, tooltips if available).
9. Press the Escape key or click exit button to exit full screen mode.
10. Verify return to normal view.

**Expected Result:**
* "View in Full Screen" option should be available in the chart context menu.
* Selecting this option should expand the chart to full screen for enhanced visibility.
* The chart should maintain its quality and proportions in full screen mode.
* User should be able to exit full screen mode using Escape key normal view.
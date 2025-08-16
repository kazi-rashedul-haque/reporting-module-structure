**Title:** Verify Add Dataset functionality for dual Y Axis

**Pre-conditions:**
* At least one report exists in the report list
* Line chart is selected as the report type
* Primary Y Axis dataset is configured

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reporting page.
3. Select any existing report from the report table to open report details page.
4. Select Line chart as the report type.
5. Configure the primary Y Axis with any data metric.
6. Locate the "Add Dataset" button.
7. Click the "Add Dataset" button.
8. Verify a second Y Axis configuration field appears.
9. Verify the second Y Axis has the same dropdown options as the primary.
10. Configure the second Y Axis with a different metric.
11. Verify both datasets are independently configurable.

**Expected Result:**
* "Add Dataset" button should be visible and clickable
* Second Y Axis configuration should appear after clicking the button
* Second Y Axis should have identical metric options to the primary
* Both datasets should be configurable independently
* Maximum of 2 datasets should be enforced
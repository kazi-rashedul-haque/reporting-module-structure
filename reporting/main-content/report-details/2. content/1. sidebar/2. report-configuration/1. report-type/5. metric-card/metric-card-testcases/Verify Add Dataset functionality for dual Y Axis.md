**Title:** Verify Add Dataset functionality for dual Y Axis

**Pre-conditions:**
* At least one report exists in the report list
* Metric Card is selected as the report type
* Primary dataset configuration is completed

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reporting page.
3. Select any existing report from the report table to open report details page.
4. Select Metric Card as the report type.
5. Configure the Data Category, Time Frame, Data Grouping, and Dataset fields.
6. Locate the "Add Dataset" button.
7. Click the "Add Dataset" button.
8. Verify a second dataset configuration section appears.
9. Verify the second dataset has the same dropdown options as the primary.
10. Configure the second dataset with different values.
11. Verify both datasets are independently configurable.

**Expected Result:**
* "Add Dataset" button should be visible and clickable
* Second dataset configuration should appear after clicking the button
* Second dataset should have identical options to the primary configuration
* Both datasets should be configurable independently
* Maximum of 2 datasets should be enforced
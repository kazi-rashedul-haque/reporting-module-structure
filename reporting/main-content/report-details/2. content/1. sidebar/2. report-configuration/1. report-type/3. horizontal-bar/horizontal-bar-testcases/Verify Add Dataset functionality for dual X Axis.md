**Title:** Verify Add Dataset functionality for dual X Axis

**Pre-conditions:**
* At least one report exists in the report list
* Horizontal Bar chart is selected as the report type
* X Axis has been configured with initial data metric

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reporting page.
3. Select any existing report from the report table to open report details page.
4. Select Horizontal Bar chart as the report type.
5. Configure the X Axis with a data metric (e.g., "# of Ideas Submitted").
6. Look for and click the "Add Dataset" button that appears.
7. Verify that a second X Axis configuration section appears.
8. Configure the second X Axis with a different data metric (e.g., "# of Idea Views").
9. Verify that color picker options appear for dataset differentiation.
10. Test the maximum limit by attempting to add a third dataset.

**Expected Result:**
* "Add Dataset" button should appear after initial X Axis selection
* Clicking "Add Dataset" should create a second X Axis configuration section
* Second X Axis should have the same data metric options as the first
* Maximum of 2 datasets for X Axis
* Note: X Axis represents data values in horizontal bar charts
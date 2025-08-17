**Title:** Verify chart type selection functionality

**Pre-conditions:**
* At least one user report exists in the report list

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reporting page.
3. Select any existing report from the Reports table to open the report details page.
4. Navigate to the sidebar report configuration section.
5. Locate the report type dropdown/selection field.
6. Verify that the following chart options are available:
   - Line
   - Bar
   - Horizontal Bar
   - Dual Axis
7. Select each chart type one by one.
8. Click "Show Results" button after each selection.
9. Verify that the chart in the main area updates accordingly for each selection.

**Expected Result:**
* All four chart types (Line, Bar, Horizontal Bar, Dual Axis) should be available for selection.
* Selecting each chart type should update the chart visualization in the main area accordingly.
* The chart should render properly for each selected type.
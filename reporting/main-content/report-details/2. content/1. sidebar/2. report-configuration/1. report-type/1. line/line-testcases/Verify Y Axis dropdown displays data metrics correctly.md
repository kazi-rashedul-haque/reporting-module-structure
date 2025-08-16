**Title:** Verify Y Axis dropdown displays data metrics correctly

**Pre-conditions:**
* At least one report exists in the report list
* Line chart is selected as the report type

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reporting page.
3. Select any existing report from the report table to open report details page.
4. Select Line chart as the report type.
5. Locate the Y Axis dropdown field.
6. Verify "Max 2 datasets" label is displayed.
7. Click on the Y Axis dropdown to open the options list.
8. Verify dropdown contains data metrics including: # of Ideas Submitted, # of Idea Views, # of Idea Votes, Idea Up Votes, Idea Down Votes, # of Comment Votes, Comment Up Votes, Comment Down Votes, # of Comments, Engagement Actions, # of Shares, Tags Applied.
9. Verify additional metrics: Reviews Completed, Assessments Completed, Estimations Completed, Refinements Submitted, Fund Allocations, Build Team Activity Count, Net Activity Score, Idea Stage Changes, Moderator Activity Count, Moderator Activity Per Idea, Selected Ideas, Implemented Ideas.
10. Select one metric and verify selection is applied.
11. Verify dropdown closes after selection.

**Expected Result:**
* Y Axis dropdown should display comprehensive list of data metrics
* All expected metrics should be available for selection
* "Max 2 datasets" limitation should be clearly indicated
* Selected metric should be applied and displayed in the field
* Dropdown should function smoothly without performance issues
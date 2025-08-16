**Title:** Verify modal interaction with multiple dashboards selection.

**Preconditions:**
* At least 5 different dashboards exist in the dashboard list.
* Dashboards have different names for easy identification

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to Reporting page and open any report details.
3. Open Add to Dashboard modal via Actions dropdown.
4. Select the first dashboard by clicking its label.
5. Verify button shows "Add to 1 Dashboard".
6. Select the second dashboard.
7. Verify button shows "Add to 2 Dashboards".
8. Continue selecting up to 5 dashboards.
9. Verify button text updates correctly for each selection.
10. Deselect the third dashboard.
11. Verify button shows "Add to 4 Dashboards".

**Expected Result:**
* Multiple dashboard selection works correctly
* Button text updates accurately with each selection
* Singular vs plural text is handled properly ("Dashboard" vs "Dashboards")
* Selection count is always accurate
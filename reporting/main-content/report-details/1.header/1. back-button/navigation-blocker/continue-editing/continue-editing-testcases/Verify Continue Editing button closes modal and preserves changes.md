**Title:** Verify Continue Editing button closes modal and preserves changes

Precondition:
At least one report is available in the report list.
**Steps:**
1. Log in to the workspace.
2. Go to the Reporting page.
3. Open any existing report.
4. Make some changes to the report (e.g., change type, axis, or dataset).
5. Click Show Results to apply the changes.
6. Without saving, try to leave the page (this should open a warning popup).
7. In the popup, click Continue Editing.

**Expected Result:**
The popup closes.
You stay on the report editing page.
All your changes are still there and editable.
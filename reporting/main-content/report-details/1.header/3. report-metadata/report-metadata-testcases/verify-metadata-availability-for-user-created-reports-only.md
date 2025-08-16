**Title:** Verify metadata fields are available only for user-created reports as per specifications

**Pre-conditions:**
* Both user-created and system-generated reports exist in the system

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reporting page.
3. Identify and open a user-created report (showing "You" in Created by column).
4. Verify that all metadata fields are present:
   - "Created by You" field
   - "Last modified on" field with timestamp
5. Navigate back to the Reports list.
6. Identify and open a system-generated report (showing "System Generated" in Created by column).
7. Examine the metadata section for system-generated reports.
8. Compare the metadata availability between user-created and system-generated reports.
9. Test with multiple reports of each type to ensure consistency.

**Expected Result:**
* For user-created reports: Both "Created by" and "Last modified on" fields should be displayed.
* For system-generated reports: The "Created by" field should not display.
* The metadata availability should be consistent across all reports of the same type.
* The behavior should match the specifications outlined in the use-cases documentation.
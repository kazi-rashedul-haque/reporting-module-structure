# Title: Ideas_ExceedDescriptionLength_030

# Pre-Condition: User has access to Reporting app with proper permissions

# Test Steps:
1. Open the browser and navigate to: https://reporting.t1.ideascale.dev
2. Accept cookies if prompted
3. Log in with the following credentials:
   - Email: superuser@ideascale.me
   - Password: brewski01
4. Click on the "Apps" button in the header
5. Click on the "Reporting" app
6. Wait for the Reporting app to load
7. Click on "Reports" in the left sidebar
8. Wait for the Reports page to load
9. Click on "Create Report" button
10. Fill in the report details:
    - Report Name: NEG_Ideas_ExceedDescriptionLength_030
    - Description: Negative test for report description exceeding 240 character limit validation. This description is intentionally very long to test the character limit validation and ensure that the system properly handles descriptions that exceed the maximum allowed length of 240 characters. Additional text here to exceed limit.
11. Attempt to type additional characters beyond the 240 character limit
12. Verify that the input field prevents typing beyond 240 characters
13. Verify character counter shows maximum limit reached
14. Attempt to click on "Next" button
15. Verify system behavior with description at/exceeding character limit

# Expected Results:
- Report description input field prevents typing beyond 240 characters
- Character counter shows 240/240 when limit is reached
- No additional characters can be entered beyond the 240 character limit
- Input field may show visual indication (red border, error styling) when limit is reached
- System either:
  - Prevents additional character input automatically (input truncation), OR
  - Shows validation error for exceeding character limit
- If validation error occurs:
  - Error message clearly indicates character limit exceeded
  - "Next" button may be disabled until within character limit
- If automatic truncation occurs:
  - Only first 240 characters are retained
  - User can proceed with truncated description
- Character counter accurately reflects current character count
- Field validation ensures data integrity
- Report name field remains functional and unaffected

# Cleanup:
1. Either proceed with the truncated description (if allowed) or reduce the description to within 240 characters
2. Click "Cancel" button to close the Create Report dialog
3. Verify that no incomplete report is created in the system
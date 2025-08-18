# Title: Members_ExceedNameLength_029

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
    - Report Name: NEG_Members_ExceedNameLength_012345678901234567890123456789012345678901234567890123456789012345678901234567890123456789ABC
    - Description: Negative test for report name exceeding 120 character limit validation
11. Attempt to type additional characters beyond the 120 character limit
12. Verify that the input field prevents typing beyond 120 characters
13. Verify character counter shows maximum limit reached
14. Attempt to click on "Next" button
15. Verify system behavior with name at/exceeding character limit

# Expected Results:
- Report name input field prevents typing beyond 120 characters
- Character counter shows 120/120 when limit is reached
- No additional characters can be entered beyond the 120 character limit
- Input field may show visual indication (red border, error styling) when limit is reached
- System either:
  - Prevents additional character input automatically (input truncation), OR
  - Shows validation error for exceeding character limit
- If validation error occurs:
  - Error message clearly indicates character limit exceeded
  - "Next" button may be disabled until within character limit
- If automatic truncation occurs:
  - Only first 120 characters are retained
  - User can proceed with truncated name
- Character counter accurately reflects current character count
- Field validation ensures data integrity

# Cleanup:
1. Either proceed with the truncated name (if allowed) or reduce the name to within 120 characters
2. Click "Cancel" button to close the Create Report dialog
3. Verify that no incomplete report is created in the system
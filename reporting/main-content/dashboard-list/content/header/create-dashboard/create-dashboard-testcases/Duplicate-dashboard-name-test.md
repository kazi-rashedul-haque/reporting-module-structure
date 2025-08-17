**Title:** Verify handling of duplicate dashboard names during creation

**Pre-conditions:**
* At least one dashboard already exists in the system

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Dashboard List page.
3. Click on the "Create Dashboard" button.
4. Enter the exact name of an existing dashboard in the Dashboard Name field.
5. Enter a valid description (optional).
6. Click the "Save Changes" button.
7. Observe the system response and any error messages.
8. Test with same name but different case (uppercase/lowercase).
9. Test with same name but leading/trailing spaces.
10. Verify error message clarity and user guidance.
11. Test correction by modifying the name to be unique.

**Expected Result:**
• System detects duplicate dashboard name before creation
• Clear error message indicates name already exists
• Error message suggests modifying name to be unique
• Form submission is prevented until name is unique
• Case sensitivity is handled consistently
• Leading and trailing spaces are trimmed properly
• Error message appears near the name field
• Save button remains disabled while duplicate exists
• User can modify name and resubmit successfully
• Error message disappears when unique name entered
• System provides helpful alternative name suggestions
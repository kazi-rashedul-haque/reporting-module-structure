**Test Case**: Verify delete button availability for user-created vs system reports

**Preconditions**: 
1. User has access to both user-created and system-generated reports

**Test Steps**:

**Scenario 1: User-created report**
1. Login to the workspace as an authenticated user
2. Navigate to the Reporting page
3. Open a user-created report details page
4. Navigate to a user-created report details page
5. Click on the Actions dropdown button in the header 
6. Verify the Delete button is present and enabled in the dropdown

**Scenario 2: System-generated report**
1. Login to the workspace as an authenticated user
2. Navigate to the Reporting page
3. Navigate to a system-generated report details page
4. Click on the Actions dropdown button in the header
5. Verify the Delete button behavior in the dropdown

**Expected Result**:
• **For user-created reports**: Delete button is visible and enabled in actions dropdown
• **For system-generated reports**: Delete button is either hidden or disabled in actions dropdown
• Delete functionality is only available for user-created reports
• System-generated reports are protected from deletion
• No error occurs when accessing actions dropdown on system reports
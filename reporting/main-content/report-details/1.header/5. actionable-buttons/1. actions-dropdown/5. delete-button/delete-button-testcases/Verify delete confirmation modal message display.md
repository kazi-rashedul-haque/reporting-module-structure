**Test Case**: Verify delete confirmation modal message display

**Test Steps**:
1. Login to the application as an authenticated user.
2. Navigate to the Reporting page.
3. Open a user-created report details page.
4. Click on the Actions dropdown button in the report header.
3. Click on the Delete button
4. Verify the modal message content

**Test Data**:
• Report name: "Monthly Sales Report"
• Report name with special characters: "Q1 2024 'Performance' & Analysis"
• Very long report name: "This is a very long report name that contains multiple words and should test message formatting"

**Expected Result**:
• Modal displays the exact message: "Are you sure you want to delete '[report_name]'?"
• Report name is correctly embedded in the confirmation message
• Special characters in report names are properly displayed
• Long report names are handled appropriately in the message
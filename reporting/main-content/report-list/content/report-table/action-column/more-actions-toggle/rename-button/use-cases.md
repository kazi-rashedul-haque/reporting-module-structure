rename_button --> onClick=opens Rename Report modal

Modal Title: Rename Report
Close_button

Report Name* textbox
    Placeholder: Enter name
    Required: true
    Max length: 120 characters
    HTML validation: Must not contain HTML tags

Description textarea
    Placeholder: Write description
    Required: false
    Max length: 240 characters
    HTML validation: Must not contain HTML tags

Cancel_button
Save_changes_button


Use Case: Rename Report Modal Functionality

Enter valid report name (1-120 characters, no HTML) and click Save
Enter valid report name and description, click Save
Enter report name with maximum allowed characters (120) and save
Enter description with maximum allowed characters (240) and save

Validation Test Cases
Use Case: Validate required field enforcement

Attempt to save with empty report name field
Verify asterisk (*) indicator shows field is required

Use Case: Validate character limits

Enter 121 characters in report name field
Enter 241 characters in description field
Test boundary values (exactly 120/240 characters)

Use Case: Validate HTML input prevention

Enter HTML tags in report name field (<script>, <div>, etc.)
Enter HTML tags in description field
Test various HTML entities and special characters

UI Interaction Test Cases
Use Case: Modal behavior and navigation

Click rename button to open modal
Verify modal title displays "Rename Report"
Click close button to dismiss modal
Click outside modal area (if applicable)
Press Escape key to close modal

Use Case: Form field interactions

Verify placeholder text displays correctly
Test tab navigation between fields
Test copy/paste functionality in both fields
Clear fields and verify placeholders reappear

Use Case: Button functionality

Cancel button closes modal without saving changes
Save button validates inputs before proceeding
Button states (enabled/disabled based on validation)

Edge Cases and Error Handling
Use Case: Handle special characters and edge inputs

Test with special characters (quotes, apostrophes, foreign characters)
Test with only spaces in required field
Test with mixed valid/invalid combinations

Use Case: System behavior validation

Test modal behavior with slow network connections
Verify data persistence after successful save
Test concurrent user scenarios (if applicable)
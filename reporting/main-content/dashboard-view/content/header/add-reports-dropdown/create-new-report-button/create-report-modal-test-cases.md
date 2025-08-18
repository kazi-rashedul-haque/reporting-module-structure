# Create Report Modal - Test Cases

## Positive Test Cases

### TC_CREATE_REPORT_001: Create New Report Modal Opens
**Description**: Verify Create New Report button opens the creation modal
**Pre-Condition**: Add Reports dropdown is open
**Test Steps**:
1. Open Add Reports dropdown
2. Click "Create New Report" option
**Expected Result**:
- Create Report modal opens
- Modal has title "Create Report"
- Form fields are empty and ready for input

### TC_CREATE_REPORT_002: Modal Structure Validation
**Description**: Verify modal contains all required elements and structure
**Pre-Condition**: Create Report modal is open
**Test Steps**:
1. Open Create Report modal
2. Verify all modal elements are present
**Expected Result**:
- Modal title: "Create Report"
- Close button (X) in top-right corner
- Report Name field with label and placeholder
- Description field with label and placeholder
- Cancel button
- Save Changes button

### TC_CREATE_REPORT_003: Report Name Field Validation
**Description**: Verify report name field properties and requirements
**Pre-Condition**: Create Report modal is open
**Test Steps**:
1. Examine Report Name field
2. Test field behavior and validation
**Expected Result**:
- Field label: "Report Name*" (asterisk indicates required)
- Placeholder text: "Enter name"
- Field is empty initially
- Field is required (mandatory for form submission)
- Maximum length: 120 characters
- HTML tags are not allowed in input

### TC_CREATE_REPORT_004: Description Field Validation
**Description**: Verify description field properties and requirements
**Pre-Condition**: Create Report modal is open
**Test Steps**:
1. Examine Description field
2. Test field behavior and validation
**Expected Result**:
- Field label: "Description"
- Placeholder text: "Write description"
- Field is empty initially
- Field is optional (not required for submission)
- Maximum length: 240 characters
- HTML tags are not allowed in input

### TC_CREATE_REPORT_005: Save Changes Success Flow
**Description**: Verify successful report creation and redirection
**Pre-Condition**: Create Report modal is open
**Test Steps**:
1. Enter valid report name (e.g., "Test Report")
2. Optionally enter description
3. Click "Save Changes" button
**Expected Result**:
- Report is created successfully
- Modal closes
- User is redirected to newly created report detail page
- Report appears in system and can be accessed

### TC_CREATE_REPORT_006: Cancel Button Functionality
**Description**: Verify Cancel button discards input and closes modal
**Pre-Condition**: Create Report modal is open with some input
**Test Steps**:
1. Enter some text in Report Name and/or Description
2. Click "Cancel" button
**Expected Result**:
- Modal closes without saving
- No report is created
- User returns to dashboard view
- Input data is discarded

### TC_CREATE_REPORT_007: Close Button Functionality
**Description**: Verify X (close) button discards input and closes modal
**Pre-Condition**: Create Report modal is open with some input
**Test Steps**:
1. Enter some text in Report Name and/or Description
2. Click X (close) button
**Expected Result**:
- Modal closes without saving
- No report is created
- User returns to dashboard view
- Input data is discarded

## Negative Test Cases

### TC_CREATE_REPORT_NEG_001: Empty Report Name Validation
**Description**: Verify validation when report name field is empty
**Pre-Condition**: Create Report modal is open
**Test Steps**:
1. Leave Report Name field empty
2. Optionally fill Description field
3. Click "Save Changes"
**Expected Result**:
- Validation error message appears
- "Report Name is required" or similar message displayed
- Modal remains open
- Save operation is prevented

### TC_CREATE_REPORT_NEG_002: Report Name Too Long
**Description**: Verify validation when report name exceeds 120 characters
**Pre-Condition**: Create Report modal is open
**Test Steps**:
1. Enter report name with 121+ characters
2. Attempt to save
**Expected Result**:
- Character limit validation triggered
- Error message about maximum length (120 characters)
- Input may be truncated automatically
- Save operation prevented if over limit

### TC_CREATE_REPORT_NEG_003: Description Too Long
**Description**: Verify validation when description exceeds 240 characters
**Pre-Condition**: Create Report modal is open
**Test Steps**:
1. Enter description with 241+ characters
2. Attempt to save
**Expected Result**:
- Character limit validation triggered
- Error message about maximum length (240 characters)
- Input may be truncated automatically
- Save operation prevented if over limit

### TC_CREATE_REPORT_NEG_004: HTML Tags in Report Name
**Description**: Verify HTML tags are rejected in report name field
**Pre-Condition**: Create Report modal is open
**Test Steps**:
1. Enter report name containing HTML tags (e.g., "<script>alert('test')</script>")
2. Attempt to save
**Expected Result**:
- HTML validation error displayed
- Tags are either stripped or validation prevents save
- Security is maintained (no script execution)
- Clear error message about invalid characters

### TC_CREATE_REPORT_NEG_005: HTML Tags in Description
**Description**: Verify HTML tags are rejected in description field
**Pre-Condition**: Create Report modal is open
**Test Steps**:
1. Enter description containing HTML tags
2. Attempt to save
**Expected Result**:
- HTML validation error displayed
- Tags are either stripped or validation prevents save
- Security is maintained
- Clear error message about invalid characters

### TC_CREATE_REPORT_NEG_006: Duplicate Report Name
**Description**: Verify handling when report name already exists
**Pre-Condition**: Report with specific name already exists
**Test Steps**:
1. Enter report name that already exists
2. Click "Save Changes"
**Expected Result**:
- Duplicate name validation error
- Error message indicating name is already in use
- Save operation prevented
- User prompted to choose different name

### TC_CREATE_REPORT_NEG_007: Network Error During Creation
**Description**: Verify handling of network errors during report creation
**Pre-Condition**: Network connectivity issues simulated
**Test Steps**:
1. Fill valid data in form
2. Click "Save Changes" with network issues
**Expected Result**:
- Error message displayed about connection problems
- Modal remains open with user data intact
- Retry option provided
- No partial report creation

## Edge Test Cases

### TC_CREATE_REPORT_EDGE_001: Maximum Valid Input Lengths
**Description**: Verify behavior with maximum allowed input lengths
**Pre-Condition**: Create Report modal is open
**Test Steps**:
1. Enter exactly 120 characters for report name
2. Enter exactly 240 characters for description
3. Save the report
**Expected Result**:
- Both fields accept maximum length input
- Save operation succeeds
- All characters are preserved in created report

### TC_CREATE_REPORT_EDGE_002: Special Characters Support
**Description**: Verify support for special characters in report data
**Pre-Condition**: Create Report modal is open
**Test Steps**:
1. Enter report name with special characters (Unicode, symbols, accents)
2. Enter description with special characters
3. Save the report
**Expected Result**:
- Special characters are accepted and preserved
- Report displays correctly with special characters
- No encoding issues occur

### TC_CREATE_REPORT_EDGE_003: Rapid Save Attempts
**Description**: Verify behavior with rapid clicking of Save button
**Pre-Condition**: Create Report modal is open with valid data
**Test Steps**:
1. Enter valid report data
2. Rapidly click "Save Changes" multiple times
**Expected Result**:
- Only one save operation is executed
- No duplicate reports are created
- Proper loading state management
- User feedback during processing

### TC_CREATE_REPORT_EDGE_004: Very Long Text Input
**Description**: Verify behavior when user pastes very long text
**Pre-Condition**: Create Report modal is open
**Test Steps**:
1. Paste text longer than field limits into name/description
2. Observe field behavior
**Expected Result**:
- Text is truncated to field limits
- User is notified about truncation
- Character count indicators work properly
- No application errors occur

## Accessibility Test Cases

### TC_CREATE_REPORT_ACC_001: Keyboard Navigation
**Description**: Verify modal is fully accessible via keyboard
**Pre-Condition**: Create Report modal is open
**Test Steps**:
1. Use Tab to navigate between form fields and buttons
2. Use Enter to activate buttons
3. Use Esc to close modal
**Expected Result**:
- All interactive elements are reachable via Tab
- Logical tab order: Report Name → Description → Cancel → Save Changes
- Enter activates buttons appropriately
- Esc closes modal and returns focus to trigger

### TC_CREATE_REPORT_ACC_002: Screen Reader Support
**Description**: Verify form is accessible to screen readers
**Pre-Condition**: Screen reader is active
**Test Steps**:
1. Open Create Report modal with screen reader
2. Navigate through all form elements
3. Test form submission with screen reader
**Expected Result**:
- Modal title is announced
- Field labels are properly associated and announced
- Required field indicators are announced ("Report Name, required")
- Placeholder text is announced
- Validation errors are announced
- Button roles and states are clear

### TC_CREATE_REPORT_ACC_003: Focus Management
**Description**: Verify proper focus management throughout modal interaction
**Pre-Condition**: Create Report modal is open
**Test Steps**:
1. Observe initial focus placement when modal opens
2. Navigate through modal elements
3. Close modal and observe focus return
**Expected Result**:
- Focus starts on first form field (Report Name)
- Focus is trapped within modal (cannot tab outside)
- Focus returns to "Create New Report" trigger when modal closes
- Focus indicators are visible and clear throughout

### TC_CREATE_REPORT_ACC_004: Error Message Accessibility
**Description**: Verify validation error messages are accessible
**Pre-Condition**: Create Report modal is open
**Test Steps**:
1. Trigger validation errors (empty name, too long text, etc.)
2. Use screen reader to navigate error messages
**Expected Result**:
- Error messages are announced when they appear
- Errors are associated with relevant form fields
- Error text is clear and actionable
- Focus moves to first field with error
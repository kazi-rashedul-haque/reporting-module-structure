# Create Dashboard Modal - Test Cases

## Positive Test Cases

### TC_CREATE_DASHBOARD_001: Create Dashboard Button Visibility
**Description**: Verify Create Dashboard button is visible and accessible in header
**Pre-Condition**: User is on Dashboard view
**Test Steps**:
1. Navigate to Dashboard view
2. Locate Create Dashboard button in header
**Expected Result**:
- "Create Dashboard" button is visible in header
- Button displays icon and "Create Dashboard" text
- Button is enabled and clickable

### TC_CREATE_DASHBOARD_002: Create Dashboard Modal Opens
**Description**: Verify clicking Create Dashboard button opens the modal
**Pre-Condition**: Dashboard view is loaded
**Test Steps**:
1. Click on "Create Dashboard" button
**Expected Result**:
- Create Dashboard modal opens
- Modal has title "Create Dashboard"
- Form fields are empty and ready for input

### TC_CREATE_DASHBOARD_003: Modal Structure Validation
**Description**: Verify modal contains all required elements and structure
**Pre-Condition**: Create Dashboard modal is open
**Test Steps**:
1. Open Create Dashboard modal
2. Verify all modal elements are present
**Expected Result**:
- Modal title: "Create Dashboard"
- Close button (X) in top-right corner
- Dashboard Name field with label and placeholder
- Description field with label and placeholder
- Cancel button
- Save Changes button

### TC_CREATE_DASHBOARD_004: Dashboard Name Field Validation
**Description**: Verify dashboard name field properties and requirements
**Pre-Condition**: Create Dashboard modal is open
**Test Steps**:
1. Examine Dashboard Name field
2. Test field behavior and validation rules
**Expected Result**:
- Field label: "Dashboard Name*" (asterisk indicates required)
- Placeholder text: "Enter name"
- Field is empty initially
- Field is required (mandatory for form submission)
- Maximum length: 120 characters
- HTML tags are not allowed in input

### TC_CREATE_DASHBOARD_005: Description Field Validation
**Description**: Verify description field properties and requirements
**Pre-Condition**: Create Dashboard modal is open
**Test Steps**:
1. Examine Description field
2. Test field behavior and validation rules
**Expected Result**:
- Field label: "Description"
- Placeholder text: "Write description"
- Field is empty initially
- Field is optional (not required for submission)
- Maximum length: 240 characters
- HTML tags are not allowed in input

### TC_CREATE_DASHBOARD_006: Save Changes Success Flow
**Description**: Verify successful dashboard creation and redirection
**Pre-Condition**: Create Dashboard modal is open
**Test Steps**:
1. Enter valid dashboard name (e.g., "My Test Dashboard")
2. Optionally enter description
3. Click "Save Changes" button
**Expected Result**:
- Dashboard is created successfully
- Modal closes
- User is redirected to newly created dashboard view
- New dashboard appears in dashboard list
- "Add Reports" dropdown appears on new dashboard

### TC_CREATE_DASHBOARD_007: Cancel Button Functionality
**Description**: Verify Cancel button discards input and closes modal
**Pre-Condition**: Create Dashboard modal is open with some input
**Test Steps**:
1. Enter some text in Dashboard Name and/or Description
2. Click "Cancel" button
**Expected Result**:
- Modal closes without saving
- No dashboard is created
- User remains on current dashboard view
- Input data is discarded

### TC_CREATE_DASHBOARD_008: Close Button Functionality
**Description**: Verify X (close) button discards input and closes modal
**Pre-Condition**: Create Dashboard modal is open with some input
**Test Steps**:
1. Enter some text in Dashboard Name and/or Description
2. Click X (close) button
**Expected Result**:
- Modal closes without saving
- No dashboard is created
- User remains on current dashboard view
- Input data is discarded

### TC_CREATE_DASHBOARD_009: Description Optional Field
**Description**: Verify dashboard can be created without description
**Pre-Condition**: Create Dashboard modal is open
**Test Steps**:
1. Enter valid dashboard name only
2. Leave description field empty
3. Click "Save Changes"
**Expected Result**:
- Dashboard is created successfully with empty description
- Modal closes and user is redirected
- Created dashboard functions normally
- Description can be added later via rename/edit

## Negative Test Cases

### TC_CREATE_DASHBOARD_NEG_001: Empty Dashboard Name Validation
**Description**: Verify validation when dashboard name field is empty
**Pre-Condition**: Create Dashboard modal is open
**Test Steps**:
1. Leave Dashboard Name field empty
2. Optionally fill Description field
3. Click "Save Changes"
**Expected Result**:
- Validation error message appears
- "Dashboard Name is required" or similar message displayed
- Modal remains open
- Save operation is prevented
- Focus moves to Dashboard Name field

### TC_CREATE_DASHBOARD_NEG_002: Dashboard Name Too Long
**Description**: Verify validation when dashboard name exceeds 120 characters
**Pre-Condition**: Create Dashboard modal is open
**Test Steps**:
1. Enter dashboard name with 121+ characters
2. Attempt to save
**Expected Result**:
- Character limit validation triggered
- Error message about maximum length (120 characters)
- Input may be truncated automatically
- Save operation prevented if over limit
- Character count indicator may show warning

### TC_CREATE_DASHBOARD_NEG_003: Description Too Long
**Description**: Verify validation when description exceeds 240 characters
**Pre-Condition**: Create Dashboard modal is open
**Test Steps**:
1. Enter description with 241+ characters
2. Attempt to save
**Expected Result**:
- Character limit validation triggered
- Error message about maximum length (240 characters)
- Input may be truncated automatically
- Save operation prevented if over limit
- Character count indicator may show warning

### TC_CREATE_DASHBOARD_NEG_004: HTML Tags in Dashboard Name
**Description**: Verify HTML tags are rejected in dashboard name field
**Pre-Condition**: Create Dashboard modal is open
**Test Steps**:
1. Enter dashboard name containing HTML tags (e.g., "<script>alert('test')</script>")
2. Attempt to save
**Expected Result**:
- HTML validation error displayed
- Tags are either stripped or validation prevents save
- Security is maintained (no script execution)
- Clear error message about invalid characters

### TC_CREATE_DASHBOARD_NEG_005: HTML Tags in Description
**Description**: Verify HTML tags are rejected in description field
**Pre-Condition**: Create Dashboard modal is open
**Test Steps**:
1. Enter description containing HTML tags
2. Attempt to save
**Expected Result**:
- HTML validation error displayed
- Tags are either stripped or validation prevents save
- Security is maintained
- Clear error message about invalid characters

### TC_CREATE_DASHBOARD_NEG_006: Duplicate Dashboard Name
**Description**: Verify handling when dashboard name already exists
**Pre-Condition**: Dashboard with specific name already exists
**Test Steps**:
1. Enter dashboard name that already exists
2. Click "Save Changes"
**Expected Result**:
- Duplicate name validation error or warning
- Option to proceed with duplicate name or choose different name
- Clear guidance provided to user
- Save operation may be prevented or allowed with warning

### TC_CREATE_DASHBOARD_NEG_007: Network Error During Creation
**Description**: Verify handling of network errors during dashboard creation
**Pre-Condition**: Network connectivity issues simulated
**Test Steps**:
1. Fill valid data in form
2. Click "Save Changes" with network issues
**Expected Result**:
- Error message displayed about connection problems
- Modal remains open with user data intact
- Retry option provided
- No partial dashboard creation

## Edge Test Cases

### TC_CREATE_DASHBOARD_EDGE_001: Maximum Valid Input Lengths
**Description**: Verify behavior with maximum allowed input lengths
**Pre-Condition**: Create Dashboard modal is open
**Test Steps**:
1. Enter exactly 120 characters for dashboard name
2. Enter exactly 240 characters for description
3. Save the dashboard
**Expected Result**:
- Both fields accept maximum length input
- Save operation succeeds
- All characters are preserved in created dashboard
- Dashboard functions normally with long name/description

### TC_CREATE_DASHBOARD_EDGE_002: Special Characters Support
**Description**: Verify support for special characters in dashboard data
**Pre-Condition**: Create Dashboard modal is open
**Test Steps**:
1. Enter dashboard name with special characters (Unicode, symbols, accents)
2. Enter description with special characters
3. Save the dashboard
**Expected Result**:
- Special characters are accepted and preserved
- Dashboard displays correctly with special characters
- No encoding issues occur
- Dashboard name appears correctly in lists and headers

### TC_CREATE_DASHBOARD_EDGE_003: Rapid Save Attempts
**Description**: Verify behavior with rapid clicking of Save button
**Pre-Condition**: Create Dashboard modal is open with valid data
**Test Steps**:
1. Enter valid dashboard data
2. Rapidly click "Save Changes" multiple times
**Expected Result**:
- Only one save operation is executed
- No duplicate dashboards are created
- Proper loading state management
- User feedback during processing

### TC_CREATE_DASHBOARD_EDGE_004: Very Long Text Paste
**Description**: Verify behavior when user pastes very long text
**Pre-Condition**: Create Dashboard modal is open
**Test Steps**:
1. Paste text longer than field limits into name/description
2. Observe field behavior
**Expected Result**:
- Text is truncated to field limits
- User is notified about truncation
- Character count indicators work properly
- No application errors occur

### TC_CREATE_DASHBOARD_EDGE_005: Browser Navigation During Creation
**Description**: Verify behavior when user navigates away during creation
**Pre-Condition**: Create Dashboard modal is open with unsaved data
**Test Steps**:
1. Enter dashboard data
2. Press browser back button or navigate away
**Expected Result**:
- Appropriate warning about unsaved changes
- Option to save or discard changes
- Graceful handling of navigation
- No partial dashboard creation

## Accessibility Test Cases

### TC_CREATE_DASHBOARD_ACC_001: Keyboard Navigation
**Description**: Verify modal is fully accessible via keyboard
**Pre-Condition**: Create Dashboard modal is open
**Test Steps**:
1. Use Tab to navigate between form fields and buttons
2. Use Enter to activate buttons
3. Use Esc to close modal
**Expected Result**:
- All interactive elements are reachable via Tab
- Logical tab order: Dashboard Name → Description → Cancel → Save Changes
- Enter activates buttons appropriately
- Esc closes modal and returns focus to trigger button

### TC_CREATE_DASHBOARD_ACC_002: Screen Reader Support
**Description**: Verify form is accessible to screen readers
**Pre-Condition**: Screen reader is active
**Test Steps**:
1. Open Create Dashboard modal with screen reader
2. Navigate through all form elements
3. Test form submission with screen reader
**Expected Result**:
- Modal title is announced
- Field labels are properly associated and announced
- Required field indicators are announced ("Dashboard Name, required")
- Placeholder text is announced
- Validation errors are announced
- Button roles and states are clear

### TC_CREATE_DASHBOARD_ACC_003: Focus Management
**Description**: Verify proper focus management throughout modal interaction
**Pre-Condition**: Create Dashboard modal is open
**Test Steps**:
1. Observe initial focus placement when modal opens
2. Navigate through modal elements
3. Close modal and observe focus return
**Expected Result**:
- Focus starts on first form field (Dashboard Name)
- Focus is trapped within modal (cannot tab outside)
- Focus returns to "Create Dashboard" trigger when modal closes
- Focus indicators are visible and clear throughout

### TC_CREATE_DASHBOARD_ACC_004: Error Message Accessibility
**Description**: Verify validation error messages are accessible
**Pre-Condition**: Create Dashboard modal is open
**Test Steps**:
1. Trigger validation errors (empty name, too long text, etc.)
2. Use screen reader to navigate error messages
**Expected Result**:
- Error messages are announced when they appear
- Errors are associated with relevant form fields
- Error text is clear and actionable
- Focus moves to first field with error

## Integration Test Cases

### TC_CREATE_DASHBOARD_INT_001: End-to-End Dashboard Creation Flow
**Description**: Verify complete flow from button click to using new dashboard
**Pre-Condition**: User is on existing dashboard
**Test Steps**:
1. Click "Create Dashboard" button
2. Fill out form with valid data
3. Save dashboard
4. Verify redirection to new dashboard
5. Test basic dashboard functionality
**Expected Result**:
- Complete flow works seamlessly
- User lands on functional new dashboard
- Dashboard appears in dashboard selection dropdown
- "Add Reports" functionality is available on new dashboard

### TC_CREATE_DASHBOARD_INT_002: Create Dashboard from Different Starting Points
**Description**: Verify Create Dashboard works from various dashboard states
**Pre-Condition**: Test from different dashboard types (system, user, empty)
**Test Steps**:
1. Test from system-generated dashboard
2. Test from user-created dashboard
3. Test from empty dashboard
**Expected Result**:
- Create Dashboard button works consistently
- Modal behavior is identical regardless of starting point
- New dashboard creation works from all contexts
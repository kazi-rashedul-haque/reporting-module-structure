# Rename Dashboard Modal - Test Cases

## Positive Test Cases

### TC_RENAME_MODAL_001: Rename Button Opens Modal
**Description**: Verify rename button opens the rename modal
**Pre-Condition**: Actions dropdown is open
**Test Steps**:
1. Open Actions dropdown
2. Click on "Rename" button
**Expected Result**:
- Rename Dashboard modal opens
- Modal has title "Rename Dashboard"
- Form fields are populated with current dashboard data

### TC_RENAME_MODAL_002: Modal Structure Validation
**Description**: Verify modal contains all required elements
**Pre-Condition**: Rename modal is open
**Test Steps**:
1. Open rename modal
2. Verify all modal elements
**Expected Result**:
- Modal title: "Rename Dashboard"
- Dashboard Name textbox with current name
- Description textarea with current description
- Close button (X)
- Cancel button
- Save Changes button

### TC_RENAME_MODAL_003: Dashboard Name Field Validation
**Description**: Verify dashboard name field properties and validation
**Pre-Condition**: Rename modal is open
**Test Steps**:
1. Open rename modal
2. Examine Dashboard Name field
3. Test input validation
**Expected Result**:
- Field label: "Dashboard Name*" (required indicator)
- Placeholder: "Enter name"
- Field is pre-populated with current dashboard name
- Field is required (validation on empty submission)
- Max length: 120 characters
- HTML tags are not allowed

### TC_RENAME_MODAL_004: Description Field Validation
**Description**: Verify description field properties and validation
**Pre-Condition**: Rename modal is open
**Test Steps**:
1. Open rename modal
2. Examine Description field
3. Test input validation
**Expected Result**:
- Field label: "Description"
- Placeholder: "Write description"
- Field is pre-populated with current description
- Field is optional (not required)
- Max length: 240 characters
- HTML tags are not allowed

### TC_RENAME_MODAL_005: Save Changes Success
**Description**: Verify successful dashboard rename operation
**Pre-Condition**: Rename modal is open with valid data
**Test Steps**:
1. Modify dashboard name to valid new name
2. Optionally modify description
3. Click "Save Changes" button
**Expected Result**:
- Dashboard is renamed successfully
- Modal closes
- Dashboard view updates with new name
- Success notification may be displayed

### TC_RENAME_MODAL_006: Cancel Operation
**Description**: Verify Cancel button discards changes
**Pre-Condition**: Rename modal is open with modified data
**Test Steps**:
1. Modify dashboard name and/or description
2. Click "Cancel" button
**Expected Result**:
- Modal closes
- No changes are saved
- Dashboard retains original name and description
- User returns to dashboard view

### TC_RENAME_MODAL_007: Close Button Operation
**Description**: Verify X (close) button discards changes
**Pre-Condition**: Rename modal is open with modified data
**Test Steps**:
1. Modify dashboard name and/or description
2. Click X (close) button
**Expected Result**:
- Modal closes
- No changes are saved
- Dashboard retains original name and description
- User returns to dashboard view

## Negative Test Cases

### TC_RENAME_MODAL_NEG_001: Empty Dashboard Name
**Description**: Verify validation when dashboard name is empty
**Pre-Condition**: Rename modal is open
**Test Steps**:
1. Clear the Dashboard Name field
2. Click "Save Changes"
**Expected Result**:
- Validation error displayed
- "Dashboard Name is required" message shown
- Modal remains open
- Save operation is prevented

### TC_RENAME_MODAL_NEG_002: Dashboard Name Too Long
**Description**: Verify validation when dashboard name exceeds 120 characters
**Pre-Condition**: Rename modal is open
**Test Steps**:
1. Enter dashboard name with 121+ characters
2. Attempt to save
**Expected Result**:
- Character limit validation triggered
- Error message about maximum length
- Input may be truncated at 120 characters
- Save operation prevented if over limit

### TC_RENAME_MODAL_NEG_003: Description Too Long
**Description**: Verify validation when description exceeds 240 characters
**Pre-Condition**: Rename modal is open
**Test Steps**:
1. Enter description with 241+ characters
2. Attempt to save
**Expected Result**:
- Character limit validation triggered
- Error message about maximum length
- Input may be truncated at 240 characters
- Save operation prevented if over limit

### TC_RENAME_MODAL_NEG_004: HTML Tags in Dashboard Name
**Description**: Verify HTML tags are rejected in dashboard name
**Pre-Condition**: Rename modal is open
**Test Steps**:
1. Enter dashboard name with HTML tags (e.g., "<script>alert('test')</script>")
2. Attempt to save
**Expected Result**:
- HTML validation error displayed
- Tags are either stripped or validation prevents save
- Security is maintained (no script execution)

### TC_RENAME_MODAL_NEG_005: HTML Tags in Description
**Description**: Verify HTML tags are rejected in description
**Pre-Condition**: Rename modal is open
**Test Steps**:
1. Enter description with HTML tags
2. Attempt to save
**Expected Result**:
- HTML validation error displayed
- Tags are either stripped or validation prevents save
- Security is maintained

### TC_RENAME_MODAL_NEG_006: Duplicate Dashboard Name
**Description**: Verify handling of duplicate dashboard names
**Pre-Condition**: Another dashboard with target name exists
**Test Steps**:
1. Enter name that already exists for another dashboard
2. Click "Save Changes"
**Expected Result**:
- Duplicate name validation error
- Appropriate error message displayed
- Save operation prevented
- User prompted to choose different name

## Edge Test Cases

### TC_RENAME_MODAL_EDGE_001: Maximum Valid Input Length
**Description**: Verify behavior with maximum allowed input lengths
**Pre-Condition**: Rename modal is open
**Test Steps**:
1. Enter exactly 120 characters for dashboard name
2. Enter exactly 240 characters for description
3. Save changes
**Expected Result**:
- Both fields accept maximum length input
- Save operation succeeds
- All characters are preserved

### TC_RENAME_MODAL_EDGE_002: Special Characters Support
**Description**: Verify support for special characters in names
**Pre-Condition**: Rename modal is open
**Test Steps**:
1. Enter dashboard name with special characters (Unicode, symbols)
2. Enter description with special characters
3. Save changes
**Expected Result**:
- Special characters are accepted and preserved
- Display is correct throughout the application
- No encoding issues occur

### TC_RENAME_MODAL_EDGE_003: Rapid Save Attempts
**Description**: Verify behavior with rapid clicking of Save button
**Pre-Condition**: Rename modal is open with valid data
**Test Steps**:
1. Enter valid data
2. Rapidly click "Save Changes" multiple times
**Expected Result**:
- Only one save operation is executed
- No duplicate requests
- Proper loading state management

### TC_RENAME_MODAL_EDGE_004: Browser Navigation During Edit
**Description**: Verify behavior when user navigates away during editing
**Pre-Condition**: Rename modal is open with unsaved changes
**Test Steps**:
1. Modify dashboard name/description
2. Press browser back button or navigate away
**Expected Result**:
- Appropriate warning about unsaved changes
- Option to save or discard changes
- Graceful handling of navigation

## Accessibility Test Cases

### TC_RENAME_MODAL_ACC_001: Keyboard Navigation
**Description**: Verify modal is fully accessible via keyboard
**Pre-Condition**: Rename modal is open
**Test Steps**:
1. Use Tab to navigate between form fields and buttons
2. Use Enter to activate buttons
3. Use Esc to close modal
**Expected Result**:
- All interactive elements are reachable via Tab
- Logical tab order through form fields
- Enter activates buttons appropriately
- Esc closes modal and returns focus

### TC_RENAME_MODAL_ACC_002: Screen Reader Support
**Description**: Verify form is accessible to screen readers
**Pre-Condition**: Screen reader is active
**Test Steps**:
1. Open rename modal with screen reader
2. Navigate through all form elements
**Expected Result**:
- Modal title is announced
- Field labels are associated and announced
- Required field indicators are announced
- Validation errors are announced
- Button roles and states are clear

### TC_RENAME_MODAL_ACC_003: Focus Management
**Description**: Verify proper focus management throughout interaction
**Pre-Condition**: Rename modal is open
**Test Steps**:
1. Observe initial focus placement
2. Navigate through modal elements
3. Close modal and observe focus return
**Expected Result**:
- Focus starts on first form field (Dashboard Name)
- Focus is trapped within modal
- Focus returns to rename trigger button when modal closes
- Focus indicators are visible and clear
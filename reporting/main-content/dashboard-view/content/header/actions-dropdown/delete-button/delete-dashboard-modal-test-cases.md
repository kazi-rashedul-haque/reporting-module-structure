# Delete Dashboard Modal - Test Cases

## Positive Test Cases

### TC_DELETE_MODAL_001: Delete Button Opens Modal
**Description**: Verify delete button opens the delete confirmation modal
**Pre-Condition**: Actions dropdown is open
**Test Steps**:
1. Open Actions dropdown
2. Click on "Delete" button
**Expected Result**:
- Delete Dashboard modal opens
- Modal has title "Delete Dashboard"
- Modal displays confirmation message with dashboard name

### TC_DELETE_MODAL_002: Modal Content Validation
**Description**: Verify modal displays correct content and structure
**Pre-Condition**: Delete modal is open
**Test Steps**:
1. Open delete modal
2. Verify modal content
**Expected Result**:
- Modal title: "Delete Dashboard"
- Body text: "Are you sure you want to delete '[dashboard_name]'?"
- Close button (X) is present
- Cancel button is present
- Delete button is present

### TC_DELETE_MODAL_003: Cancel Button Functionality
**Description**: Verify Cancel button closes modal without deleting
**Pre-Condition**: Delete modal is open
**Test Steps**:
1. Open delete modal
2. Click "Cancel" button
**Expected Result**:
- Modal closes
- Dashboard is not deleted
- User remains on dashboard view
- No changes to dashboard state

### TC_DELETE_MODAL_004: Close Button Functionality
**Description**: Verify X (close) button closes modal without deleting
**Pre-Condition**: Delete modal is open
**Test Steps**:
1. Open delete modal
2. Click the X (close) button
**Expected Result**:
- Modal closes
- Dashboard is not deleted
- User remains on dashboard view
- No changes to dashboard state

### TC_DELETE_MODAL_005: Delete Confirmation Success
**Description**: Verify Delete button successfully deletes dashboard
**Pre-Condition**: Delete modal is open, dashboard can be deleted
**Test Steps**:
1. Open delete modal
2. Click "Delete" button
**Expected Result**:
- Dashboard is permanently deleted
- User is redirected to dashboard list or default dashboard
- Success notification may be shown
- Deleted dashboard no longer appears in lists

### TC_DELETE_MODAL_006: Dashboard Name Display
**Description**: Verify correct dashboard name is displayed in confirmation message
**Pre-Condition**: Different dashboards available
**Test Steps**:
1. Navigate to a specific dashboard
2. Open Actions dropdown → Delete
3. Verify dashboard name in modal
**Expected Result**:
- Modal shows exact name of current dashboard
- Special characters in name are displayed correctly
- Long names are handled appropriately

## Negative Test Cases

### TC_DELETE_MODAL_NEG_001: Delete System Generated Dashboard
**Description**: Verify behavior when trying to delete system-generated dashboard
**Pre-Condition**: On system-generated dashboard
**Test Steps**:
1. Navigate to system-generated dashboard
2. Check if delete option is available
**Expected Result**:
- Delete option should be disabled or not available
- If available, deletion should be prevented with error message
- System dashboard remains protected

### TC_DELETE_MODAL_NEG_002: Delete Dashboard in Use
**Description**: Verify behavior when dashboard is referenced elsewhere
**Pre-Condition**: Dashboard is referenced by other users/systems
**Test Steps**:
1. Open delete modal for referenced dashboard
2. Click Delete button
**Expected Result**:
- Warning message about dependencies
- Option to force delete or cancel
- Appropriate error handling if deletion fails

### TC_DELETE_MODAL_NEG_003: Network Error During Deletion
**Description**: Verify handling of network errors during delete operation
**Pre-Condition**: Network connectivity issues simulated
**Test Steps**:
1. Open delete modal
2. Click Delete with network issues
**Expected Result**:
- Error message displayed
- Modal remains open
- Dashboard state unchanged
- Retry option provided

## Edge Test Cases

### TC_DELETE_MODAL_EDGE_001: Multiple Rapid Delete Attempts
**Description**: Verify behavior with rapid clicking of delete button
**Pre-Condition**: Delete modal is open
**Test Steps**:
1. Open delete modal
2. Rapidly click Delete button multiple times
**Expected Result**:
- Only one delete operation is executed
- No duplicate delete requests
- Proper loading state management

### TC_DELETE_MODAL_EDGE_002: Modal Behavior on Browser Back
**Description**: Verify modal behavior when user navigates back
**Pre-Condition**: Delete modal is open
**Test Steps**:
1. Open delete modal
2. Press browser back button
**Expected Result**:
- Modal closes gracefully
- User navigates to previous page
- No deletion occurs

### TC_DELETE_MODAL_EDGE_003: Very Long Dashboard Names
**Description**: Verify modal handles very long dashboard names
**Pre-Condition**: Dashboard with maximum length name (120 characters)
**Test Steps**:
1. Open delete modal for long-named dashboard
**Expected Result**:
- Long name is displayed properly (wrapped or truncated)
- Modal layout remains intact
- All buttons remain accessible

### TC_DELETE_MODAL_EDGE_004: Special Characters in Dashboard Name
**Description**: Verify modal handles special characters in dashboard names
**Pre-Condition**: Dashboard with special characters (&, <, >, ", ')
**Test Steps**:
1. Open delete modal for dashboard with special characters
**Expected Result**:
- Special characters are properly escaped/displayed
- No HTML injection occurs
- Modal remains functional

## Accessibility Test Cases

### TC_DELETE_MODAL_ACC_001: Keyboard Navigation
**Description**: Verify modal is fully accessible via keyboard
**Pre-Condition**: Delete modal is open
**Test Steps**:
1. Open modal
2. Use Tab to navigate between buttons
3. Use Enter/Space to activate buttons
4. Use Esc to close modal
**Expected Result**:
- Focus moves between Cancel, Delete, and Close buttons
- Enter/Space activates focused button
- Esc key closes modal
- Focus returns to delete button when modal closes

### TC_DELETE_MODAL_ACC_002: Screen Reader Support
**Description**: Verify modal content is accessible to screen readers
**Pre-Condition**: Screen reader is active
**Test Steps**:
1. Open delete modal with screen reader
2. Navigate through modal content
**Expected Result**:
- Modal title is announced
- Confirmation message is read aloud
- Button roles and states are announced
- Modal context is clear to screen reader users

### TC_DELETE_MODAL_ACC_003: Focus Management
**Description**: Verify proper focus management in modal
**Pre-Condition**: Delete modal is open
**Test Steps**:
1. Open modal and observe initial focus
2. Tab through all elements
3. Close modal and observe focus return
**Expected Result**:
- Focus starts on the first actionable element (Cancel or Delete)
- Focus is trapped within modal
- Focus returns to delete trigger button when modal closes
- Focus indicator is visible throughout
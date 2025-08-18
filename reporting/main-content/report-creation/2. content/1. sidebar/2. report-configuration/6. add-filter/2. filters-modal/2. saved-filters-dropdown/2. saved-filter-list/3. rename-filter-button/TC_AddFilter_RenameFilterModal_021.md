# TC_AddFilter_RenameFilterModal_021

## Title:
Verify Rename Filter modal validates input and updates filter name successfully

## Pre-Condition:
1. User is logged into the reporting application
2. User is on the report creation page with completed basic configuration
3. Add Filter modal is open
4. At least one saved filter exists (e.g., "Customer Experience Filter")
5. Saved Filters dropdown is expanded showing filter list

## Test Steps:
1. Locate a saved filter with rename button in the filter list
2. Click the "Rename Filter" button (edit icon)
3. Verify Rename Filter modal opens with current filter name
4. Test input field validation with various scenarios:
   - Clear field and attempt to save (empty name)
   - Enter valid new name and save
   - Enter name exceeding 120 characters
   - Enter name with HTML tags
   - Enter name with special characters
   - Enter duplicate filter name
5. Test the Close button (×) functionality
6. Test Cancel button functionality
7. Test Update button with valid input
8. Verify filter name is updated in saved filters list
9. Test character counter functionality
10. Test accessibility features of the modal

## Expected Results:
1. Rename Filter modal opens successfully when rename button is clicked
2. Modal displays correct elements:
   - Modal title: "Rename Filter"
   - Field label: "Filter Name*" (asterisk indicates required)
   - Input field pre-populated with current filter name
   - Placeholder text: "Filter Name"
   - Character counter: "X/120" showing current character count
   - Close button (×) in top-right corner
   - Cancel button (secondary styling)
   - Update button (primary styling)
3. Input field validation:
   - Empty name validation:
     - Update button becomes disabled
     - Required field validation message displayed
     - Cannot save empty or whitespace-only names
   - Character limit validation:
     - Counter updates in real-time as user types
     - Input prevents typing beyond 120 characters
     - Update button disabled when limit exceeded
   - HTML tag validation:
     - HTML tags are stripped or rejected
     - Warning message if HTML detected
     - Clean text-only names are saved
   - Special characters:
     - Most special characters are allowed
     - Proper encoding/escaping of special characters
     - Unicode characters are supported
   - Duplicate name handling:
     - System detects duplicate filter names
     - Appropriate error message displayed
     - User guided to choose unique name
4. Close button (×) functionality:
   - Clicking closes modal without saving changes
   - Original filter name remains unchanged
   - Returns to Filters modal
   - No validation errors persist
5. Cancel button functionality:
   - Clicking closes modal without saving changes
   - Input field changes are discarded
   - Original filter name preserved
   - Consistent behavior with Close button
6. Update button functionality:
   - Enabled only when valid name is entered
   - Clicking saves the new filter name
   - Modal closes after successful update
   - Returns to Filters modal with updated name
7. Filter name update verification:
   - Updated name appears in saved filters dropdown
   - Filter configuration/conditions remain unchanged
   - Only the display name is modified
   - Update persists across browser sessions
8. Character counter functionality:
   - Updates in real-time during typing
   - Shows format "current/120"
   - Visual indication when approaching limit
   - Prevents input beyond maximum length
9. Accessibility compliance:
   - Modal properly announced by screen readers
   - Input field has appropriate labels and descriptions
   - Required field status communicated to screen readers
   - Validation errors announced when they occur
   - All buttons keyboard navigable and activatable
   - Escape key closes modal without saving
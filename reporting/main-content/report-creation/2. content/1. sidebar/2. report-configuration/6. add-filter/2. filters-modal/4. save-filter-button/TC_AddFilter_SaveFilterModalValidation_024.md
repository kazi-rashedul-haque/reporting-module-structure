# TC_AddFilter_SaveFilterModalValidation_024

## Title:
Verify Save Filter modal input validation and character counter functionality

## Pre-Condition:
1. User is logged into the reporting application
2. User is on the report creation page with completed basic configuration
3. Add Filter modal is open
4. Complex filter configuration is created (multiple conditions)
5. User has clicked "Save Filter" button

## Test Steps:
1. Verify Save Filter modal opens with all required elements
2. Test character counter functionality:
   - Verify initial counter shows "0/120"
   - Type text and verify real-time counter updates
   - Test counter behavior at character limits
3. Test input validation scenarios:
   - Submit with empty filter name
   - Enter exactly 120 characters
   - Attempt to enter 121+ characters
   - Enter HTML tags in filter name
   - Enter special characters and Unicode
   - Test whitespace-only names
4. Test button states and interactions:
   - Verify Save button state changes based on validation
   - Test Close button (×) functionality
   - Test Cancel button functionality
5. Test error message display and behavior
6. Test successful save scenario
7. Test accessibility features
8. Test edge cases and error handling

## Expected Results:
1. Save Filter modal opens with correct structure:
   - Modal title: "Save Filter"
   - Field label: "Filter Name*" (required indicator)
   - Input field with placeholder: "Filter Name"
   - Character counter displaying: "0/120"
   - Close button (×) in top-right
   - Cancel button (secondary styling)
   - Save button (primary styling, initially disabled)
2. Character counter functionality:
   - Updates in real-time as user types
   - Shows format "current/120" (e.g., "15/120")
   - Counter color changes as approaching limit:
     - Normal color when under limit
     - Warning color when near limit (e.g., >100 characters)
     - Error color when at/over limit
   - Counter prevents input beyond 120 characters
3. Input validation behavior:
   - Empty/whitespace names:
     - Save button remains disabled
     - Required field validation message appears
     - Message: "Filter name is required" or similar
   - Character limit validation:
     - Input field prevents typing beyond 120 characters
     - Save button disabled when at character limit with invalid input
     - Visual indication of character limit reached
   - HTML tag validation:
     - HTML tags are stripped from input or rejected
     - Warning message if HTML detected: "HTML tags are not allowed"
     - Cleaned input is displayed without HTML
   - Special characters:
     - Most special characters allowed (!@#$%^&*()_+-=[]{}|;:,.<>?)
     - Unicode characters supported (émojis, accents, etc.)
     - Input field handles international characters correctly
4. Button interactions:
   - Save button states:
     - Disabled initially and when validation fails
     - Enabled only when valid name is entered
     - Clicking saves filter and closes modal
   - Close button (×):
     - Closes modal without saving
     - No validation errors persist
     - Input changes are discarded
   - Cancel button:
     - Same behavior as Close button
     - Consistent styling and positioning
5. Error message handling:
   - Validation errors display immediately
   - Error messages are clear and actionable
   - Errors are announced to screen readers
   - Multiple validation errors prioritized appropriately
   - Error state cleared when input becomes valid
6. Successful save scenario:
   - Valid input enables Save button
   - Clicking Save:
     - Closes modal immediately
     - Returns to Filters modal
     - New filter appears in Saved Filters dropdown
     - Success feedback provided (optional)
     - Filter configuration preserved correctly
7. Accessibility compliance:
   - Modal announced by screen readers
   - Required field status communicated
   - Character counter information available to screen readers
   - Validation errors announced when they occur
   - Keyboard navigation works for all interactive elements
   - Input field properly labeled and described
8. Edge cases and error handling:
   - Network errors during save handled gracefully
   - Duplicate filter names detected and handled
   - Modal remains functional during slow network conditions
   - Input field performs well with rapid typing
   - Modal state preserved if user navigates away and returns
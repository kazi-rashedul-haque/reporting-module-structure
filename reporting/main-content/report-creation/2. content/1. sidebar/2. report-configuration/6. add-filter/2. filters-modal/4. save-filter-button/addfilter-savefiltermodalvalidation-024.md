**Title:** Verify Save Filter modal validates input correctly and handles character limits appropriately

**Pre-Condition:**
1. User is logged into the reporting application
2. User is on the report creation page with completed basic configuration
3. Add Filter modal is open
4. Complex filter configuration is created (multiple conditions)
5. User has clicked "Save Filter" button

**Test Steps:**
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
4. Test button states and interactions
5. Test successful save scenario
6. Test duplicate filter name handling

**Expected Results:**
1. Save Filter modal opens with proper structure:
   - Modal title: "Save Filter"
   - Field label: "Filter Name*" (asterisk indicates required)
   - Input field with placeholder: "Filter Name"
   - Character counter displaying: "0/120"
   - Close button (×), Cancel button, and Save button
2. Character counter functionality:
   - Updates in real-time as user types
   - Shows format "current/120" (e.g., "15/120")
   - Prevents input beyond 120 characters
3. Input validation behavior:
   - Empty/whitespace names:
     - Save button remains disabled
     - Required field validation message displayed
   - Character limit validation:
     - Input field prevents typing beyond 120 characters
     - Visual indication when character limit is reached
   - HTML tag validation:
     - HTML tags are rejected or stripped from input
     - Warning message displayed if HTML detected
   - Special characters and Unicode are supported appropriately
4. Button functionality:
   - Save button: Disabled initially, enabled only with valid input
   - Close button (×) and Cancel button: Close modal without saving
   - Successful save: Closes modal and adds filter to Saved Filters dropdown
5. Duplicate filter name handling:
   - System detects duplicate names and displays appropriate error message
   - User is prompted to enter a unique name
6. Filter configuration is preserved correctly when saved
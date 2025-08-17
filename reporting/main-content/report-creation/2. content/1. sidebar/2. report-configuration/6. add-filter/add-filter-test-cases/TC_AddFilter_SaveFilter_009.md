# TC_AddFilter_SaveFilter_009

## Title:
Verify Save Filter functionality allows users to save and manage custom filter configurations

## Pre-Condition:
1. User is logged into the reporting application
2. User is on the report creation page with completed basic configuration
3. Add Filter modal is open
4. Complex filter configuration is created with multiple conditions

## Test Steps:
1. Configure a complex filter:
   - WHERE Campaign = "Customer Experience"
   - AND Community = "Test Community"  
   - OR Stage = "Review"
2. Click the "Save Filter" button
3. Enter filter name in the Save Filter modal
4. Save the filter and verify it appears in Saved Filters
5. Test saving filters with different names and configurations
6. Test saving filter with maximum character limit (120 characters)
7. Test saving filter with special characters
8. Attempt to save filter without entering a name

## Expected Results:
1. "Save Filter" button is visible and accessible
2. Clicking "Save Filter" opens Save Filter modal with:
   - Modal title: "Save Filter"
   - Field label: "Filter Name*" (required field)
   - Placeholder: "Filter Name"
   - Character counter: 0/120
   - Close button (×)
   - Cancel button
   - Save button
3. Filter name requirements:
   - Required field (cannot be empty)
   - Maximum 120 characters
   - HTML tags not allowed
   - Special characters allowed
4. Successful save behavior:
   - Save button saves the filter
   - Returns to Filters modal
   - Saved filter appears in Saved Filters dropdown
   - Success feedback provided to user
5. Error handling:
   - Empty name shows validation error
   - Exceeding 120 characters prevents saving
   - HTML tags are stripped or rejected
   - Duplicate names are handled appropriately
6. Saved filter contains complete configuration:
   - All filter conditions preserved
   - Nested filters maintained
   - Logical operators saved correctly
7. Save Filter modal is accessible via keyboard
8. Screen reader compatibility for save process
**Title:** Verify right operand field dynamically adapts based on left operand selection and data type

**Pre-Condition:**
1. User is logged into the reporting application
2. User is on the report creation page with completed basic configuration
3. Add Filter modal is open
4. Filter form is visible with WHERE condition

**Test Steps:**
1. Select "Campaign" from the left operand dropdown
2. Observe the right operand field changes
3. Click on the right operand dropdown and verify available options
4. Select a campaign option
5. Repeat steps 1-4 with different left operand types:
   - Select "Community" and verify community options
   - Select "Stage" and verify stage options
   - Select "Owner Status" and verify status options
   - Select date-based operands (e.g., "Campaign Start Date")
   - Select text-based operands (e.g., "Idea Title")
6. Test multi-select functionality where applicable
7. Test field behavior with different comparison operators

**Expected Results:**
1. Right operand field type changes dynamically based on left operand selection:
   - Entity-based operands (Campaign, Community, Stage): Display as dropdowns
   - Date-based operands: Display as date picker
   - Text-based operands: Display as text input field
   - Status-based operands: Display as dropdown with predefined options
2. Dropdown operands behavior:
   - Show "Select" placeholder when no selection is made
   - Populate with actual system data relevant to the selected operand
   - Display options with appropriate formatting (icons, names, etc.)
3. Multi-select functionality:
   - Available for appropriate field types
   - Selected values display with individual remove buttons
   - "Remove All" button appears when multiple items are selected
4. Field behavior adapts to comparison operator:
   - "Defined"/"Not defined" operators disable the right operand field
   - Other operators enable appropriate input type
5. Selected values are properly maintained and displayed
6. Input validation works appropriately for each field type
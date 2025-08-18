**Title:** Verify left operand dropdown displays categorized filter options and handles selection correctly

**Pre-Condition:**
1. User is logged into the reporting application
2. User is on the report creation page with completed basic configuration
3. Add Filter modal is open
4. Filter form is visible with WHERE condition

**Test Steps:**
1. Click on the left operand dropdown (showing "Select")
2. Observe the dropdown options that appear
3. Verify category groups are present and properly organized
4. Select different operands from different categories
5. Test dropdown behavior after each selection
6. Verify selected operand affects subsequent filter options

**Expected Results:**
1. Left operand dropdown expands showing all available filter options
2. Options are properly grouped by categories:
   - WORKSPACE (Workspace Group)
   - COMMUNITY (Community, Community Name, Community Group)
   - IDEA PROPERTIES (Idea, Idea Number, Idea Title, etc.)
   - IDEA OWNER (Owner, Owner Email, Owner Source, etc.)
   - IDEA SUBMITTER (Submitter, Submitter Email, etc.)
   - STAGE PROPERTIES (Stage, Stage Name, etc.)
   - CAMPAIGN PROPERTIES (Campaign, Campaign Group, etc.)
   - ENGAGEMENTS (Idea Submitted, Idea Views, etc.)
   - IDEA CUSTOM FIELDS (Single Choice, Multiple Choice)
3. Each option displays with appropriate icon and descriptive label
4. Selecting an option:
   - Updates the left operand field with selected value
   - Closes the dropdown automatically
   - Enables the comparison operator dropdown
5. Different operand selections work consistently across all categories
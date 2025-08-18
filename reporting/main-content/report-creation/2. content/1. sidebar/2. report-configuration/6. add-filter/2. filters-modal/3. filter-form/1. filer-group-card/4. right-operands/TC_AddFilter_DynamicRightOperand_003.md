# TC_AddFilter_DynamicRightOperand_003

## Title:
Verify right operand field is dynamically populated based on left operand selection

## Pre-Condition:
1. User is logged into the reporting application
2. User is on the report creation page with completed basic configuration
3. Add Filter modal is open
4. Filter form is visible with WHERE condition

## Test Steps:
1. Select "Campaign" from the left operand dropdown
2. Observe the right operand field changes
3. Click on the right operand dropdown
4. Verify available campaign options
5. Select a campaign (e.g., "Customer Experience")
6. Repeat steps 1-5 with different left operands:
   - Select "Community" and verify community options
   - Select "Stage" and verify stage options
   - Select "Owner Status" and verify status options

## Expected Results:
1. When "Campaign" is selected:
   - Right operand changes from text input to dropdown
   - Right operand shows "Select" placeholder
   - Dropdown contains actual campaign data from the system
   - Options include campaigns like: Customer Experience, Process Improvement, Product Innovation, Private Campaign
   - Each option displays campaign logo and name
2. When "Community" is selected:
   - Right operand displays available communities
3. When "Stage" is selected:
   - Right operand displays available stages
4. When "Owner Status" is selected:
   - Right operand displays status options (Active, Inactive, etc.)
5. Right operand type (dropdown, text input, date picker) changes appropriately based on data type
6. Multi-select capability is available for appropriate fields
7. Selected values are properly displayed with remove buttons
8. "Remove All" button appears when multiple items are selected
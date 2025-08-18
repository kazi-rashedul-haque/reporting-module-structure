# TC_ACTIONS_DROPDOWN_EDGE_003: Clone with Maximum Name Length

**Description**: Verify clone behavior when original name is at maximum length

**Pre-Condition**: Dashboard name is 120 characters (maximum)

**Test Steps**:
1. Open Actions dropdown
2. Click "Clone"

**Expected Result**:
- Clone operation handles long names gracefully
- New dashboard name with "(Copy)" fits within constraints
- No truncation errors occur
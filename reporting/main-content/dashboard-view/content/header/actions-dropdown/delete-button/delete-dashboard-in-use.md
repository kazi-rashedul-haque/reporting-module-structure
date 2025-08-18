**Title**: Delete Dashboard in Use

**Description**: Verify behavior when dashboard is referenced elsewhere

**Pre-Condition**: Dashboard is referenced by other users/systems

**Test Steps**:
1. Open delete modal for referenced dashboard
2. Click Delete button

**Expected Result**:
- Warning message about dependencies
- Option to force delete or cancel
- Appropriate error handling if deletion fails
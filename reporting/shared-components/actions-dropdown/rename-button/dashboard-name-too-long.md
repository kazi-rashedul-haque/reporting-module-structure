**Title**: Dashboard Name Too Long

**Description**: Verify validation when dashboard name exceeds 120 characters

**Pre-Condition**: Rename modal is open

**Test Steps**:
1. Enter dashboard name with 121+ characters
2. Attempt to save

**Expected Result**:
- Character limit validation triggered
- Error message about maximum length
- Input may be truncated at 120 characters
- Save operation prevented if over limit
# TC_RENAME_MODAL_NEG_003: Description Too Long

**Description**: Verify validation when description exceeds 240 characters

**Pre-Condition**: Rename modal is open

**Test Steps**:
1. Enter description with 241+ characters
2. Attempt to save

**Expected Result**:
- Character limit validation triggered
- Error message about maximum length
- Input may be truncated at 240 characters
- Save operation prevented if over limit
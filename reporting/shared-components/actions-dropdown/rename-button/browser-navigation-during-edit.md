**Title**: Browser Navigation During Edit

**Description**: Verify behavior when user navigates away during editing

**Pre-Condition**: Rename modal is open with unsaved changes

**Test Steps**:
1. Modify dashboard name/description
2. Press browser back button or navigate away

**Expected Result**:
- Appropriate warning about unsaved changes
- Option to save or discard changes
- Graceful handling of navigation
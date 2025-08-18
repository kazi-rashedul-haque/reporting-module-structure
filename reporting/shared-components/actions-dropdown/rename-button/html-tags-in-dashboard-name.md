# TC_RENAME_MODAL_NEG_004: HTML Tags in Dashboard Name

**Description**: Verify HTML tags are rejected in dashboard name

**Pre-Condition**: Rename modal is open

**Test Steps**:
1. Enter dashboard name with HTML tags (e.g., "<script>alert('test')</script>")
2. Attempt to save

**Expected Result**:
- HTML validation error displayed
- Tags are either stripped or validation prevents save
- Security is maintained (no script execution)
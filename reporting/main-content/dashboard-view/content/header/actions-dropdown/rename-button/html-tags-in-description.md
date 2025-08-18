**Title**: HTML Tags in Description

**Description**: Verify HTML tags are rejected in description

**Pre-Condition**: Rename modal is open

**Test Steps**:
1. Enter description with HTML tags
2. Attempt to save

**Expected Result**:
- HTML validation error displayed
- Tags are either stripped or validation prevents save
- Security is maintained
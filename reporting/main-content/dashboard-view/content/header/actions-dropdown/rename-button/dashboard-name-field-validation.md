**Title**: Dashboard Name Field Validation

**Description**: Verify dashboard name field properties and validation

**Pre-Condition**: Rename modal is open

**Test Steps**:
1. Open rename modal
2. Examine Dashboard Name field
3. Test input validation

**Expected Result**:
- Field label: "Dashboard Name*" (required indicator)
- Placeholder: "Enter name"
- Field is pre-populated with current dashboard name
- Field is required (validation on empty submission)
- Max length: 120 characters
- HTML tags are not allowed
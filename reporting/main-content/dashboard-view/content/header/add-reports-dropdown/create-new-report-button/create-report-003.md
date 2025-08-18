**Test Case ID**: TC_CREATE_REPORT_003
**Title**: Report Name Field Validation
**Description**: Verify report name field properties and requirements
**Pre-Condition**: Create Report modal is open
**Test Steps**:
1. Examine Report Name field
2. Test field behavior and validation
**Expected Result**:
- Field label: "Report Name*" (asterisk indicates required)
- Placeholder text: "Enter name"
- Field is empty initially
- Field is required (mandatory for form submission)
- Maximum length: 120 characters
- HTML tags are not allowed in input
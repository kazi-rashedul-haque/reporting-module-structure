# TC_SAVE_AS_NEW_004 - Dashboard Name Field Validation

* **Title**: Dashboard Name Field Validation
* **Description**: Verify dashboard name field properties and requirements in Save as New flow
* **Pre-Condition**: Save as New modal is open
* **Test Steps**:
  * Examine Dashboard Name field
  * Test field behavior and validation rules
* **Expected Result**:
  * Field label: "Dashboard Name*" (asterisk indicates required)
  * Placeholder text: "Enter name"
  * Field is empty initially
  * Field is required (mandatory for form submission)
  * Maximum length: 120 characters
  * HTML tags are not allowed in input
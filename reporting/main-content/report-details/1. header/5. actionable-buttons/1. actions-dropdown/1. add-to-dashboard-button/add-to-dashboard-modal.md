* **Name**: `Add to Dashboard`
* **Modal Trigger**: On click of the `Add to Dashboard` button in the `Actions` dropdown of the report details header.

Search: textbox
Placeholder: Search
Invalid Input: No options to show
Valid Input: Search by dashboard name
No validation is found in the code.
Close_button

**Report List**:
- List of reports with checkboxes
- Checkbox: Select reports to add. The number of selected reports will be displayed in the `Add to Dashboard` button.
- HTML validation: Must not contain HTML tags

**Actionable Buttons**:
- **Cancel** button: 
  - Label: `Cancel`
  - Action: Closes the modal without making any changes.
  - Disabled state: Not applicable, always enabled.
- **Add to Dashboard** button: 
  - Label: `Add to Dashboard`
  - Action: Adds the selected reports to the specified dashboard.
  - Disabled state: If no reports are selected, the button is disabled.
- **Close** button: 
  - Label: `Close`
  - Action: Closes the modal without saving changes.
  - Disabled state: Not applicable, always enabled.
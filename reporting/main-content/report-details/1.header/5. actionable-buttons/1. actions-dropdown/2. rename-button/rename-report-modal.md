* **Name**: `Rename Report`
* **Modal Trigger**: On click of the `Rename` button in the `Actions` dropdown of the report details header.
* **Available for**: User-created reports only (not system-generated reports).

**Report Name*** textbox:
* Placeholder: Enter name
* Required: true
* Max length: 120 characters
* HTML validation: Must not contain HTML tags

Description textarea:
* Placeholder: Write description
* Required: false
* Max length: 240 characters
* HTML validation: Must not contain HTML tags

Actionable Buttons:
- **Cancel** button:
    - Label: `Cancel`
    - Action: Closes the modal without making any changes.
    - Disabled state: Not applicable, always enabled.
- **Save Changes** button:
    - Label: `Save changes`
    - Action: Saves the new report name and description.
    - Disabled state: Enabled only when the report name is valid (not empty, no HTML tags, within max length).
    - Shows loading state while saving.
- **Close** button:
    - Label: `Close`
    - Action: Closes the modal without saving changes.
    - Disabled state: Not applicable, always enabled.
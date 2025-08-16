* **Name**: Delete Report
* **Modal Trigger**: On click of the `Delete` button in the `Actions` dropdown of the report details header.
* **Available for**: User-created reports only (not system-generated reports).

**Message**: `Are you sure you want to delete '<report_name>'?`

**Actionable Buttons**:
- **Cancel** button:
    - Label: `Cancel`
    - Action: Closes the modal without making any changes.
    - Disabled state: Not applicable, always enabled.
- **Delete** button:
    - Label: `Delete`
    - Action: Deletes the report.
    - Disabled state: Enabled only when the report is user-created and not system-generated.
    - Shows loading state while deleting.
- **Close** button:
    - Label: `Close`
    - Action: Closes the modal without saving changes.
    - Disabled state: Not applicable, always enabled.
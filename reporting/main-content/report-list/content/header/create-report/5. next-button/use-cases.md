### Positive:
* Proceeds to Report Configuration page with valid Report Name (and optionally Description).
* Works at min/max character boundaries.

### Negative:
* Next is disabled or shows error with invalid Report Name (empty, whitespace, too long, etc.).
* Attempt to proceed with too long Description.
* Tries to submit duplicate Report Name (if handled here).
* Attempts submission with malicious input (HTML/JS).

### Edge:
* Rapid/multiple clicks: only one submission processed.
* Keyboard navigation/Enter key triggers Next.
* Only Report Name filled, Description empty.
* Both fields at max length, click Next.
# Verify security validation against HTML and script injection

## Test Case ID
TC_ReportName_007

## Description
Verify that the system properly sanitizes and validates against HTML tags and JavaScript injection attempts in the report name field.

## Pre-conditions
- User is logged in
- User is on the Reports page
- Create Report modal is open

## Test Steps
1. Click on the Report Name field
2. Enter HTML tags (e.g., `<script>alert('test')</script>`)
3. Enter common XSS payloads
4. Enter HTML formatting tags
5. Verify system behavior (sanitization, rejection, or escaping)
6. Attempt to proceed with Next button

## Expected Results
- System should either:
  - Sanitize/escape HTML tags and scripts
  - Reject input containing HTML/scripts with error message
  - Strip HTML tags and keep only text content
- No script execution should occur
- Security measures should prevent XSS attacks

## Test Data
- Script injection: `<script>alert('XSS')</script>`
- HTML tags: `<div>Test</div>`
- Image tag: `<img src=x onerror=alert('XSS')>`
- Link injection: `<a href="javascript:alert('XSS')">Test</a>`

## Priority
High
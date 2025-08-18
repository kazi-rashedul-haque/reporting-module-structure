**Title**: Special Characters in Dashboard Name

**Description**: Verify modal handles special characters in dashboard names

**Pre-Condition**: Dashboard with special characters (&, <, >, ", ')

**Test Steps**:
1. Open delete modal for dashboard with special characters

**Expected Result**:
- Special characters are properly escaped/displayed
- No HTML injection occurs
- Modal remains functional
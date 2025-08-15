Use playwright mcp to:
- Open browser to w1.t1.ideascale.dev
- Log in with admin credentials:
    - Email: superuser@ideascale.me
    - Password: brewski01

Navigate to: Reporting page
Select the Reports table existing any report to open report details page
Target directory:/$ARGUMENTS

Analyze Content
- Read the use-cases.md file content
- Examine corresponding UI elements
- Review existing test files for patterns and conventions

Create Test Structure
- Create testcases folder inside each leaf folder
- Folder naming convention: {leaf-folder-name}-testcases

Generate Test Files
- Write test cases as individual .md files
- File naming: Title should match test case name
- Follow established testing patterns and conventions

Example Test Case Structure
**Title:** Verify Created by column sorting functionality in descending order.

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reports page.
3. Click on the "Created by" column header once to sort ascending.
4. Click on the "Created by" column header again to sort descending.
5. Verify the sort indicator changes to show descending order (down arrow).
6. Examine the order of reports in the table.
7. Verify the reports are sorted in reverse alphabetical order.

**Expected Result:**
* The Created by column should sort reports in descending alphabetical order when clicked twice.
* Display the correct sort indicator (down arrow).
* Reverse the alphabetical order from the ascending sort.


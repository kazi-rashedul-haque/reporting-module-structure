Use playwright mcp to:
- Open browser to w1.t1.ideascale.dev
- Log in with admin credentials:
    - Email: superuser@ideascale.me
    - Password: brewski01

Navigate to: Reporting page
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
- Title: Verify Sidebar does not collapse if the button is disabled
- Test Steps:
  1. Login to the workspace as an authenticated user.
  2. Navigate to the Reports page.
  3. Click the collapse sidebar button when it is disabled.

- Expected Result:
  The collapse button should not function when it is disabled.


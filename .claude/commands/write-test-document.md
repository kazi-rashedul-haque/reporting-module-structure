Use playwright mcp to open a browser to w1.t1.ideascale.dev
Log in using the admin credentials:
Email: superuser@ideascale.me
Password: brewski01
Navigate to the Reporting page.
The report list is located at the path:
reporting-module-structure/reporting/$ARGUMENTS
Each leaf folder in this path contains a use-cases.md file.
Based on:
The use-cases.md content and The corresponding UI elements of that leaf
Create a testcases folder inside each leaf folder.
In each testcases folder: the testcase folder name is the last leaf folder name-testcases
Write all test cases as .md files.
The title of each .md file should match the test case name.
please existing test files to understand your testing patterns and conventions
i want the testcases for favorite-column 
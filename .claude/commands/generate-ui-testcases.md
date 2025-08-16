## Purpose
Generate manual UI test cases that will later be converted to automated Playwright tests with TypeScript.

## Process Overview
Use playwright mcp to:
- Open browser to w1.t1.ideascale.dev
- Log in with admin credentials:
    - Email: superuser@ideascale.me
    - Password: brewski01

Navigate to: Reporting page
Select the Reports table existing any report to open report details page
Target directory:/$ARGUMENTS

## Analysis Phase
- Read the use-cases.md file content
- Examine corresponding UI elements
- Review existing test files for patterns and conventions

## Test Structure Creation
- Create testcases folder inside each leaf folder
- Folder naming convention: {leaf-folder-name}-testcases

## Manual Test Case Generation
- Write test cases as individual .md files
- File naming: Title should match test case name
- Follow established testing patterns and conventions
- Generate comprehensive manual test cases that can be easily converted to automated Playwright tests

## Playwright Compatibility Guidelines
When writing manual test cases, consider Playwright automation capabilities:

### Fully Supported in Playwright
- Click, type, hover, keyboard interactions
- Element visibility, text content, attribute verification
- Page navigation, URL verification
- Screenshot capture and visual comparisons
- Network request/response interception
- Local storage, session storage, cookies
- Basic accessibility testing (axe-core integration)
- Form interactions, file uploads
- Drag and drop operations
- Multi-tab/window handling

### Limited or Not Supported - Use Alternatives
- **File downloads**: [Not supported in Playwright – use API validation or mock downloads]
- **OS-level dialogs**: [Not supported in Playwright – use browser dialog handling or mock]
- **Email verification**: [Not supported in Playwright – use API validation or mock email service]
- **SMS/Phone verification**: [Not supported in Playwright – use API validation or mock]
- **External system integrations**: [Not supported in Playwright – use API mocking or stubs]
- **Browser notifications**: [Limited support – use page.on('dialog') or mock notifications]
- **Camera/microphone access**: [Not supported in Playwright – use mock media or skip step]
- **Print dialogs**: [Not supported in Playwright – use CSS media queries or mock]
- **Third-party authentication popups**: [Limited support – use token-based auth or mock]

### Alternative Approaches
- **API Validation**: Verify backend endpoints directly instead of UI interactions
- **Mocking**: Use Playwright's route interception to mock external services
- **Manual Verification**: Mark steps for manual execution during test runs
- **Environment Setup**: Pre-configure test data through APIs or database seeding

## Example Test Case Structures
The test cases rewritten in a simple, easy-to-read way so anyone (QA, Dev, or Business user) can easily understand.
### Standard Functional Test Case
**Title:** Verify Created by column sorting functionality in descending order.

**Pre-conditions:**
* At least one report exists in the report list

**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reporting page.
3. Click on the "Created by" column header once to sort ascending.
4. Click on the "Created by" column header again to sort descending.
5. Verify the sort indicator changes to show descending order (down arrow).
6. Examine the order of reports in the table.
7. Verify the reports are sorted in reverse alphabetical order.

**Expected Result:**
* The Created by column should sort reports in descending alphabetical order when clicked twice.
* Display the correct sort indicator (down arrow).
* Reverse the alphabetical order from the ascending sort.

### Accessibility Test Case Format
**Title:** Verify **Accessibility** compliance in [Component/Feature Name]

---

**Preconditions:**
- Specific setup requirements for the feature
- Screen reader software is available (NVDA, JAWS, or VoiceOver)
- Browser supports keyboard navigation and accessibility features

---

**Test Steps:**
1. Login to the **Workspace** as **authenticated user**.
2. Navigate to the specific page/feature.
3. Press the `Tab` key repeatedly to navigate through all interactive elements.
4. Press `Shift + Tab` to navigate backward through the elements.
5. Press `Enter` and `Space` on interactive elements to verify activation behavior.
6. Enable **screen reader** and verify content is properly announced.
7. Use browser **developer tools** to inspect ARIA labels and semantic markup.
8. Test **color contrast** ratios for all text and icons.
9. Test the section at **200% zoom level** for readability.
10. Switch to **mobile view** and verify touch target sizing.
11. Test with **high contrast mode** enabled.

---

**Expected Result:**
- Each `Tab` key press moves focus in a logical order:
    1. [List specific tab order]
    2. [Next element]
    3. [Continue...]
- `Shift + Tab` navigates in reverse order correctly.
- Interactive elements can be activated with both `Enter` and `Space` keys.
- **Screen reader** properly announces all content and states.
- **ARIA compliance**: Proper labels, roles, and semantic markup.
- **Visual accessibility**: WCAG AA color contrast ratios (4.5:1 text, 3:1 graphics).
- **Mobile accessibility**: Touch targets meet 44x44 pixel minimum.
- **Focus management**: Clear focus indicators and logical navigation.
- No accessibility violations when tested with automated tools.

## Test Case Writing Rules

### Step Classification
When writing test steps, classify each step:
1. **Playwright Supported**: Keep step as written
2. **Playwright Limited**: Provide alternative approach
3. **Not Supported**: Mark with `[Not supported in Playwright – use alternative]`

### Writing Guidelines
- Use specific, identifiable element descriptions (buttons, links, inputs)
- Include clear verification points for assertions
- Specify expected visual states and text content
- Consider data-testid attributes or unique selectors for elements
- **Always include comprehensive accessibility testing** using the dedicated accessibility test case format
- Structure test steps to be modular and reusable
- Mark unsupported steps clearly with alternatives
- Ensure final output is well-structured and directly usable for automation
- **Simplify preconditions** - Remove redundant access requirements
- **Simplify navigation steps** - Use "Navigate to [Page]" instead of detailed app navigation

### Example of Playwright Compatibility Annotations
```markdown
**Test Steps:**
1. Login to the workspace as an authenticated user.
2. Navigate to the Reporting page.
3. Click on the "Export" button.
4. Select "PDF" from the export options.
5. Verify file is downloaded to default directory. [Not supported in Playwright – use API validation or mock download]
6. Open downloaded file and verify content. [Not supported in Playwright – use API response validation]
```

### Quality Checklist
- [ ] All test steps are clearly written
- [ ] Unsupported Playwright steps are marked with alternatives
- [ ] Expected results are programmatically verifiable
- [ ] Test case can be executed manually
- [ ] Test case provides clear automation guidance
- [ ] **Accessibility test case included** following the structured format with horizontal rules
- [ ] **Preconditions simplified** without redundant access statements
- [ ] **Navigation steps simplified** to essential actions only
- [ ] Test cases cover both positive and negative scenarios
- [ ] File naming matches test case titles for easy identification


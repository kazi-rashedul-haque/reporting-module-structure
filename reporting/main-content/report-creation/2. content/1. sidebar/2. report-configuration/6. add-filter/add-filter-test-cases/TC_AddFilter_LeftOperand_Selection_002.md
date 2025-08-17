# TC_AddFilter_LeftOperand_Selection_002

## Title:
Verify left operand dropdown displays all available filter categories and options

## Pre-Condition:
1. User is logged into the reporting application
2. User is on the report creation page with completed basic configuration
3. Add Filter modal is open
4. Filter form is visible with WHERE condition

## Test Steps:
1. Click on the left operand dropdown (showing "Select")
2. Observe the dropdown options that appear
3. Verify all category groups are present
4. Verify options within each category
5. Select different operands from different categories
6. Observe the behavior after each selection

## Expected Results:
1. Left operand dropdown expands showing all 59 available options
2. Options are properly grouped by categories:
   - WORKSPACE: Workspace Group
   - COMMUNITY: Community, Community Name, Community Group
   - IDEA PROPERTIES: Idea, Idea Number, Idea Title, Idea Description, Idea Submission Date, Labels
   - IDEA OWNER: Owner, Owner Email, Owner Source, Owner Registration Date, Owner Status, Owner Profile Language
   - IDEA SUBMITTER: Submitter, Submitter Email, Submitter Source, Submitter Registration Date, Submitter Status, Submitter Profile Language
   - STAGE PROPERTIES: Stage, Stage Name, Stage Description, Stage Function, Funnel
   - CAMPAIGN PROPERTIES: Campaign, Campaign Group, Campaign Title, Campaign Subtitle, Question/Challenge Statement, Campaign Start Date, Campaign End Date, Campaign Privacy, Campaign Language, Idea Submission Start Date, Idea Submission End Date
   - ENGAGEMENTS: Idea Submitted, Idea Views, Idea Votes, Idea Shares, Idea Comments, Idea Up Votes, Idea Down Votes, Comment Votes, Comment Up Votes, Comment Down Votes, Kudos Given, Tag Usage, Engagement Actions, Review Completed, Assessments Completed, Estimation Completed, Refinement Submitted, Fund Allocations
   - IDEA CUSTOM FIELDS: Single Choice, Multiple Choice
3. Each option has appropriate icon and label
4. Selecting an option updates the left operand field
5. Dropdown closes after selection
6. Screen reader announces the selected option
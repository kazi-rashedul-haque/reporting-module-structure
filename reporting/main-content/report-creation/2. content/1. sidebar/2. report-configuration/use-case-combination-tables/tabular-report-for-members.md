| Scenario ID | Data Category | Time Frame | Data Grouping   | Dataset            | Expected Result                                                        | Remarks                 |
|-------------|---------------|------------|-----------------|--------------------|------------------------------------------------------------------------|-------------------------|
| S1          | Members       | All Times  | Time Properties | Total Members      | Total Members table is shown. Drilldown shows the correct member list. |                         |
| S2          | Members       | All Times  | Member Email    | Total Members      | Total Members grouped by email. Drilldown details match summary.       |                         |
| S3          | Members       | All Times  | Member Status   | Total Members      | Total Members grouped by status. Drilldown matches.                    |                         |
| S4          | Members       | All Times  | Campaign        | Total Members      | Total Members by campaign. Drilldown works.                            |                         |
| S5          | Members       | All Times  | Community Group | Total Members      | Community group summary shown. Drilldown works.                        |                         |
| S6          | Members       | All Times  | Workspace Group | Total Members      | Workspace group summary shown. Drilldown works.                        |                         |
| S7          | Members       | All Times  | Time Properties | Engaged Members    | Engaged members listed per time period. Drilldown verified.            |                         |
| S8          | Members       | All Times  | Member Email    | Engaged Members    | Email-wise engaged members listed with drilldown.                      |                         |
| S9          | Members       | All Times  | Member Status   | Engaged Members    | Engaged members grouped by status. Drilldown matches.                  |                         |
| S10         | Members       | All Times  | Campaign        | Engaged Members    | Engaged members shown by campaign. Drilldown verified.                 |                         |
| S11         | Members       | All Times  | Community Group | Engaged Members    | Community group-wise engagement is shown.                              |                         |
| S12         | Members       | All Times  | Workspace Group | Engaged Members    | Engaged members shown per workspace group.                             |                         |
| S13         | Members       | All Times  | Time Properties | New Members        | Time-based new member count shown.                                     |                         |
| S14         | Members       | All Times  | Member Email    | New Members        | New members grouped by email. Drilldown matches.                       |                         |
| S15         | Members       | All Times  | Member Status   | New Members        | New members grouped by status.                                         |                         |
| S16         | Members       | All Times  | Campaign        | New Members        | ‘N/A’ or empty result shown. No crash.                                 |                         |
| S17         | Members       | All Times  | Community Group | New Members        | Community-wise new members displayed.                                  |                         |
| S18         | Members       | All Times  | Workspace Group | New Members        | Workspace-wise new member count shown.                                 |                         |
| S19         | Members       | All Times  | Time Properties | Total Logins       | Shows login count with drilldown to date, name, email                  |                         |
| S20         | Members       | All Times  | Member Email    | Total Logins       | Shows login counts grouped by email                                    |                         |
| S21         | Members       | All Times  | Member Status   | Total Logins       | Status-wise logins displayed with date, name, and email drilldown      |                         |
| S22         | Members       | All Times  | Campaign        | Total Logins       | 'N/A' or feature not available                                         |                         |
| S23         | Members       | All Times  | Community Group | Total Logins       | Community group-wise login count with full drilldown                   |                         |
| S24         | Members       | All Times  | Workspace Group | Total Logins       | Workspace-wise login count and drilldown validated                     |                         |
| S25         | Members       | All Times  | Time Properties | Unique Login Count | Unique users shown with member reg. date, name, email                  |                         |
| S26         | Members       | All Times  | Member Email    | Unique Login Count | 'N/A' or not available                                                 |                         |
| S27         | Members       | All Times  | Member Status   | Unique Login Count | Displays correct unique count with drilldown                           |                         |
| S28         | Members       | All Times  | Campaign        | Unique Login Count | N/A result or feature disabled                                         |                         |
| S29         | Members       | All Times  | Community Group | Unique Login Count | Community-wise unique logins with full drilldown                       |                         |
| S30         | Members       | All Times  | Workspace Group | Unique Login Count | Workspace-wise unique logins with drilldown                            |                         |
| S31         | Members       | All Times  | Time Properties | Total Visit Count  | Shows visitor count with full drilldown                                | Activity count mismatch |
| S32         | Members       | All Times  | Member Email    | Total Visit Count  | Displays visit count per email with name/date/email                    |                         |
| S33         | Members       | All Times  | Member Status   | Total Visit Count  | Correct drilldown of visit counts                                      | Skip                    |
| S34         | Members       | All Times  | Campaign        | Total Visit Count  | Campaign-wise visits shown and validated                               |                         |
| S35         | Members       | All Times  | Community Group | Total Visit Count  | Visit count grouped by community with drilldown                        |                         |
| S36         | Members       | All Times  | Workspace Group | Total Visit Count  | Visit count per workspace group shown                                  | Activity count mismatch |
| S37         | Members       | All Times  | Time Properties | Unique Visit Count | Unique visit counts shown per period                                   | Activity count mismatch |
| S38         | Members       | All Times  | Member Email    | Unique Visit Count | Email-based unique visitors shown                                      |                         |
| S39         | Members       | All Times  | Member Status   | Unique Visit Count | Status-wise unique visitor count with drilldown                        |                         |
| S40         | Members       | All Times  | Campaign        | Unique Visit Count | Shows unique visits for campaign correctly                             |                         |
| S41         | Members       | All Times  | Community Group | Unique Visit Count | Displays community group unique visits                                 |                         |
| S42         | Members       | All Times  | Workspace Group | Unique Visit Count | Displays unique visit counts per workspace group                       |                         |
| S43         | Members       | All Times  | Time Properties | Kudos Given        | Kudos count per time shown with drilldown                              | Activity count mismatch |
| S44         | Members       | All Times  | Member Email    | Kudos Given        | Shows email-wise kudos count with name and date                        | Skip                    |
| S45         | Members       | All Times  | Member Status   | Kudos Given        | Shows kudos by status with details                                     | Skip                    |
| S46         | Members       | All Times  | Campaign        | Kudos Given        | Campaign-wise kudos count validated                                    |                         |
| S47         | Members       | All Times  | Community Group | Kudos Given        | Kudos per community with drilldown                                     | Skip                    |
| S48         | Members       | All Times  | Workspace Group | Kudos Given        | Workspace-wise kudos count shown and drilldown validated               |                         |


# Design Parameters and Process Variables

## Overview
With the final dataset established, we proceeded to the next step in ASD, defining the **Design Parameters (DP)** of the problem. 
We developed a descriptive model built primarily on data visualization, with each created visual referencing one or more columns 
in the final dataset. Columns and respective visuals would target one or more RQs, and because of the mapping shown earlier in 
Figure 8, they would contribute to the satisfaction of one or more Functional Requirements (FR).

Because of their direct influence on FR, the columns in the final dataset represented the **DP** of this problem, with the visuals, 
later collated into a Tableau dashboard, acting as the **Process Variables (PV)**. The completed ASD process is depicted in Figure 13.

## Mapping Columns to Research Questions (RQs)
### Columns and Functional Requirements (FRs)
To assert the mapping between the functional and physical domains, we created a link between every column and the RQ it helps 
answer. For brevity, the columns were renamed as per Table 8.

**Renamed Data Columns**

| Column Name                     | Abbreviation |
|---------------------------------|--------------|
| Course Name                     | C1           |
| Academic?                       | C2           |
| Conforming?                     | C3           |
| Semester by Date                | C4           |
| Semester by Type                | C5           |
| Course ID                       | C6           |
| Date                            | C7           |
| USER ID                         | C8           |
| Anon_USER_ID                    | C9           |
| Username                        | C10          |
| Faculty/Staff                   | C11          |
| Sub-subaccount                  | C12          |
| Subaccount                      | C13          |
| Total Errors                    | C14          |
| brokenLink                      | C15          |
| aMustContainText                | C16          |
| imgAltIsDifferent               | C17          |
| imgAltIsTooLong                 | C18          |
| imgAltNotEmptyInAnchor          | C19          |
| imgHasAltDeco                   | C20          |
| tableDataShouldHaveTh           | C21          |
| tableThShouldHaveScope          | C22          |
| cssTextHasContrast              | C23          |
| headersHaveText                 | C24          |
| videosEmbeddedOrLinkedNeedCaptions | C25      |
| headingLevelSkipped             | C26          |
| fontIsNotUsed                   | C27          |
| videoProvidesCaptions           | C28          |
| Announcements?                  | C29          |
| Assignments?                    | C30          |
| Discussions?                    | C31          |
| Files?                          | C32          |
| Pages?                          | C33          |
| Syllabus?                       | C34          |
| Module URLs?                    | C35          |

### Column Contribution to RQs
To complete the mapping, columns were examined individually to weigh their contribution to each RQ. This process is expounded below:

- **C1/C6:** Course identity is used in conjunction with date, user, and total errors to examine whether a user scanning the same 
course multiple times is remediating errors, which has direct influence on RQ4.

- **C2-C5:** These columns are directly linked with RQ1.

- **C7:** This column is directly linked with RQ1 and, like C1 and C6, with RQ4.

- **C8-C10:** These columns affect RQ4, as explained in C1. Moreover, they are imperative for answering RQ5 and RQ6, seeing as 
training targets user behavior.

- **C11:** Distinction between faculty and staff affects both RQ4 and RQ5. Further, because training is given to both faculty and staff, 
areas of improvement should target both. Thus, RQ6 is also influenced by C11.

- **C12-C13:** These columns have a direct influence on RQ2.

- **C14:** This column is linked to RQ4 as mentioned in C1 and to RQ6 in terms of understanding users’ use of the tool.

- **C15-C28:** These columns have a straightforward link to RQ3. Moreover, more frequent errors can be targeted in training, so the 
columns could affect RQ6.

- **C29-C35:** These columns affect RQ6; understanding areas being scanned by users could give insight into the effects of training.

**The FR hierarchy with completed mapping is shown in Figure below**

  <img src="https://github.com/HassanBerro05/Accessibility-Tool-Analysis/blob/main/Viz/Figure%2014%20Complete%20FR%20Hierarchy.png" alt="Dbeaver" width="700" height="300">





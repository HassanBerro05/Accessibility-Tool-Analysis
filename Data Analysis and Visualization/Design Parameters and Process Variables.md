
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

  <img src="https://github.com/HassanBerro05/Accessibility-Tool-Analysis/blob/main/Viz/Figure%2014%20Complete%20FR%20Hierarchy.png" alt="Dbeaver" width="500" height="300">

# Data Analysis and Visualization

## RQ1: Frequency of UDOIT Usage Across Semesters

## Semester Mapping
To examine the frequency of UDOIT usage across semesters from Winter 2021 to Winter 2023, we utilized **C7** to assign a semester to each scan. 
By referring to academic calendars provided by UM for the relevant period, we mapped each scan date to its respective semester. 
The mapping process is detailed in Table 9.

**Semester Mapping by Date**

| Semester     | Start Date         | End Date           |
|--------------|--------------------|--------------------|
| Winter 2021  | January 19, 2021   | April 30, 2021     |
| Summer 2021  | May 4, 2021        | August 20, 2021    |
| Fall 2021    | August 30, 2021    | December 20, 2021  |
| Winter 2022  | January 5, 2022    | April 28, 2022     |
| Summer 2022  | May 3, 2022        | August 19, 2022    |
| Fall 2022    | August 29, 2022    | December 19, 2022  |
| Winter 2023  | January 4, 2023    | April 27, 2023     |

Two key considerations for this mapping:
1. The term “Summer” encompasses both Spring half-terms and Spring-Summer terms at UM.
2. Scans executed during inter-semester periods were attributed to the upcoming semester. For example, a scan on December 27, 2022, was assigned to Winter 2023.

## Visualization
Figure 15 shows the number of UDOIT scans by semester. The data reveals:
- The highest number of scans occurred during Winter 2021, closely followed by Summer 2021.
- A significant drop of 55% (from 176 to 80 scans) was observed in Fall 2021.
- The pattern reflects the impact of the COVID-19 pandemic, as semesters before Fall 2021 were entirely online, leading to increased scan usage.

**Figure 15: Time Chart of Errors by Semester**

*(Placeholder for visualization)*

## Adjustments for Course Types
Assigning semesters by dates makes analytical sense but overlooks two unique data features:
1. Courses in the dataset are categorized as **academic** or **non-academic**.
2. Some courses have scans run in semesters that do not match their designated semester.

To address these issues:
- Two new columns were added to the dataset: one identifying whether a course is academic and the other assigning a semester based on course type.
- Non-academic courses were further classified as **conforming** (confined to a single semester) or **non-conforming** (spanning multiple semesters).

**Table 10: Sample Questionable Dates**

| Course Name          | Course ID | Date Run          |
|----------------------|-----------|-------------------|
| EPID 636 001 WN 2020 | 356409    | 4/12/2021 8:23    |
| PUBHLTH 450 001 FA 2020 | 396983 | 4/12/2021 15:56   |
| EPID 633 001 FA 2020 | 378160    | 4/12/2021 15:49   |

**Table 11: Sample (non-)Conforming Courses**

| Course Name               | Course ID | Conforming? | Date           | Semester by Type |
|---------------------------|-----------|-------------|----------------|------------------|
| FoL Online - Winter 2022  | 530239    | Yes         | 1/27/2022 15:00| Winter 2022      |
| Canvas at Michigan        | 200       | No          | 1/6/2022 15:12 | None             |

### Example of Adjustments
- The course "FoL Online - Winter 2022" is conforming and assigned to Winter 2022.
- "Canvas at Michigan," a non-conforming course available year-round, is assigned "None" for Semester by Type.

## Semester Assignment Comparison
To analyze user behavior, we compared semester assignments by date and type. 
- Example: A course offered in Winter 2023 had a scan run on 12/9/2022, which falls in Fall 2022 by date but is assigned to Winter 2023 by type (preparatory scan).

**Table 12: Sample Preparatory Scan**

| Course    | Given Semester | Date Run    | Semester by Date | Semester by Type |
|-----------|----------------|-------------|------------------|------------------|
| ISD 520   | Winter 2023    | 12/9/2022   | Fall 2022        | Winter 2023      |

### Timing of Scans
Figure 17 categorizes scans into three groups: **Before**, **During**, and **After** the semester. 
Key observations:
- Almost half of all scans occurred during the semester in which they were offered.
- Preparatory scans (Before) often occurred within three months before a semester started.
- Retroactive scans (After) were primarily executed to update content for future offerings.

**Figures 18–20: Timing Categories for Scans**

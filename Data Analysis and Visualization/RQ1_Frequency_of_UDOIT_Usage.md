
# RQ1: Frequency of UDOIT Usage Across Semesters

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
#### Figure 1 shows the number of UDOIT scans by semester. The data reveals:
- The highest number of scans occurred during Winter 2021, closely followed by Summer 2021.
- A significant drop of 55% (from 176 to 80 scans) was observed in Fall 2021.
- The pattern reflects the impact of the COVID-19 pandemic, as semesters before Fall 2021 were entirely online, leading to increased scan usage.

<img src="https://github.com/HassanBerro05/Accessibility-Tool-Analysis/blob/main/Viz/Figure%2015.png" alt="Excel Painter" width="500" height="300">

## Adjustments for Course Types
Assigning semesters by dates makes analytical sense but overlooks two unique data features:
1. Courses in the dataset are categorized as **academic** or **non-academic**.
2. Some courses have scans run in semesters that do not match their designated semester.

To address these issues:
- Two new columns were added to the dataset: one identifying whether a course is academic and the other assigning a semester based on course type.
- Non-academic courses were further classified as **conforming** (confined to a single semester) or **non-conforming** (spanning multiple semesters).

**Sample Questionable Dates**

| Course Name          | Course ID | Date Run          |
|----------------------|-----------|-------------------|
| EPID XXXX WN 2020 | 356XXXX    | 4/12/2021 8:23    |
| PUBHLTH XXXX FA 2020 | 396XXXX | 4/12/2021 15:56   |
| EPID XXXX FA 2020 | 378XXXX   | 4/12/2021 15:49   |

**Sample (non-)Conforming Courses**

| Course Name               | Course ID | Conforming? | Date           | Semester by Type |
|---------------------------|-----------|-------------|----------------|------------------|
| FoL XXXX - Winter 2022  | 530XXXX    | Yes         | 1/27/2022 15:00| Winter 2022      |
| Canvas XXXX       | 20XXXX       | No          | 1/6/2022 15:12 | None             |

#### Figure 2 displays the visuals resultant of the scanned data. It highlights:

- Number of scans by course type

- Percentage of total conformity

- Percentage of conformity among non-academic courses

 <img src="https://github.com/HassanBerro05/Accessibility-Tool-Analysis/blob/main/Viz/Figure%2016.png" alt="Excel Painter" width="500" height="300">
 

### We observe that:

- Academic courses outnumber non-academic courses in our dataset.

- Conforming courses are almost four times as abundant as non-conforming courses.

- Among non-academic courses, 38% conform, while the remaining 62% mainly consist of Canvas course templates and self-paced online offerings.
### Example of Adjustments
- The course "FoL XXXX - Winter 2022" is conforming and assigned to Winter 2022.
- "Canvas XXXX," a non-conforming course available year-round, is assigned "None" for Semester by Type.

## Semester Assignment Comparison
To analyze user behavior, we compared semester assignments by date and type. 
- Example: A course offered in Winter 2023 had a scan run on 12/9/2022, which falls in Fall 2022 by date but is assigned to Winter 2023 by type (preparatory scan).

**Sample Preparatory Scan**

| Course    | Given Semester | Date Run    | Semester by Date | Semester by Type |
|-----------|----------------|-------------|------------------|------------------|
| ISD XXXX WN 2023   | Winter 2023    | 12/9/2022   | Fall 2022        | Winter 2023      |

### Timing of Scans
#### Figure 3 categorizes scans into three groups: **Before**, **During**, and **After** the semester. 

 <img src="https://github.com/HassanBerro05/Accessibility-Tool-Analysis/blob/main/Viz/Figure%2017%20UDOIT%20scan%20timing.png" alt="Excel Painter" width="500" height="300">

Key observations:
- Almost half of all scans occurred during the semester in which they were offered.
- Preparatory scans (Before) often occurred within three months before a semester started.
- Retroactive scans (After) were primarily executed to update content for future offerings, since it is usual that instructors give the same course in different semsters.

**We further investigated the three categories shown in Figure 4-6**

**Figure 3 (Before): Most scans occurred within a three-month period before the semester starts, while the previous semester was still in session.**

<img src="https://github.com/HassanBerro05/Accessibility-Tool-Analysis/blob/main/Viz/Figure%2018.png" alt="Excel Painter" width="500" height="300">

**Figure 4 (During): Most scans occurred during the break period between semesters, attributed to the upcoming semester.**

<img src="https://github.com/HassanBerro05/Accessibility-Tool-Analysis/blob/main/Viz/Figure%2019.png" alt="Excel Painter" width="500" height="300">

**Figure 5 (After): Most scans occurred one to six months after a semester ended.**

<img src="https://github.com/HassanBerro05/Accessibility-Tool-Analysis/blob/main/Viz/Figure%2020.png" alt="Excel Painter" width="500" height="300">





---

# Scans and Remediation: RQ4

## Top 10 Scanned Courses (Table 1)

In seeking answers to this RQ, we examined courses for which multiple scans were run and tracked changes in the number of errors resulting from each scan. Out of the 211 unique courses in the dataset, 112 were scanned more than once. The table below shows the top 10 most scanned courses:

| **Course ID** | **Times Scanned** | **Subaccount**                             |
|---------------|-------------------|--------------------------------------------|
| 578XXXX        | 29                | College of LXXXX             |
| 449XXXX        | 24                | U-M HXXXX                       |
| 483XXXX        | 19                | School Of XXXX                          |
| 587XXXX        | 19                | U-M HXXXX                        |
| 486XXXX        | 19                | College of LXXXX            |
| 481XXXX        | 18                | School Of XXXX                          |
| 20XXXX           | 17                | University of Michigan - XXXX       |
| 51XXXX        | 17                | School Of XXXX                          |
| 458XXXX        | 16                | School Of XXXX                          |
| 458XXXX        | 14                | School Of XXXX                          |

## Remediation Results

### Remediation Overview (Figure 1)
For each course identified, we tracked the number of errors for every scan to identify the following:
- Whether errors in a course were remediated by users.
- Whether the same course was scanned by multiple users.
- In the event of remediation, whether remediators happened to be faculty or staff.
- In the event of remediation, whether remediation was complete, i.e., eliminated errors from a course completely.
  
**Figure 1 depicts the results of this process**
  
- **70%** of courses with multiple scans underwent remediation.
- **27%** of courses with multiple scans were associated with scans made by multiple users.
- There were over three times as many **staff remediators** compared to **faculty remediators**.
- Out of all remediated courses, **14 out of 78** were completely remediated (i.e., errors were eliminated entirely).
- **Course Remediation Analysis:** **78 out of 211 courses** (around 37%) were remediated across the dataset.

   <img src="https://github.com/HassanBerro05/Accessibility-Tool-Analysis/blob/main/Viz/Figure%2029.png" alt="Excel Painter" width="900" height="300">


## Remediation by Error Type (Table 2)

The following table outlines the remediation efforts for individual error types in remediated courses.

### Columns:
Columns in the table apply to 78 remediated courses and are explained as follows:
- Total: total number of times an error of this type was detected.
- Complete: total number of times a detected error of this type was eliminated completely.
- Partial: total number of times a detected error of this type was partially remediated.
- No: total number of times a detected error of this type was not remediated.

| **Error**                              | **Total** | **Complete** | **Partial** | **No** |
|----------------------------------------|-----------|--------------|-------------|--------|
| imgAltIsDifferent                      | 62        | 67.74%       | 22.58%      | 9.68%  |
| tableDataShouldHaveTh                  | 61        | 40.98%       | 19.67%      | 39.34% |
| aMustContainText                        | 55        | 52.73%       | 27.27%      | 20.00% |
| cssTextHasContrast                      | 39        | 41.03%       | 33.33%      | 25.64% |
| headersHaveText                         | 32        | 59.38%       | 3.13%       | 37.50% |
| videosEmbeddedOrLinkedNeedCaptions      | 31        | 16.13%       | 6.45%       | 77.42% |
| imgAltIsTooLong                         | 13        | 69.23%       | 0.00%       | 30.77% |
| imgHasAltDeco                           | 11        | 54.55%       | 27.27%      | 18.18% |
| tableThShouldHaveScope                  | 8         | 25.00%       | 0.00%       | 75.00% |
| imgAltNotEmptyInAnchor                  | 7         | 57.14%       | 28.57%      | 14.29% |
| brokenLink                              | 4         | 75.00%       | 0.00%       | 25.00% |
| headingLevelSkipped                     | 4         | 100.00%      | 0.00%       | 0.00%  |
| videoProvidesCaptions                   | 1         | 100.00%      | 0.00%       | 0.00%  |
| fontIsNotUsed                           | 0         | 0.00%        | 0.00%       | 0.00%  |

### Key Insights:

- **imgAltIsDifferent**, **imgAltIsTooLong**, **imgAltNotEmptyInAnchor**, and **imgAltHasDeco** (all belonging to the **Alternative Text for Images** group) were the most frequently **completely remediated** errors.
- **videosEmbeddedOrLinkedNeedCaptions** had a high rate of non-remediation (77.42%), likely due to the difficulty of modifying captions in embedded or linked YouTube videos. This error was remediated only 16.13% of the time.

### Conclusion:

The analysis indicates that users are more comfortable addressing errors related to **alternative text for images**. However, issues like missing **video captions** remain difficult to resolve and may require further focus in future training or tool improvements for better remediation support.

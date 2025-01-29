# Scans and Remediation: RQ4

## Top 10 Scanned Courses (Table 16)

Out of the 211 unique courses in the dataset, 112 were scanned more than once. The table below shows the top 10 most scanned courses:

| **Course ID** | **Times Scanned** | **Subaccount**                             |
|---------------|-------------------|--------------------------------------------|
| 578403        | 29                | College of Lit, Sci, and Arts             |
| 449512        | 24                | U-M Human Resources                        |
| 483250        | 19                | School Of Nursing                          |
| 587659        | 19                | U-M Human Resources                        |
| 486100        | 19                | College of Lit, Sci, and Arts             |
| 481307        | 18                | School Of Nursing                          |
| 200           | 17                | University of Michigan - Ann Arbor        |
| 512759        | 17                | School Of Nursing                          |
| 458665        | 16                | School Of Nursing                          |
| 458670        | 14                | School Of Nursing                          |

## Remediation Results

### Remediation Overview (Figure 29)

We tracked remediation for courses with multiple scans and examined the following:

- **70%** of courses with multiple scans underwent remediation.
- **27%** of courses with multiple scans were associated with scans made by multiple users.
- There were over three times as many **staff remediators** compared to **faculty remediators**.
- Out of all remediated courses, **14 out of 78** were completely remediated (i.e., errors were eliminated entirely).

### Course Remediation Analysis

- **78 out of 211 courses** (around 37%) were remediated across the dataset.
- **Figure 29** depicts the results of remediation efforts, showing the proportion of courses that were remediated, as well as the roles of users involved in the remediation process.

## Remediation by Error Type (Table 17)

The following table outlines the remediation efforts for individual error types in remediated courses:

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

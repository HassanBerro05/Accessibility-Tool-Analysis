# RQ3: Scans and Errors

## Error Statistics

### Descriptive Statistics for Errors (Table 1)

The following table summarizes the descriptive statistics for the total errors detected in the dataset:

| **Total Errors Detected** | **Average Errors per Scan** | **Minimum** | **Mode** | **Median** | **Maximum** |
|---------------------------|-----------------------------|-------------|----------|------------|-------------|
| 52,880                    | 72.34                       | 0           | 0        | 13         | 6,628       |

- **Total Errors Detected**: 52,880
- **Average Errors per Scan**: 72.34
- **Minimum**: 0
- **Mode**: 0
- **Median**: 13
- **Maximum**: 6,628 (appears twice, contributing to over 25% of all errors)

About 89% of all scans in the dataset resulted in at least one error, while 81 scans yielded no errors. The most common outcome is 0 errors, while the maximum number of errors in a single scan is 6,628 and appears twice; those two scans alone contribute to over 25% of all errors detected and will be revisited in an upcoming section.

### Error Frequency by Type

#### Figure 1

 <img src="https://github.com/HassanBerro05/Accessibility-Tool-Analysis/blob/main/Viz/Figure%20255.png" alt="Excel Painter" width="500" height="300">

- **"aMustContainText"** occurred in 414 scans, making it the most frequent error.
- **"tableDataShouldHaveTh"** occurred in 411 scans, ranking as the second most frequent error.

These errors relate to accessibility issues:
- **"aMustContainText"** refers to ambiguous links with no descriptive text, such as "Click Here," which are problematic for screen readers.
- **"tableDataShouldHaveTh"** refers to tables without headers, which are essential for explaining the data in rows and columns.

#### Figure 2

 <img src="https://github.com/HassanBerro05/Accessibility-Tool-Analysis/blob/main/Viz/Figure%2026.png" alt="Excel Painter" width="500" height="300">

This figure shows the total occurrences of each error type, highlighting the discrepancy between errors in terms of total occurrence, with **"imgAltIsDifferent"** being the most frequent.

## Error Grouping

### Grouping Errors by Accessibility Problem Areas 

The errors were grouped into five accessibility problem areas:
1. **Alternative Text for Images** – issues with missing or incorrect alt text for images.
2. **Table Headers** – missing headers for tables.
3. **Links** – ambiguous or missing descriptive text in links.
4. **Page Headers/Text** – issues related to page structure and text color contrast.
5. **Video Captions** – missing or faulty video captions.

#### Figure 3: Errors Grouped by Accessibility Problem Areas

<img src="https://github.com/HassanBerro05/Accessibility-Tool-Analysis/blob/main/Viz/Figure%2027.png" alt="Excel Painter" width="500" height="300">

### Error Group-Level Trends (Figure 4 and Table 2)

#### Figure 28: Errors by Group

The figure below illustrates:
- **"Table Headers"** contributed the largest number of errors, followed by **"Alternative Text for Images"** and **"Page Headers/Text"**.
- **"Video Captions"** had the fewest errors.
 
<img src="https://github.com/HassanBerro05/Accessibility-Tool-Analysis/blob/main/Viz/Figure%2028.png" alt="Excel Painter" width="500" height="300">

#### Table 2: Average Errors by Group

The following table shows the average errors per scan for each group:

| **Group**                       | **Average Errors per Scan** |
|----------------------------------|-----------------------------|
| Table Headers                    | 36.44%                      |
| Alternative Text for Images      | 25.50%                      |
| Page Headers/Text                | 23.78%                      |
| Links                             | 12.52%                      |
| Video Captions                    | 10.53%                      |

- **Table Headers** contributed to 36.44% of the total errors per scan, making it the most error-prone group.
- **Video Captions** had the smallest share, with only 10.53% of the errors.

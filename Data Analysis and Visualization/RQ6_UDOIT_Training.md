# UDOIT Training: RQ6

## Error Frequency and Course Design

In answering this RQ, we leveraged insights from previous RQs and introduced new considerations. A key aspect of this analysis was revisiting **error frequency**, previously discussed in RQ3.  

- **Table 14** revealed an **average of 72.34 errors per scan**, but this figure was skewed by **two extreme values (6,628 errors each)** from an academic course where the same Canvas template was used across two semesters without remediation.
- **Excluding these extreme values**, the average error count per scan drops to **54.35 errors**.

While reduced, this average remains **substantially high**, suggesting that **course design processes may not prioritize accessibility**. This indicates a need for **proactive intervention by ITS**, focusing on:

1. **Incorporating accessibility considerations in course design.**
2. **Raising awareness through targeted training sessions.**
3. **Providing faculty and staff with structured design training.**

## Remediation Trends by Error Group (Table 18)

Our analysis extended to **remediation trends across error groups**, as shown in **Table 18**. Weighted averages were used to **account for variations in occurrence** among error types.

### **Table 18: Remediation in Groups**
| Group                          | Complete | Partial | No Remediation |
|--------------------------------|----------|---------|---------------|
| Alternative Text for Images    | 65.59%   | 20.43%  | 13.98%        |
| Table Headers                  | 39.13%   | 17.39%  | 43.48%        |
| Page Headers/Text              | 52.00%   | 18.67%  | 29.33%        |
| Links                          | 54.24%   | 25.42%  | 20.34%        |
| Video Captions                 | 18.75%   | 6.25%   | 75.00%        |

### **Key Findings**
- **Alternative text errors** had the **highest complete remediation rate (65.59%)** and the **lowest instances of no remediation (13.98%)**.
- **Video captions** were **least likely to be remediated (75% not remediated)**, supporting our earlier conclusion that users tend to **avoid fixing video caption issues**.
- **Table headers** exhibited a **valley-like pattern**, where errors were either **completely remediated or not remediated at all**, with minimal partial remediation. This is critical because the **second most frequent error** belongs to this group.

By focusing on these trends, **ITS can identify gaps in user awareness** and **tailor training programs accordingly**.

## Semi-Automated Remediation (Figure 32)

To further investigate **remediation behavior**, we accessed a **sandbox (test course)** provided by ITS to experiment with UDOIT.

- **Remediation requires manual user intervention**, but some errors can be fixed **directly within the scan output** using a **"U FIX IT!" button** (Figure 32).
- **Errors that allow for one-click fixes** were remediated more often than those requiring **manual intervention**.
- This explains why **alternative text issues were frequently remediated**, as many can be resolved via the **"U FIX IT!" mechanism**.

However, **this is not absolute**. Revisiting **Table 17**, we see that **"headersHaveText"** ranked highly in complete remediation **despite not having a semi-automated fix**.  

To **validate this theory**, **user surveys or interviews** could provide valuable insight into **how training and ease-of-use impact remediation behavior**.

## Faculty vs. Staff Training Needs

We revisited our earlier analysis of **faculty vs. staff participation** in UDOIT scans.  
- **Most users in the dataset are staff, not faculty**.
- **Most remediations were carried out by staff**.

This suggests a **discrepancy in UDOIT training effectiveness between faculty and staff**.  
To **bridge this gap**, ITS could **prioritize faculty training**, ensuring **both groups benefit equally** from training sessions.

## Error Distribution by Canvas Area (Table 19)

Finally, we examined **UDOIT usage across different Canvas areas**.  
- **Table 19** provides a breakdown of **scan frequency, total errors, and average errors per scan** for each Canvas area.

### **Table 19: Scans and Errors by Canvas Area**
| Area           | Times Scanned | Total Errors | Errors per Scan |
|---------------|--------------|-------------|----------------|
| Announcements | 618          | 1,184       | 1.92          |
| Assignments   | 641          | 3,177       | 4.96          |
| Discussions   | 627          | 658         | 1.05          |
| Files         | 604          | 13,159      | 21.79         |
| Pages         | 688          | 34,476      | 50.11         |
| Syllabus      | 614          | 226         | 0.37          |
| Module URLs   | 631          | 0           | 0.00          |

### **Key Insights**
- **Pages have the highest error count**, averaging **50.11 errors per scan**.
- **Files also exhibit a high error rate**, with an average of **21.79 errors per scan**.
- **Announcements, discussions, and syllabus areas** have **relatively low error frequencies**.

These findings suggest that **pages and files require special attention in future training efforts**.  
ITS could implement **Key Performance Indicators (KPIs)** to track **error trends and remediation progress over time**, ensuring training efforts yield tangible improvements.

## Conclusion

RQ6 emphasizes the **importance of targeted UDOIT training** by identifying key areas for improvement:
1. **Enhancing accessibility considerations in course design.**
2. **Prioritizing training on commonly neglected errors (e.g., video captions).**
3. **Utilizing semi-automated remediation tools to encourage user engagement.**
4. **Addressing the faculty-staff training gap.**
5. **Focusing training on high-error Canvas areas (e.g., pages and files).**

By leveraging these insights, **ITS can refine its training strategy, improving accessibility compliance across courses**.

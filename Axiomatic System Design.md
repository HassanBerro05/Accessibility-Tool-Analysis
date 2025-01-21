## **Functional Requirements (FR) and Axiomatic System Design (ASD)**

### **Axiomatic System Design (ASD) Overview**
ASD is a systematic approach for designing systems, focusing on mapping **Customer Needs (CN)** to **Functional Requirements (FR)** and further to **Design Parameters (DP)**. This ensures that each customer need is addressed through actionable system features.  


ASD divides the design process into:
1. **Customer Domain**: Defines customer needs.
2. **Functional Domain**: Specifies requirements to satisfy customer needs.
3. **Physical Domain**: Implements solutions.
4. **Process Domain**: Executes and manages processes.

---

### **Customer Needs (CN)**
| **CN#** | **Customer Need**                                                             |
|---------|-------------------------------------------------------------------------------|
| CN1     | Understanding how UM users interact with UDOIT, i.e., whether they are using the tool and how they are using it.       |
| CN2     | Identifying gaps in usage of the tool, whether by subaccount or by semester.|
| CN3     | Tracking the occurrence of errors in outputs of scans in terms of error frequency and the most abundant errors.          |
| CN4     | Identifying patterns in the usage of UDOIT over time, particularly across semesters. |

---

### **Functional Requirements (FR)**
| **FR#** | **Functional Requirement**                                                   | **Mapped CN** |
|---------|-------------------------------------------------------------------------------|---------------|
| FR1     | User Tracking: the system must be able to identify users using UDOIT and identify their role in a course, i.e., faculty or staff.            | CN1, CN3          |
| FR2     | Subaccount Tracking: the system must be able to identify subaccounts, i.e., colleges or schools pertinent to each UDOIT scan.               | CN2           |
| FR3     | Error Tracking: the system must be able to track the type and quantity of each individual error.  | CN3, CN4          |
| FR4     | Temporal Tracking: the system should be able to track the usage of UDOIT and the occurrence of errors over time, particularly with the procession of the relevant semesters              | CN2, CN4          |

---
<img src="https://raw.githubusercontent.com/HassanBerro05/Accessibility-Tool-Analysis/main/Viz/Figure%201%20Axiomatic%20Design.png" alt="Axiomatic Design">

### **Mapping Research Questions (RQ) to Functional Requirements**
| **RQ** | **Research Question**                                           | **Mapped FR**          |
|--------|-----------------------------------------------------------------|------------------------|
| RQ1    | How has UDOIT usage frequency changed across semesters?         | FR4                   |
| RQ2    | Are there usage patterns across different colleges/schools?     | FR2                   |
| RQ3    | What types of errors are most common?                           | FR3                   |
| RQ4    | Are errors being addressed by faculty and staff?                | FR1, FR3, FR4         |
| RQ5    | Who are the power users (faculty or staff)?                     | FR1                   |
| RQ6    | What are potential improvements in UDOIT training?              | FR1                   |

---

## **UDOIT Overview**

UDOIT is an open-source tool developed by the Center for Distributed Learning (CDL) at the University of Central Florida. It scans Canvas courses to detect accessibility issues and provides recommendations for addressing them.  

### **Features Analyzed by UDOIT**
- Announcements  
- Assignments  
- Discussions  
- Pages  
- Syllabus  
- Module URLs  
- Files (HTML)  

### **Common Accessibility Problem Areas**
- Use of headings in page structure.  
- Alternative text for images.  
- Table headers.  
- Color contrast.  
- Video captions.  

---

### **Error Types Identified by UDOIT**
The following table summarizes the 22 error types detected by UDOIT:

| **Internal Name**                   | **UDOIT Output**                                   |
|-------------------------------------|---------------------------------------------------|
| `imgAltIsDifferent`                 | Alternative text should not be the image filename.|
| `tableDataShouldHaveTh`             | No table headers found.                           |
| `cssTextHasContrast`                | Insufficient text color contrast with background. |
| `videoProvidesCaptions`             | No closed captions found.                         |
| `brokenLink`                        | Broken link detected.                             |

_For a complete list, see the full report in the repository._  

---


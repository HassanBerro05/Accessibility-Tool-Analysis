Scans and Remediation: RQ4

In seeking answers to this RQ, we examined courses for which multiple scans were run and tracked changes in the number of errors resulting from each scan. Out of 211 unique courses in the dataset, 112 were scanned more than once. Table 16 contains information on the 10 most scanned courses.
Table 16

Top 10 Scanned Courses

Course ID	Times Scanned	Subaccount
578403	29	College of Lit, Sci, and Arts
449512	24	U-M Human Resources
483250	19	School Of Nursing
587659	19	U-M Human Resources
486100	19	College of Lit, Sci, and Arts
481307	18	School Of Nursing
200	17	University of Michigan - Ann Arbor
512759	17	School Of Nursing
458665	16	School Of Nursing
458670	14	School Of Nursing


For each course identified, we tracked the number of errors for every scan to identify the following:
-	Whether errors in a course were remediated by users.
 


-	Whether the same course was scanned by multiple users.

-	In the event of remediation, whether remediators happened to be faculty or staff.

-	In the event of remediation, whether remediation was complete, i.e., eliminated errors from a course completely.
Figure 29 depicts the results of this process. Around 70% of all courses with multiple scans underwent remediation. Further, for courses with multiple scans, roughly 27% were associated with scans made by multiple users. The middle visual in Figure 29 examines the identity of users remediating errors. It is revealed that there were over three times as many remediators among staff as among faculty. We also enumerated among all instances of remediation 14 out of 78 complete remediations. Extending our analysis to include all courses, we inferred that 78 out of 211 courses, a little under 37%, were remediated.

Figure 29

Remediation in Courses with Multiple Scans


 


Furthermore, we examined course remediation on an individual error type level; we isolated remediated courses and tracked the frequency of each individual error as scans progressed. Results are demonstrated in Table 17.
 


Table 17

Remediation by Error Type

Error	Total	Complete	Partial	No
imgAltIsDifferent	62	67.74%	22.58%	9.68%
tableDataShouldHaveTh	61	40.98%	19.67%	39.34%
aMustContainText	55	52.73%	27.27%	20.00%
cssTextHasContrast	39	41.03%	33.33%	25.64%
headersHaveText	32	59.38%	3.13%	37.50%
videosEmbeddedOrLinkedNeedCaptions	31	16.13%	6.45%	77.42%
imgAltIsTooLong	13	69.23%	0.00%	30.77%
imgHasAltDeco	11	54.55%	27.27%	18.18%
tableThShouldHaveScope	8	25.00%	0.00%	75.00%
imgAltNotEmptyInAnchor	7	57.14%	28.57%	14.29%
brokenLink	4	75.00%	0.00%	25.00%
headingLevelSkipped	4	100.00%	0.00%	0.00%
videoProvidesCaptions	1	100.00%	0.00%	0.00%
fontIsNotUsed	0	0.00%	0.00%	0.00%


Columns in the table apply to 78 remediated courses and are explained as follows:

-	Total: total number of times an error of this type was detected.

-	Complete: total number of times a detected error of this type was eliminated completely.

-	Partial: total number of times a detected error of this type was partially remediated.

-	No: total number of times a detected error of this type was not remediated.

Results revealed that out of errors that appeared at least 5 times, errors “imgAltIsDifferent”, “imgAltIsTooLong”, “imgAltNotEmptyInAnchor”, and “imgAltHasDeco” were completely remediated most often. Interestingly, all four of those belong to the group “Alternative Text for Images”. We concluded based on those results that UDOIT users seemed to be comfortable or willing to correct issues with alternative text.
The same cannot be said about “videosEmbeddedOrLinkedNeedCaptions”. The self- explanatory error appeared 31 times in remediated courses, 24 out of which it was not remediated. This was not a surprising result; this error detects instances in which a linked video does not contain human-generated captions. Most embedded or linked videos come from YouTube and mostly contain automatically-generated captions, which users cannot modify. Although this issue
 


can be more difficult to remediate, the few times it has been remediated justify isolating it in future UDOIT training offerings.

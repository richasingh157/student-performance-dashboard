Student Performance Dashboard - Power BI Project

 Overview:

This Power BI project visualizes student academic performance across subjects, gender, states, and terms. It helps educators and administrators quickly identify:

  Subject-wise performance trends
  
  Grade distributions

  Regional comparisons

  Top performers

Overall KPIs such as pass rate, average marks, etc.

 Features Included

 Charts:

Clustered Bar Chart: Average marks by subject

Pie Chart: Grade distribution (A+, A, B, C, D, F)

Map : Student distribution across Indian states

Slicers: Class, Gender, State, Exam Term

Top Performer Card

=======Dynamic  Cards:========

  Avg Marks

  Highest Score

  Pass %

  Distinct Students

  States Represented

========== Calculated Measures & DAX:========

Pass % = DIVIDE(COUNT(Passed), COUNT(StudentID))

Selected Class, Selected Gender, etc. using SELECTEDVALUE()

Top performer name with:

Top Performer =
VAR MaxMarks = MAX(student_marks[Marks])
RETURN CALCULATE(MAX(student_marks[Name]),student_marks[Marks] = MaxMarks)

 Filter Debug Table:

Displays current slicer values for Class, Gender, Term, and State



 Styling:

Light purple background

Medal icon for Top Performer card


Center-aligned text and bold titles



student_marks_dataset_200.csv


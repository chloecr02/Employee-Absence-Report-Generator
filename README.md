# Employee-Absence-Report-Generator
Developed a program using file I/O and functions to generate reports on employee absences.

#### Pseudocode
Display the message: "Calculate the average number of days a company's employees are absent."  
Ask user: "Please enter the number of employees in the company"  
Input numberOfEmployees  
  
If numberOfEmployees < 1  
Display the message: "The number of employees must not be negative."  
  
Open output file "employeeAbsences.txt" for the report text  
File displays title: "EMPLOYEE ABSENCE REPORT"  
File displays 2 columns: "EMPLOYEE ID DAYS ABSENT"  
  
For i=1 to numberOfEmployees  
Ask user: "Please enter an employee ID"  
Input: employeeID  
Ask user: "Please enter the number of days this employee was absent"  
Input: daysAbsent  
  
While daysAbsent < 0  
Display: "The number of days must not be negative. Please re-enter."  
Input: daysAbsent  
End While  
  
Add daysAbsent to totalDaysAbsent   
Write to file: employeeID and daysAbsent formatted in columns  
End For  
  
Calculate: averageAbsence = totalDaysAbsent / numberOfEmployees  
  
File displays 2 columns and the data reported by user:  
"Total employees:"numberOfEmployees  
"Total days absent:"totalDaysAbsent  
"Average days absent:"averageAbsence (rounded to 2 decimal places)  
  
Close output file  
Display programmer information 
End Program    

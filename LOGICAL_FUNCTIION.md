🔥 Excel Logical Formulas Master Sheet (With Practical Examples)

Sr.	Formula Type	Syntax	Example	Explanation

1️⃣	IF	=IF(condition, value_if_true, value_if_false)	=IF(A2>60, "Pass", "Fail")	Agar A2 > 60 hai to "Pass" warna "Fail".
2️⃣	AND	=AND(condition1, condition2,...)	=AND(A2>60, B2="Yes")	Dono condition true honi chahiye: A2 > 60 aur B2 = "Yes".
3️⃣	OR	=OR(condition1, condition2,...)	=OR(A2="Cash", A2="Online")	Dono me se ek bhi true ho to result TRUE.
4️⃣	NOT	=NOT(condition)	=NOT(A2>50)	Agar A2 > 50 false hai to TRUE dega.
5️⃣	IF + AND	=IF(AND(A2>60, B2="Yes"), "Eligible", "Not Eligible")	Dono condition sahi ho to "Eligible".	
6️⃣	IF + OR	=IF(OR(A2="Male", B2>30), "Allowed", "Denied")	Kisi bhi ek sahi ho to "Allowed".	
7️⃣	IFS	=IFS(condition1, value1, condition2, value2,...)	=IFS(A2>90, "A+", A2>80, "A", A2>70, "B", TRUE, "Fail")	Multiple condition ke liye. IF ka upgrade.
8️⃣	Nested IF	=IF(A2>90, "A+", IF(A2>80, "A", IF(A2>70, "B", "Fail")))	IF ke andar IF. Flexible grading ke liye.	
9️⃣	IFERROR	=IFERROR(A2/B2, "Error")	Agar error aata hai to "Error" print karega.	
🔟	SWITCH	=SWITCH(A2, "Mon", 1, "Tue", 2, "Wed", 3, "Invalid")	A2 ke value ke hisaab se number assign karta hai.	



---

🎯 Real-life Data Entry Automation Use Case (No Internet Required)

Scenario: Tumhare computer mein net nahi chal raha, lekin tumhare pass Excel aur offline data hai. Tum chaahte ho ki tumhara data entry automatic ho jaye.

👉 Example Table:

Name	Marks	Gender	Result Formula

Ravi	85	Male	=IF(AND(B2>=60, C2="Male"), "Selected", "Not Selected")
Priya	78	Female	=IF(AND(B3>=60, C3="Female"), "Selected", "Not Selected")


🔁 Auto Logic:

Use drop-down (Data Validation)

Use conditional formatting to color "Fail" in red

Use IF to auto-generate result

Use macro to auto-move selected data to "Final List" sheet



---

🧠 Conditional Formatting (with Formula)

Task	Formula	Use

Red color if marks < 33	=$B2<33	Fail highlight
Green if “Selected”	=$D2="Selected"	Passed students
Grey if blank	=ISBLANK(A2)	Highlight empty rows



---

📦 Folder Format for GitHub

📁 Excel-Logic-Formulas
├── 📄 README.md
├── 📊 Logical_Formula_Examples.xlsx
├── 📁 Practical_UseCases
│   ├── 🎓 Student_Result_Auto.xlsx
│   ├── 🧾 Invoice_Status_Logic.xlsx
│   └── 🏢 Employee_Attendance_Auto.xlsx


---

✅ Bonus Tip: Job Interviews के लिए Ready Lines

"I can automate data validation and decision-making using IF, IFS, AND, OR."

"I’ve used conditional formatting with formulas for real-time visual tracking."

"I understand nested logic to build scalable Excel dashboards."



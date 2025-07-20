
📊 Excel: Sort, Filter & Data Validation (Dropdown) – with Sales Data Example

🧾 Dataset Used: Sales Data

Sale Date	Customer Name	City	State	Region	Category	Product	Quantity	Price per Unit	Sales Amount

25-06-2023	Meera	Nagpur	Maharashtra	West	Furniture	Table	6	4016.25	24097.5
01-11-2023	Vihaan	Coimbatore	Tamil Nadu	South	Stationery	Ruler	9	3601.85	32416.65
…	…	…	…	…	…	…	…	…	…



---

🔢 1. Sort (Manual)

📌 Objective:

Sort the sales data by:

Sale Date (Newest to Oldest)

Sales Amount (Largest to Smallest)


🔧 Steps:

1. Select the entire data range (including headers).


2. Go to Data → Sort.


3. Choose column: Sales Amount, Sort: Largest to Smallest.




---

🔍 2. Filter (Manual)

📌 Objective:

Filter only the sales from “Maharashtra” OR Filter for Furniture category.

🔧 Steps:

1. Select the header row.


2. Go to Data → Filter (Shortcut: Ctrl + Shift + L).


3. Click the dropdown in the State column → Select Maharashtra.


4. OR in the Category column → Select Furniture.




---

🔽 3. Data Validation with Drop-down

📌 Objective:

Create a drop-down in a new column (e.g., Order Status) with fixed values like:

Pending

Shipped

Delivered


🔧 Steps:

1. Create a list somewhere (e.g., in Sheet2):

Pending  
Shipped  
Delivered


2. Go to column Order Status in your main sheet.


3. Select the range where you want dropdowns.


4. Click Data → Data Validation.


5. In Allow: Choose List.


6. Source: Select the list from Sheet2.



✅ Now you have a dropdown for each order!


---

🎯 BONUS: Filter with Formula

You can use FILTER function (Excel 365+ only):

=FILTER(A2:J100, D2:D100="Maharashtra")

This will filter only rows where State = Maharashtra dynamically.


---

📁 Suggested File Name for GitHub:



Or if you're maintaining it in a single document:

01_Sort_Filter_Validation_Excel.md


---

📌 Summary Table

Feature	Method	Example

Sort	Manual	Sales Amount Descending
Filter	Manual	State = Maharashtra
Filter	Formula	=FILTER(...) (Excel 365 only)
Drop-down	Data Validation	Status: Pending, Shipped, etc.

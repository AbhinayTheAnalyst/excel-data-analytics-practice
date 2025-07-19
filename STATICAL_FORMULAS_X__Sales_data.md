
📌 Q1: Total Transactions by Each State

🧠 Explanation:

"Transaction" ka matlab hota hai ek row — ek sale. To humein har state me kitni rows hain woh count karna hai.

✅ Formula:

=COUNTIF(E:E, "Maharashtra")

👉 Use dynamic table ke liye:

=COUNTIF(E:E, A2)

📌 Use PivotTable:

Rows: State

Values: Count of State



---

📌 Q2: Total Transactions by State + Product Category

✅ Formula:

=COUNTIFS(E:E, "Maharashtra", F:F, "Furniture")

📌 Use PivotTable:

Rows: State

Columns: Product Category

Values: Count of Product Category



---

📌 Q3: Total Quantity Sold by Region

✅ Formula:

=SUMIF(D:D, "West", H:H)

📌 Use PivotTable:

Rows: Region

Values: Sum of Quantity



---

📌 Q4: Total Quantity Sold by Region + Product Name

✅ Formula:

=SUMIFS(H:H, D:D, "South", G:G, "Table")

📌 Use PivotTable:

Rows: Region

Columns: Product Name

Values: Sum of Quantity



---

📌 Q5: Average Sales Amount by State

✅ Formula:

=AVERAGEIF(E:E, "Maharashtra", J:J)

📌 Use PivotTable:

Rows: State

Values: Average of Sales Amount



---

📌 Q6: Average Sales Amount by State + Product Name

✅ Formula:

=AVERAGEIFS(J:J, E:E, "Maharashtra", G:G, "Table")

📌 Common mistake: If any one of the criteria values doesn't exist, AVERAGEIFS will return #DIV/0!

📌 Use PivotTable:

Rows: State

Columns: Product Name

Values: Average of Sales Amount



---

📌 Q7: Max Sales by Each City

✅ Formula:

=MAXIFS(J:J, C:C, "Nagpur")

📌 Use PivotTable:

Rows: City

Values: Max of Sales Amount


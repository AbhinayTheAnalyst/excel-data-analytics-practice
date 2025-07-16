🧹 Excel Data Cleaning - Real World Practice by Abhinay

## 📌 Objective
Clean raw data using Excel functions and features to ensure accurate analysis.  
🧠 *"Data analysis tabhi kaam karega jab data saaf hoga!"*

---

## 🔧 Tools Used:
- Microsoft Excel (with keyboard shortcuts)
- Formula bar and built-in functions
- Special characters handling

---

## ✅ Topics Covered in Data Cleaning

---

### 1. 🔍 Identify Extra Spaces

Using `=LEN()`:
```excel
=LEN(A2)

Compare length before and after TRIM to identify hidden spaces.


---

2. ✂️ Remove Extra Spaces

A. =TRIM(A2)

Removes leading, trailing and multiple spaces between words.

Name (Before)	LEN	After Trim	LEN

"  golu   "	9	"golu"	4


B. TRIM doesn't work on unbreakable space (CHAR(160))

Use:

=SUBSTITUTE(A2,CHAR(160),"")

To remove such special spaces.


---

3. 🔁 Replace Text with SUBSTITUTE

Example:

=SUBSTITUTE(A2,"go","lo")

Changes “golu” → “lolu”


---

4. 🔤 Standardize Text Format

=PROPER(A2) → Capitalize first letters.

=UPPER(A2) → All uppercase.

=LOWER(A2) → All lowercase.



---

5. 📏 Remove Duplicates

A. Entire Row Duplicates:

Select all data → Go to Data → Click Remove Duplicates


B. Specific Column Duplicates:

Select column only → Data → Remove Duplicates


👉 Tip: Use =COUNTIF(A:A, A2) to check repeated values


---

6. 🧪 Data Validation

Use:

Data → Data Validation → Whole Number → Min: 1000000000 → Max: 9999999999

Restrict values (e.g., only 10-digit mobile numbers)


---

7. ⚡ Flash Fill (Smart Auto-Fill)

Shortcut: Ctrl + E

E.g., If cell A2 has abhi-844114, Flash Fill can split name and ID automatically based on the first pattern you enter.


---

8. 🪓 Text Splitting using LEFT, RIGHT, FIND

Split Name-ID:

=LEFT(A2,FIND("-",A2)-1)    → "abhi"
=RIGHT(A2,LEN(A2)-FIND("-",A2))  → "844114"


---

9. 🧠 Handle Negative Values

Replace negatives with 0:

=IF(A2<0,0,A2)


---

10. 🚨 Delete Empty Rows Using “Go To Special”

Ctrl + G → Go To → Special → Blanks → Ctrl + - → Delete row
(Be careful: blank cells ≠ blank rows)



---

📊 Example Table from My Practice

Name	Age	Salary	Length	After Trim

golu	18	1000000	9	4
radha	12	100	5	5
annm	23	20000	4	4
abhinay	24	232	12	7
kmm	22	3444	3	3
knnmkm	20	1000	6	6


→ =TRIM(), =LEN(), and =COUNTIF() helped me clean this.


---

💬 My Notes:

> Jab maine TRIM ke saath LEN lagakar comparison kiya, tab samjha ki space ki wajah se duplicate dikhta hi nahi.
Flash Fill ka Ctrl + E use karke naam-ID split kiya — real-world mein invoice aur email list banane ke liye useful hai.




---

🧾 Summary Checklist:

[x] Remove spaces: TRIM, SUBSTITUTE

[x] Format text: PROPER, UPPER, LOWER

[x] Remove duplicates

[x] Validate clean input with Data Validation

[x] Split text using LEFT, RIGHT, FIND

[x] Flash Fill

[x] Negative handling: IF()

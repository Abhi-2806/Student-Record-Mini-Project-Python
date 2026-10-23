# 🎓 Student Data Management System (Python Mini-Project)

A lightweight, console-based Python application designed to collect, process, grade, and filter student academic records using native data structures (lists and dictionaries).

---

## 📌 Project Overview

This project serves as a practical implementation of fundamental Python concepts, focusing on interactive user inputs, conditional grading logic, dictionary-based record structuring, and iterative list processing.

### Key Highlights
- **Dynamic Data Ingestion:** Accepts dynamic user input for any arbitrary number of students.
- **Automated Grade Assignment:** Categorizes performance based on tiered percentage cutoffs.
- **Structured In-Memory Storage:** Bundles individual student attributes into dictionaries and maintains them within an overarching records list.
- **Clean Console Reporting:** Displays formatted records line-by-line and extracts passed students meeting the pass threshold ($\ge 33$ marks).

---

## ⚙️ Grading Logic & Rules

The application uses standard conditional branching (`if-elif-else`) to classify scores:

| Marks Range | Assigned Grade | Academic Status |
| :---: | :---: | :---: |
| $> 95$ | **A** | Distinction / Pass |
| $> 80$ and $\le 95$ | **B** | First Class / Pass |
| $> 60$ and $\le 80$ | **C** | Second Class / Pass |
| $\ge 33$ and $\le 60$ | **D** | Third Class / Pass |
| $< 33$ | **F** | Fail |

---

## 🛠️ Concepts & Technologies Used

- **Language:** Python 3.x
- **Data Structures:** 
  - `list`: Stores master collections of student entities (`StudentData = []`).
  - `dict`: Stores key-value mappings for each student (`Name`, `Roll_No`, `Marks`, `Grade`).
- **Control Flow:**
  - `for` loops with `range()` for batch data collection and display formatting.
  - Multi-way branching (`if-elif-else`) for grade mapping and filtering logic.
- **String Manipulation:** Python f-strings for dynamic formatting and tabular console printing.

---

## 📂 Project Structure

```text
student-data-management/
│
├── student_data_manager.py       # Main Python executable script
└── README.md                     # Project documentation
```

---

## 🚀 How to Run the Project

### Prerequisites
Make sure Python 3 is installed on your local machine. You can verify this by running:
```bash
python --version
```

### Execution Steps
1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/student-data-management.git
   cd student-data-management
   ```

2. **Run the script:**
   ```bash
   python student_data_manager.py
   ```

3. **Follow the interactive prompts:**
   - Input the total count of students.
   - Enter each student's `Name`, `Roll_Number`, and `Marks`.

---

## 🖥️ Sample Run & Output

```text
Total Number Of Students: 2

Enter the data of Student: 1
Name: Abhishek
Roll_Number: 101
Marks: 98

Enter the data of Student: 2
Name: Rohan
Roll_Number: 102
Marks: 28

All Students Data: 
 
Name: Abhishek | Roll Number: 101 | Marks: 98 | Grade: A
Name: Rohan | Roll Number: 102 | Marks: 28 | Grade: F

 Students who have Passed: 
Abhishek - Marks: 98 
```

---

## 🔮 Future Enhancements

- [ ] Export compiled student records to CSV or Excel using `pandas`.
- [ ] Add exception handling (`try-except`) for non-integer inputs.
- [ ] Implement search and update functionality by Roll Number.
- [ ] Calculate class summary metrics (average marks, top scorer, pass percentage).

---

## 👤 Author

- **Abhishek Pathak**
- **GitHub:** [@Abhi-2806](https://github.com/Abhi-2806)
- **LinkedIn:** [Abhishek Pathak](https://www.linkedin.com/in/abhishekpathak2806/)
# 📌 Project Proposal (Draft)

## 📝 Project Title  
### Student Login Project

---

## 🔍 Problem Statement  

- Students who arrive late or return after an absence often do not know if they need an admission slip before entering class. Checking this manually creates confusion and forces students to line up at school offices just to verify their status.
---

## 🎯 Project Objectives  
- Objective 1: Automate Real-Time Arrival Verification — To develop a Python login program that captures a student's name and current arrival timestamp, evaluating whether they are Too Early (before 5:00 AM), On Time (5:00 AM – 7:30 AM), or Tardy (after 7:30 AM, requiring an admission slip).

- Objective 2: Streamline Morning Entry & Reduce Delays — To provide students with instant, clear feedback upon arrival so tardy students can immediately secure an admission slip before disrupting ongoing classes.

- Objective 3: Apply Core Python Programming Concepts — To practice essential Python skills—including functions (def), string formatting (.strip(), .title()), real-time datetime handling, and conditional logic (if/elif/else)—to solve a practical school problem.


---

## ⚙️ Planned Features  
- `Feature 1: Student Identification & Name Formatting`
Prompts the student for their first and last name, automatically cleaning up extra spaces (.strip()) and capitalizing initials (.title()) for a neat, standardized login record.
- `Feature 2: Real-Time Arrival & Admission Slip Check`
Captures the exact date and system time (datetime) upon login and compares it against the school's schedule (5:00 AM opening and 7:30 AM late cut-off) to immediately display whether the student is Too Early, On Time, or Tardy (Admission Slip Required).
- `feature 3: Absence History Prompt`
Asks the student if they were absent during the previous school day—if they answer "Yes," the system automatically flags them to get an admission slip even if they arrived before 7:30 AM.
- `Feature 4: Continuous Multi-Student Login Loop`
Allows multiple students to log in one after another during the morning rush without having to restart the Python program every time, with an option for staff to exit when classes begin.
- `Feature 5: Daily Login & Tardy Summary Counter`
Tracks and displays a summary at the end of the session showing the total number of students who logged in, how many were On Time, and how many required an Admission Slip.


---

## ⌨️ Planned Inputs and Outputs  

- **Inputs**  
  - What kind of data will the user provide (if any)?  
  - Example: student ID, date range, product name  

- **Outputs**  
  - What kind of results will your program display?  
  - Example: class averages, top products, weather summary  

---

## 🧠 Logic Plan  
Describe your program’s logic:  

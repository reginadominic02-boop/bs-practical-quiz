Project Title : Mini Rule-Based Knowledge-Based System for Campus Access

Description
This project implements a simple rule-based Knowledge-Based System (KBS) using forward chaining.
The system evaluates campus access eligibility based on predefined facts and rules related to student verification, registration, financial clearance, and safety checks.

How to Run
step 1: Open kbs_quiz.ipynb
step 2: Run all cells
step 3: View inferred facts and final decision

Facts Used: 
has_student_id
fees_cleared
registered_for_semester
security_check_passed

Rules (IF–THEN)
IF has_student_id THEN identity_verified
IF security_check_passed THEN safe_to_enter
IF identity_verified AND registered_for_semester THEN active_student
IF active_student AND fees_cleared THEN financially_cleared
IF financially_cleared AND safe_to_enter THEN entry_granted

Final Decision Logic
If the fact "entry_granted" exists after inference → ENTRY GRANTED.
Otherwise → ENTRY DENIED.

Student Details
Name: Regina Dominic
Reg Number: 670709

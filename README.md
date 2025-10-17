# Assessment3_Hussam

Project Title: Requisition System
Overview

This repository contains my own Python project called Requisition System, created as part of my IT5016 course.
The program allows staff to submit requisitions with dates, staff ID, and staff names, enter multiple items for each requisition, and automatically approve requests with totals less than $500.
Managers can also review pending requisitions and change their status to Approved, Not approved, or Pending.
Finally, the program displays all requisition information and summary statistics.

Code Collection

This repository includes:

My own original Python code – requisitionsystem.py (also attached as Assignment 1).

Practice and inspired code – simple examples I studied to improve my understanding of Python classes and object-oriented programming.

Commentary and analysis – explanation of how software design principles are demonstrated in my code.

Programming Principles and Concepts Applied
1. Modularity

Each part of the program is divided into logical sections:

The class RequisitionSystem handles all operations related to requisitions.

Methods like staff_info(), requisitions_details(), and display_requisition() each have a single clear purpose.

This modular design makes the program easy to maintain and extend, as new features (such as saving to a file) can be added without rewriting existing code.

2. Object-Oriented Programming (OOP)

The project follows the OOP approach:

A class (RequisitionSystem) was created to represent each requisition and its details.

Encapsulation: All data related to each requisition (date, staff info, items, totals, and status) is stored inside the class.

Methods handle specific operations like approval, statistics, and displaying details.

OOP makes the code more organized and reusable.

3. Single Responsibility Principle (SRP)

Each function in the code performs only one responsibility:

staff_info() only collects staff information.

requisitions_details() only gathers items and calculates the total.

requisition_approval() only handles the automatic approval condition.

respond_requisition() only manages manager decisions.

This structure helps ensure clarity and reduces the chance of introducing errors during updates.

4. Readability and Maintainability

I used clear variable names and comments to describe the purpose of each method and section.
For example:

# Method b: add items and calculate total


This improves readability, making it easier for others (or myself in the future) to understand the code quickly.

5. Automation and Decision Logic

The system includes automated approval logic for totals less than $500:

if self.total < 500:
    self.status = "Approved"
    self.approval_ref = self.staff_id + str(self.requisition_id)


This design principle reflects efficiency and maintainability, as rules can be easily updated in the future (for example, changing the threshold value).

6. Testing and Reliability

The project includes several test cases where I ran the program with multiple requisitions to confirm:

Totals below $500 are approved automatically.

Totals equal to or above $500 remain pending.

Manager decisions correctly update the status.

Example output:

Total requisitions submitted: 5
Approved: 2
Pending: 1
Not approved: 2


Testing confirms the program works as intended and handles all scenarios correctly.

7. Future Improvements

During the maintenance phase, I proposed several enhancements:

Save all requisitions to a file or database.

Add more automatic approval rules.

Improve the interface for easier use.

Display more reports and statistics.

This aligns with the principles of extensibility and continuous improvement.

Analysis Summary

Through this project, I practiced and analyzed how programming principles such as modularity, OOP, encapsulation, and SRP contribute to code that is maintainable, readable, and extendable.

I also explored the importance of testing and automation in developing reliable software systems.

Reflection

Working on this project helped me connect theory to practice. I understood how:

Design principles improve code quality.

Organizing logic into classes and functions makes programs easier to debug.

Adding comments and structure helps in long-term maintenance.

The project demonstrates my ability to apply design principles in real-world coding tasks, matching Learning Outcome LO3:

Analyse a range of design principles, in relation to coding that is easy to maintain and extend.

Repository Contents
/Code
   ├── requisitionsystem.py      
   ├── Assignment 1.py           
   └── practice_examples/        


End of README

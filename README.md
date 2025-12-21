# CS 255 System Design: DriverPass
#### A Simulated Client Project for SNHU CS 255 
##### By: Alec Brandt

## Project Summary
**DriverPass** is a client-specific project for **Liam**, the owner of a driver training business. The goal was to design a centralized, cloud-based **Driver Training Management System** to replace his existing manual, paper-based operations. The system was designed to allow customers to register and schedule lessons online, while enabling the business to track student progress, manage instructor schedules, and automate vehicle assignments, thereby addressing the inefficiency of phone-based booking and lack of real-time data visibility.

## What did you do particularly well?
I was particularly effective in designing a robust **Role-Based Access Control (RBAC)** system. By clearly defining distinct actors: Customers, Instructors, Secretaries, and Administrators- and mapping their specific permissions in the **Use Case Diagrams**, I ensured the system would be secure and usable for different stakeholders. Additionally, the **Sequence Diagrams** I created for the lesson booking process were highly detailed, correctly modeling the complex interaction between the user interface, database, and scheduling logic to prevent double-booking.

## Revisions and Improvements
If I could revise one part of the system design, I would improve the **Training Package Management** module. Currently, the design implies that adding new training packages requires developer intervention to update the code (as noted in the project limitations).
**Improvement:** I would refactor this to be a fully data-driven feature. I would design an administrative interface that allows the Owner to create, edit, and price packages dynamically and store them in the database. This would remove the dependency on developers for routine business changes, making the system more sustainable for Liam in the long run.

## User Needs and System Design
**Interpretation:** The user (Liam) needed to reduce administrative overhead, and his customers needed flexibility. I interpreted this as a need for a **self-service portal**.
**Implementation:** I designed the system with a responsive web interface that allows customers to book lessons 24/7 without calling a secretary. For the owner, I ensured the system could generate reports and export data to Excel, matching his existing workflow for financial analysis.
**Importance:** Considering user needs is critical because a system that doesn't fit the user's actual workflow will be rejected. By automating the specific pain points (manual scheduling and progress tracking), the system provides immediate, tangible value.

## Software Design Approach
My approach to software design is **Architecture First**. I rely on visualizing the system using **UML (Unified Modeling Language)** diagrams before writing any code. For this project, I started with Use Case diagrams to understand scope, then moved to Class diagrams to structure the data, and finally Sequence diagrams to define logic.
**Future Perspective:** In the future, I will continue to use this iterative, visual modeling strategy but will incorporate more **user-centric prototyping** earlier in the process. I would essentially "wireframe" the critical user flows (like the booking engine) to validate requirements with the client before finalizing the backend architecture, ensuring the design is not just technically sound but also intuitive.
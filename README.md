# miniSIS
The system has students, teachers and administration members.
Students belong to group(s).
Each group is determined by a unique combination of speciality and group year.
Students take courses and may get grades from the assignments belonging to the course. The grading is the same as UFAZ's(out of 20)
***
Teachers can teach many courses and they can only grade the students in their courses.
Same course may be duplicated every year and semester, but in the given year and semester, it must be unique.
A subject may be assigned to a group, in which case all the students in that group must also be enrolled to that subject.
Each student has a unique ID that's generated when inserting the student.(It must be primary key).
Student ID is in the following format:
2024001, 2024002, 2024003
here, the first 4 digits show the admission year of the student, and the rest of the digits are automatically generated for each student. (The system can't have more than 999 students for each admission year, so don't worry about overflow.)
***
- Firstly implement this system's ERD using any tool you want.
- Implement the database schema in the supabase. However, don't use supabase's dashboard, create the tables using migrations.(https://supabase.com/docs/guides/deployment/database-migrations)
- Create all the necessary business logic using database functions.(For example, adding a student to a group, enrolling to a subject etc).
- Implement an edge function that returns comprehensive statistics about the student performance.(For example, show student who has the highest GPA in all groups for the given semester and academic year, show mean/min/max GPA of groups and subjects, show failing students(who has GPA below 10 for the academic year).
P.S: more tasks may be added in the future.

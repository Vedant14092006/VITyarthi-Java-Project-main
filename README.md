# VITyarthi-Java-Project
A project made for Programming In Java course of VITyarthi platform
Campus Course & Records Manager (CCRM) – Java SE Project
Project Overview:
CCRM is a Java console-based application for managing students, courses, and enrollment records. It supports:
Adding, listing, and managing students and courses
Enrolling students in courses and assigning grades
Importing/exporting data in CSV format
Generating simple reports such as GPA distribution
Backup of exported files

This project is designed for Java SE 17+ and uses a modular structure to separate CLI, domain, services, IO, and configuration.

Folder Structure:
CCRM-Project/
├─ src/                # Java source files
│  ├─ edu/ccrm/cli/       # Main CLI and console menu
│  ├─ edu/ccrm/config/    # App configuration and data store
│  ├─ edu/ccrm/domain/    # Domain classes (Student, Course, Enrollment, etc.)
│  ├─ edu/ccrm/io/        # Import/export and backup utilities
│  ├─ edu/ccrm/service/   # Service classes (StudentService, CourseService, Reports, etc.)
│  └─ edu/ccrm/util/      # Utility classes
├─ data/
│  └─ test-data/
│     ├─ students.csv     # Sample students data
│     └─ courses.csv      # Sample courses data
├─ build.bat            # Windows build script
├─ run.bat              # Windows run script
├─ README.txt           # Project instructions (this file)

Prerequisites:
Java JDK 17 or newer
Command Prompt / Terminal for building and running
Make sure JAVA_HOME is set to your JDK path, and PATH includes $JAVA_HOME/bin.
Building the Project
Windows:
Open Command Prompt at the project root.
Run:
build.bat
This compiles all .java files from src/ into the out/ folder.
If successful, you will see a message:
Build finished. Run using: run.bat

Linux/macOS (if applicable):
chmod +x build.sh
./build.sh

Running the Project:
Windows:
run.bat

Linux/macOS:
chmod +x run.sh
./run.sh

Notes:
Make sure out/ folder exists after build.
Sample data files are located under data/test-data/.
CSV Sample Data Format

students.csv:

id,regNo,fullName,email,dob
s1,REG2025/001,Vedant Seth,vedant@example.com,2003-05-12
s2,REG2025/002,Alice tiwari,alice@example.com,2004-02-01
s3,REG2025/003,Bob Singh,bob@example.com,2003-09-10

courses.csv:

code,title,credits,instructorId,semester,department
CS101,Intro to Programming,3,i1,SPRING,CS
CS102,Data Structures,4,i2,FALL,CS
MA101,Calculus I,3,i3,SPRING,Math

Features & Usage:
Manage Students
Add new student
List all students
Print student transcript
Manage Courses
Add new course
List all courses
Enrollment / Grades
Enroll/unenroll student in course
Assign grade to student

Import/Export:
Import students/courses from CSV
Export students/courses to CSV

Backup:
Backup exported files into timestamped folders

Reports:
GPA distribution report

Troubleshooting:
UnsupportedClassVersionError – Ensure JDK used to compile matches or is newer than the runtime version.
Classes not found – Verify src/ folder structure and package names.
Empty exports/backup – Ensure data/test-data/ exists and CSV files are in the correct format.

Author:
Vedant Seth
24BCE11450
B.Tech, Computer Science, VIT Bhopal


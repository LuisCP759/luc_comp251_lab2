# Lab 2 - Conceptual Modeling using Draw.io
This lab will meet the following course objectives:
1. Determine appropriate entity structure for relational databases
2. Apply the correct terminology to an ER Model
3. Design an ER model

## Instructions
In this lab, you will practice writing business rules that describe the relationships between entities. Using the school ER diagram below, write and recreate a conceptual ER diagram that illustrates the relationships shown.

![alt text](https://instructorc.github.io/site/home/images/school_ERD.PNG)

You will record your relationships within this README file. When writing down the relationships, follow the bullet points below.
- Entity names are uppercase and bolded
- The connecting verb is underlined
- Bidirectionality of the relationship is represented

Once you complete the README.md file, create an ER Diagram based on the relationships you identified. Create the ER Diagram using a free web-based tool called draw.io. The shapes you will use to create your ER diagram can be found under the "Entity Relation" tab. Instructions on how to use draw.io are in the assignment resources section below.

## Requirements

### Deliverable 1 (5 Points)
All relationships are identified, including the relationships that are formed when identifying the new **associative entities**

### Deliverable 2 (5 Points)
Update the ReadMe.md file to reflect the relationships. The relationships adhere to the following bullet points below.
- Entity names are uppercase and bolded
- The connecting verb is <ins>underlined</ins>
- Bi-direction of the relationship is represented

### Deliverable 3 (5 Points)
A conceptual Entity Relationship Diagram(ERD) is created to reflect all entities and relationships identified in the write-up

## Submission Guidelines
For this lab, submit 2 items to the repository. The two items that you will need to submit are listed below:
1. The README.MD file that identifies the various Entities and briefly describes each entity, including possible attributes, relationships, and assumptions.
   1. When identifying relationships, be sure to bold and uppercase the entity name, underline the verb, and make sure relationships are bidirectional.
   2. When identifying assumptions, make sure to formulate assumptions based on what is represented in the school ERD with either a Yes or No.
   3. You can override this README.md file that contains the instructions or extend this README.md file by listing your requirements below the lab Resources section.
2. The draw.io XML file that contains your ER Diagram. You will also need to take a snippet of the ER Diagram and add it as an image in your README file.

Once you complete both items above, submit the link to your repository for lab 2 before the due date and time listed.

## Lab Resources
- [Mark-down Syntax Cheat Sheet](https://enterprise.github.com/downloads/en/markdown-cheatsheet.pdf)
- [Make a ReadMe file Web-based Editor](https://www.makeareadme.com/)
- [Draw.io Web-based diagramming tool](https://app.diagrams.net/)
- [Creating Entity Relationship Diagrams using Draw.io](https://www.youtube.com/watch?v=lAtCySGDD48)

---

## Student Work Added Below

### Entity Descriptions
- **STUDENT**: Represents a person enrolled in classes. Possible attributes include student ID, name, and address.
- **SEAT**: Represents a specific assigned seat for a student within a classroom or section. Possible attributes include seat number and seat position.
- **COURSE**: Represents an academic subject offered by the school. Possible attributes include course number and course name.
- **SECTION**: Represents a specific offering of a course. Possible attributes include section number.
- **PROFESSOR**: Represents a faculty member who teaches sections. Possible attributes include professor ID, name, and faculty.
- **INSTRUCTOR**: Represents the faculty member assigned to teach a course. Possible attributes include instructor number, name, and faculty.

### Relationships
- **STUDENT** <ins>fills</ins> **SEAT**
- **SEAT** <ins>is filled by</ins> **STUDENT**
- **STUDENT** <ins>takes</ins> **COURSE**
- **COURSE** <ins>is taken by</ins> **STUDENT**
- **COURSE** <ins>has</ins> **SECTION**
- **SECTION** <ins>belongs to</ins> **COURSE**
- **SECTION** <ins>is taught by</ins> **PROFESSOR**
- **PROFESSOR** <ins>teaches</ins> **SECTION**
- **INSTRUCTOR** <ins>teaches</ins> **COURSE**
- **COURSE** <ins>is taught by</ins> **INSTRUCTOR**

### Assumptions
- Yes — A student may take multiple courses.
- Yes — A course can be offered in multiple sections.
- Yes — A section is associated with one course.
- Yes — A professor can teach multiple sections.
- Yes — An instructor can teach more than one course.
- No — A student is not limited to one seat across all courses; seat assignment depends on the specific course or section context.
- No — A professor and an instructor are not always the same entity if the diagram distinguishes roles separately.

### ERD Snippet
![ERD Snippet](https://instructorc.github.io/site/home/images/school_ERD.PNG)

### Summary
The conceptual model shows how students, courses, sections, instructors, and professors relate to each other in a school system. These relationships support the design of a normalized relational database and clarify the academic rules for enrollment and teaching assignments.

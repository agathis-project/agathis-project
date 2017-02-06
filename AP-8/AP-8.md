```
AP:      8
Title:   AP Purpose and Guidelines
State:   Draft
Type:    Process
License: CC-BY-SA
Author:  md-agathisproject
Issues:	 https://github.com/agathis-project/agathis-project/issues
```

## AP Purpose and Guidelines

###1. What is AP?

- AP stands for **Agathis Proposal**. An AP is a document providing
  information or describing a development feature, a process or an environment
  for the Agathis Project.

- The AP is developed and maintained as text file written in github flavoured 
  markdown with attachments files as needed.

### 2. AP Types

- **HW (Hardware Development)** describes the development of a hardware 
 feature(mechanical included) for the Agathis Project.

- **SW (Software Development)** describes the development of a software 
 feature(firmware included) for the Agathis Project.

- **Process** describes a process within Agathis Project community with the
  purpose of increasing development productivity and quality of communication.
 
- **Informational** provides general guidelines or information to the 
  Agathis Project community (not a feature) with the goals of improved 
  communications and creative productivity; standards derived from development
  APs fall under this type.  

### 3. The Workflow of Agathis Proposals

- Following workflows are identified:
  - Informational and Process AP Workflow
  - HW Development Workflow
  - SW Development Workflow 

- This document convers only the first workflow, whereas the other workflows 
  are convered by dedicated APs.

**Informational and Process AP Workflow:**
  
![AP Workflow](https://github.com/agathis-project/agathis-project/blob/master/AP-8/AP-8-1.png)

1. The AP process begins with a new idea.

  - Keep the AP focused. If in doubt, split AP into several well-focused ones.

  - Each AP have an author: someone who writes the AP using the proper style and 
  format, leads the discussions and builds community consensus around the idea.

2. Author get an AP number and a folder in the agathis-project repo.

3. Author sets the AP state to Idea.

4. Author last commmit before the review request should call "Idea Review" in 
  the first line.

5. Author open an issue titled **AP-? Idea Review Request** and identify the
   @arbiters in the body of the issue.

6. Agathis Project admin team release an anouncement about this review being 
   open to increase community awareness.

7. Comments to the review are collected.
   
8. Author fixes and reconciles all review findings.

9. Author request approval with issue titled **AP-? Idea Approval Request** 

10. Arbiters review fixes and reconciliations then comment issue with APPROVED
  or REJECTED; all arbiters shall respond; simple majority needed to pass the 
  review.

  - If Idea is not approved, then change the AP state to **Rejected**.
  
  - If Idea is approved, then change the AP state to **Draft**.

11. Author works to elaborates the idea to the draft completion.  

12. Author last commmit before the review request should call "Draft Review" in 
  the first line.

13. Author open an issue titled **AP-? Draft Review Request** and identify the
   @arbiters in the body of the issue.

14. The arbiters release an anouncement about this review open to increase 
  community awareness.

15. Comments to the review are collected.
   
16. Author fixes and reconciles all review findings.

17. Author request approval with issue titled **AP-? Draft Approval Request** 

18. Arbiters review fixes and reconciliations then comment issue with APPROVED
  or REJECTED; all arbiters shall respond; simple majority needed to pass the 
  review.

  - If Draft is not approved, then change the AP state to **Rejected**.
  
  - If Draft is approved, then change the AP state to **Release**.
  
19. As the AP is used by the community, issues start to accumulate.
  Any member may ask for an **AP-? Release Review Request** with an issue when 
  needed; call the @arbiters in the body of the issue.
  
20. The arbiters decide about the review by either:
  - replacing **Request** with **IN PROGRESS** in the title and release a
  community anouncement.
  - replacing **Request** with **REJECTED** in the title and closing the review 
   request issue it with an argument.

21. Author change the state of the AP to **Draft** then fixes and reconciles 
  all accumulated issues and new comments.

22. Author request approval with issue titled **AP-? Draft Approval Request** 

23. Arbiters review fixes and reconciliations then comment issue with APPROVED
  or REJECTED; all arbiters shall respond; simple majority needed to pass the 
  review.

  - If Release is not approved, then change the AP state to **Rejected**.
  
  - If Release is approved, then change the AP state to **Released**.

### 4. AP Structure

- **Title**
  - be consistent with the content.

- **Preamble**
  - headers containing meta-data about the AP as listed:

```
AP:      [AP number]
Title:   [title]
State:   [Idea | Draft | Release | Rejected]
Type:    [type]
License: [license]
Author:  [gihub username]
Issues:  [where the issues are tracked, url]
```  

- **Abstract**
  - keep it short.
  
- **Motivation and Rationale**
  - Motivation: something that needs no explanation or reasoning; 
    the originating desire or driver.
  - Rationale: provide a logical explanation.

- **Content**
  
- **References**

- **License**
  - preferred licenses by AP type:
    - Process and Informational: CC-BY-SA
	- SW development: GPL
	- HW development: TAPR
  
- **Attachments**
  - list the attachments; include visual prints for non-text files.
  - note the application software used for each non-text source.


### 5. Reporting AP Issues

- Issues during review process to be recorded as comments in the review request.

- Issues outside review request to be re recorded as proper issues starting
  with **AP-? Title** in the title of the issue.

### 6. Changing the AP

- Changing AP is possible only when AP is at Idea or Draft states.

### 7. Changing AP Author

- AP author may change as needed; always seek agreement; adding a new author 
  is preferred for a replacement
- Changing is done with updating the AP preamble and opening an issue titled
  **AP-? Author Change**  

### 8. AP Editing Checklist

- Overall compliance with AP-8 (this doc)

- Title consistency and accuracy.

- Edit the AP for language (spelling, grammar, sentence structure, etc.),
  markup and code style.

- Assign a AP number (the next available number).

- List the AP in AP-0.

### 9. References

### 10. License

- This work is licensed under Creative Commons Attribution-ShareAlike 4.0
  International License.

### 11. Attachments

- AP-1-1
  - AP-1-1.odg (source)
  - AP-1-1.png (presentation, image)
  - content: flowchart
  - editor: LibreOffice Draw 3.3.3


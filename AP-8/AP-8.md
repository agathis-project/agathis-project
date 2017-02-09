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

- AP stands for **Agathis Proposal**. An AP is a document describes a 
  development feature, a process or an environment for the Agathis Project.

- AP is developed and maintained as text file written in github flavoured 
  markdown with attachments files as needed.

### 2. AP Types

- **HW (Hardware Development)** describes a hardware feature.

- **SW (Software Development)** describes a software feature.

- **Process** formalize how to do things around with increased efficiency.
 
- **Informational** capture information worth documenting.

### 3. AP Workflows

- Following workflows are identified
  - **Informational and Process AP Workflow** - described herein.
  - **HW Development Workflow** - documented in a separate AP.
  - **SW Development Workflow** - documented in a separate AP.

***
  
#### Informational and Process AP Workflow:
  
![AP Workflow](https://github.com/agathis-project/agathis-project/blob/master/AP-8/AP-8-1.png)

1. There is an author with an idea:
  - to engage the Agathis Project, the author should get a number:
	- name the title of the idea.
	- describe the idea as an *Abstract* chapter.
	- provide the AP admin with the title and the abstract and ask for a number.
	- AP admin provides a number, AP folder and document template.

2. Prepare the idea for review:
	- the author forks the template and add content to the first two chapters:
		- Abstract
		- Rationale
	- add any supporting files.
	- pick a name from AP-10 Repository Names as repo field in the AP preamble.

3. Review the idea with AP community:
    - create a pull request.
	- follow the **AP-9 AP Review Process**
	- stop here if the idea is rejected; may go back and change the description 
	of the idea and try later another review.

4. Enter the draft state:
    - if review passed, the admin completes the github merge of AP document 
	and included attachments.
	- admin creates a repo with the name in the AP preamble and assign the 
	appropriate access for the AP author.
	- admin updates the state in the AP doc and **AP-0 Agathis Proposals Index**
    to **Draft**

5. Work on the draft:
	- Author works on Draft
	
6. Review the draft with AP community:
	- create a review request issue.
	- follow the **AP-9 AP Review Process**
	- stop here if the draft is rejected; may go back and change the draft
	and try later another review.

4. Enter the released state:
    - if review passed:
		- author updates the state in the APD doc preamble to **Released** 
		and - this must be the last change since the AP passed the 
		review.
		- admin updates the state in **AP-0 Agathis Proposals Index** to 
		**Released**
		- admin fills in the commit link (verifies first the AP doc	state is
		update)
		- the admin must now lockout any updates to the master.
		- any post release changes of the AP (the document or any attachment) 
		must start with creating a fork and updating the AP doc state to 
		"Draft".

5. Review the issues with AP community
		
		
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


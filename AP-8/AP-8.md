```
AP:      8
Title:   AP Guideline
Repo:    agathis-project
State:   Draft
Type:    Process
License: CC-BY-SA
Author:  md-agathisproject
Issues:	 https://github.com/agathis-project/agathis-project/issues
```

# AP Guideline

## 1. Abstract

The work on Agathis Project is organized using Agathis Proposals. The Agathis 
Proposal describes a development feature, a process or a formalized information 
for the Agathis Project. This document specifies how to work the Agathis 
Proposal from idea to release.

## 2. Rationale
AP Guideline helps improving:
  1. communication through documentation consistency 
  2. productivity by using well defined workflows

## 3. Content

### 3.1 AP Types

- **HW (Hardware Development)** documents a hardware feature.

- **SW (Software Development)** documents a software feature.

- **Process** documents how to do things around here with increased efficiency.
 
- **Informational** documents useful information.

### 3.2. AP Workflow

- the following workflows are identified:
  - **Informational and Process AP Workflow** - described herein.
  - **HW Development Workflow** - described in a separate AP.
  - **SW Development Workflow** - described in a separate AP.

***
  
### Informational and Process AP Workflow:
  
![AP Workflow](https://github.com/agathis-project/agathis-project/blob/master/AP-8/AP-8-1.png)

#### 3.2.1. There is an author with an idea:
- to engage the Agathis Project, the author should get a number; here is how:
  1. title the idea
  2. describe the idea in *Abstract* chapter
  3. provide admin with the title and the abstract and ask for a number
- admin responds:
  1. check AP title and abstract for sanity
  2. creates a new AP folder and with an AP document template.
  3. list the new AP in the AP Index

#### 3.2.2. Prepare the idea for review:
- author forks the template and add content to the first two chapters:
	- Abstract
	- Rationale
- author adds supporting files as needed

#### 3.2.3. Idea Review:
- author creates a pull request
- admin anounces the Idea Review
- all folks follow the [**AP-9 AP Review Process**] (https://github.com/agathis-project/agathis-project/blob/master/AP-9/AP-9.md)
- author stops here if idea is rejected; possible to go back later to 
  change the idea description and try another review.

#### 3.2.4. Entering the Draft state:
- admin merge the AP
- admin updates the state to "Draft" in AP-0 AP Index

#### 3.2.5. Work on the Draft:
- author first commit must have the preamble state updated to Draft
- author works on Draft
- author commits as necessary
- author may engage community for comments before entering the formal review
  by opening an issue; use **"Draft Comments Request"** label.
	
#### 3.2.6. Draft Review:
- create a review request issue; use *"Draft Review Request"* label
- admin anounces the Draft Review
- all folks follow the [**AP-9 AP Review Process**] (https://github.com/agathis-project/agathis-project/blob/master/AP-9/AP-9.md)
- stop here if the draft is rejected; possible to go back later to change 
  the draft and try another review

#### 3.2.7. Entering the Released State:
- author updates the state in the AP doc preamble to **Released**
- admin updates the state in **AP-0 Agathis Proposals Index**
- follow github process [**Creating Releases**](https://help.github.com/articles/creating-releases/)

#### 3.2.8. Issues during Released State:
- issues may be open by anyone; use Release# and AP-# labels to identify the 
  object of the issue.
- author responds to all issues within 5 days (normal case) or 30 days 
  (exceptions); passing 30 days limit triggers the change of the author (see below)

#### 3.2.9. Issues Review:
- **Issues Review** is the only mechanism to change a release (generate a new release?) !!!!!!!!!!!!!!!!
- triggered by anyone who creates an issue titled **Issues Review Request**
  and a rationale in the body; use Release# and AP-# labels to identify the 
  object of the issue. 
- the request is confirmed by admin who changes the state of the AP to 
  draft in AP-0 list; !!!!! should have some link pointing to last release? or to the list of the releases? !!!!!!!!!!!!!!!
- admin anounces the Issues Review
- all folks follow the [**AP-9 AP Review Process**] (https://github.com/agathis-project/agathis-project/blob/master/AP-9/AP-9.md)

#### 3.2.10. New release !!! see [github release process] (https://help.github.com/articles/creating-releases/) !!!! how we deal with next releases? !!!!!!!!!!!!!!!!!

### 3.3. AP Structure

- **Title**
  - consistent with the content.

- **Preamble**
  - headers containing meta-data about the AP as listed:

```
AP:      [AP number]
Title:   [title]
Repo:    [agathis-project]
State:   [Idea | Draft | Released | Rejected]
Type:    [Informational | Process]
License: [license]
Author:  [gihub username]
Issues:  [where the issues are tracked, url]
```  

- **1. Abstract**
  - keep it short; 
  - it's a *must have* for Idea Review
  
- **2. Rationale**
  - provide a logical explanation about the value of this AP;
  - it's a *must have* for Idea Review

- **3. Content**
  - this is the descriptive part of the AP.
  
- **4. References**

- **5. License**
  - CC-BY-SA is the preferred license for *Process* and *Informational* APs.
  
- **6. Attachments**
  - list the attachments; include visual prints for non-text files.
  - note the application software used for each non-text source.

### 3.4. Changing AP Author

- author may change; always seek agreement; adding a new author is preferred 
  for a replacement.
  
- APs are declared orphaned if isues are not commented by author within 30 days.

- admin makes an anouncement about the orphaned AP and the seek for a new 
  author.

- anyone interested in taking the author role should open an issue for that AP.

- admin decides about the new author and assign the rights to the repo.

- author change is effective when the AP preamble is updated by author.

## 4. References

## 5. License

- This work is licensed under Creative Commons Attribution-ShareAlike 4.0
  International License.

## 6. Attachments

- AP-1-1
  - AP-1-1.odg (source)
  - AP-1-1.png (presentation, image)
  - content: flowchart
  - editor: LibreOffice Draw 3.3.3
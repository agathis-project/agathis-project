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

The work on Agathis Project is organized using Agathis Proposals. An Agathis 
Proposal describes a development feature, a process or a formalized information 
for the Agathis Project. This document specifies how to work the Agathis 
Proposal from idea to release.

## 2. Rationale
AP Guideline helps to:
  1. improve communication through documentation consistency. 
  2. improve productivity through repeatable workflows.

## 3. Content

### 3.1. AP Types
A number of four types of Agathis Proposals are identified:

- **HW (Hardware Development) AP** documents a hardware feature.

- **SW (Software Development) AP** documents a software feature.

- **Process AP** documents how to do things around here with increased efficiency.
 
- **Informational AP** documents useful information.

### 3.2. APs and the Repository

- **Informational and Process APs** are always located in agathis-project repo, 
  under their *AP-? folder*; the main text file, markdown formated, is 
  named *AP-?.md*.
  
- During idea state, **Development APs** are located in agathis-project repo, 
  under their *AP-?* folder; the AP text file, markdown formated, is *AP-?.md*.
  These APs are moved into their own repo when they pass the idea 
  review; at the time of this move, the *AP-?.md* file is renamed as 
  *readme.md* and stored in the root of the repo, becoming the main 
  documentation file.
  
- The github **master** branch of any repo can be modified only through merge 
  preceded by a pull-request; direct master editing is horrible.
  
- Actual editing of a repo shall be done only on branches; these branches are
  merged into the master following a pull-request.
  
- All merges in agathis-project repository (holding informational and 
  process APs) are done by admins only. 

### 3.3. Informational and Process AP Workflow
The workflows for HW and SW APs are described in their respective docs.

***
  
### Workflow Overview:

![AP Workflow](https://github.com/agathis-project/agathis-project/blob/master/AP-8/AP-8-1p1.png)

Process and Informational APs have three main states: **Idea, Draft and Release**

#### 3.3.1. Idea State
![AP Workflow](https://github.com/agathis-project/agathis-project/blob/master/AP-8/AP-8-1p2.png)

**Someone (called author herein) got an idea worth pursuing:**
- To engage the Agathis Project, the author should get a number; here is how:
  - go to agathis-project repo and **open an new issue:**
  - label it with **New idea**:
  - **title** is with intended AP title.
  - fill in the comments area with the **abstract of the idea**.
  - append **@admin** tag at the end of the abstract.
  - **submit**.
	
**This issue will trigger the admin response:**

  1. check AP title and summary for sanity; if the idea is insane skip to 
     last step.
	 
  2. create a new AP folder with an AP document template; fill in preamble 
     and abstract; the AP number should be taken as the next available in the 
	 AP Index.
	 
  3. list the new AP at idea state in the AP Index.
  
  4. create a branch named *AP-? Title*; any other branches related to this AP 
     shall use this branch name as prefix.
  
  5. comment the issue and close it.
  
  6. create a community anouncement for this event.
  
** The author prepares the idea for review:**
  - work on branch *AP-? Title*
	- not too much, not too little: just enough for the team to get the idea
	  and comment - before too much work may get to waste or block team 
	  contributions.
    - commit as needed.
  - get ready for pull request.
	
**Idea Pull Request**
  - the author open a pull request when ready.
  - discuss and fix issues, comments; 
  - commit as needed.
  
**Idea Review**
- follow AP-9 Review.

#### 3.3.2. Draft State
![AP Workflow](https://github.com/agathis-project/agathis-project/blob/master/AP-8/AP-8-1p3.png)

**Entering the Draft State:**
- if review vote is passed: 
  - the admin merge the AP as voted with the preamble state updated to Draft.
  - the admin updates the state to "Draft" in AP-0 AP Index.

**Work on the draft:**
- the author creates a branch and edit AP.
- commit as needed.

**Draft Pull Request**
- the author open a pull request when ready.
- discuss and fix issues, comments; commit as needed.

**Draft Review**
- follow AP-9 Review.

#### 3.3.3. Released State
![AP Workflow](https://github.com/agathis-project/agathis-project/blob/master/AP-8/AP-8-1p4.png)

**Entering the Released State:**
- if the review vote is passed:
  - the admin merge the AP branch with the preamble state updated to Released.
  - the admin updates the AP state to "Released" in AP Index.

**Work on the release:**
- issues accumulating
- the author creates a branch *AP-# Title ___Release* and edit when needed; all 
  edits in the released state should refer to an issue; in other words no 
  edits without issues.
- commit as needed; commits messages should refer to addressed issues.

**Release Pull Request**
- the author open a pull request when ready.
- discuss and fix issues, comments.
- commit as needed.

**Release Review**
- follow AP-9 Review.

Note1: for Informational and Process AP, at any time, there is only one valid 
release: the master (default branch) - the latest and greatest.

Exception to Note1: AP-9 AP Index content is always edited on the master.

Note2: Workflows already in progress should adapt on-the-fly to latest relevant 
APs.

### 3.4. AP Structure

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
  - it's a *must* for Idea Review
  
- **2. Rationale**
  - provide a logical explanation about the value of this AP;
  - it's a *must* for Idea Review

- **3. Content**
  - this is the descriptive part of the AP.
  
- **4. References**

- **5. License**
  - CC-BY-SA is the preferred license for *Process* and *Informational* APs.
  
- **6. Attachments**
  - list the attachments; include visual prints for non-text files.
  - note the application software used for each non-text source.

### 3.5. Changing AP Author

- the author is not a title, but a reponsibility.

- the author may change; always seek agreement.
  
- APs are declared orphaned if its issues are not commented by author within 
  30 days and a specific issue is created.

- the admin makes an anouncement about the orphaned AP and the search for a new 
  author.

- anyone interested in taking the author responsibility  should comment on the 
  issue.

- the admin decides about the new author and assign the rights to the repo.

- the author change is effective when the author in the AP preamble is updated 
  by the admin.

## 4. References

- github pull request workflow
- AP Review

## 5. License

- This work is licensed under Creative Commons Attribution-ShareAlike 4.0
  International License.

## 6. Attachments

- AP-1-1
  - AP-1-1.odg (source)
  - AP-1-1.png (presentation, image)
  - AP-1-1p1.png (presentation, image)
  - AP-1-1p2.png (presentation, image)
  - AP-1-1p3.png (presentation, image)  
  - AP-1-1p4.png (presentation, image)  
  - content: flowchart diagrams
  - editor: LibreOffice Draw 3.3.3
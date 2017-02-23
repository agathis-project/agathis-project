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

### 3.2. APs and the Repository

- **Informational and Process APs** are always located in agathis-project repo, 
  under their *AP-? folder*; the main text file, markdown formated, is 
  named *AP-?.md*.
  
- During idea state, **Development APs** are located in agathis-project repo, 
  under their *AP-?* folder; the AP text file, markdown formated, is *AP-?.md*.
  
- Development APs are moved into their own repo when they pass the idea 
  review; at the time of this move, the *AP-?.md* file is renamed as 
  *readme.md* and stored in the root of the repo, becoming the main 
  documentation file.
  
- The github **master** branch of any repo can be modified only through merge 
  preceded by pull-request a operation; no direct master editing allowed.
  
- Actual editing of a repo shall be done only on branches; these branches are
  merged back into the master after a pull-request.
  
- All merges in agathis-project repository (holding informational and 
  process APs) are done by admins only. 

### 3.3. AP Workflow, Informational and Process

- overall, the following workflows are identified:
  - **Informational and Process AP Workflow** - described herein.
  - **HW Development Workflow** - covered by a dedicated AP.
  - **SW Development Workflow** - covered by a dedicated AP.

***
  
### Informational and Process AP Workflow:

![AP Workflow](https://github.com/agathis-project/agathis-project/blob/master/AP-8/AP-8-1.png)

- an AP has three main states: **Idea, Draft and Released**

#### 3.3.1. Idea State
![AP Workflow](https://github.com/agathis-project/agathis-project/blob/master/AP-8/AP-8-1p1.png)

**Someone (called author herein) got an idea worth pursuing:**
To engage the Agathis Project, the author should get a number; here is how:
  1. Go to agathis-project repo and open an new issue:
    - label it with **New idea**:
	- title is same as AP title.
    - fill in the comments area with the abstract of the AP idea.
	- append @admin tag at the end of the abstract.
	- submit.
	
**This issue will trigger the admin response:**

  1. check AP title and summary for sanity; if the idea is insane skip to 
     last step.
	 
  2. create a new AP folder with an AP document template; fill in preamble 
     and abstract; the AP number should be taken as the next available in the 
	 AP Index.
	 
  3. list the new AP at idea state in the AP Index.
  
  4. create a branch named AP-# <Title>; any other branches related to this AP 
     shall use this branch name as prefix followed by --<specific identifier>.
  
  5. comment the issue and close it.
  
  6. create a community anouncement for this event.
  
** The author prepares the idea for review:**
  - work on branch AP-# <Title>
	- not too much not too little: just enough for the team to get the idea
	  and comment before too much work may get to waste.
    - commit as needed.
  - do pull request when ready
	
**Idea Pull Request**
  - author open a pull request when ready.
  - discuss and fix issues, comments; commit as needed.
  
**Idea Review**
- follow AP-9 Review.

#### 3.3.2. Draft State
![AP Workflow](https://github.com/agathis-project/agathis-project/blob/master/AP-8/AP-8-1p2.png)

**Entering the Draft State:**
- admin merge the AP as voted with the preamble state updated to Draft.
- admin updates the state to "Draft" in AP-0 AP Index.

**Work on the draft:**
- author creates a branch and edit AP;  commit as needed.

**Draft Pull Request
- author open a pull request when ready.
- discuss and fix issues, comments; commit as needed.

**Draft Review**
- follow AP-9 Review.

#### 3.3.3. Released State
![AP Workflow](https://github.com/agathis-project/agathis-project/blob/master/AP-8/AP-8-1p3.png)

**Entering the Released State:**
- admin merge the AP as voted with the preamble state updated to Released.
- admin updates the state to "Released" in AP-0 AP Index.

**Work on the release:**
- issues accumulating
- author creates a branch *AP-# Title ___Release* and edit when needed; all 
  edits in the released state should refer to an issue; in other words no 
  edits without issues.
- commit as needed; commits messages should refer to addressed issues.

**Release Pull REquest
- author open a pull request when ready.
- discuss and fix issues, comments; commit as needed.

**Released Review**
- follow AP-9 Review.

Note: for Informational and Process AP there is only one active and valid 
release: the master (default branch).


### 3.4. AP Structure

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

### 3.5. Changing AP Author

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
```
AP:      8
Title:   AP Guideline
Repo:    agathis-project
State:   Draft
Type:    Process
License: CC-BY-SA
Author:  md-agathisproject
```

# AP Guideline

## 1. Abstract

The work on Agathis Project github organization is organized using Agathis
Proposals. An Agathis Proposal describes a development feature, a process or a
formalized information. This document specifies the general framework of
Agathis Proposals and specifically how to drive the Process and Information APs
from idea to release.

## 2. Rationale

AP Guideline helps to:

- improve communication through documentation consistency.
- improve productivity through repeatable workflows.

## 3. Content

### 3.1. AP Types

A number of four types of Agathis Proposals are identified:

1. **HW (Hardware Development) AP** documents a hardware feature.
2. **SW (Software Development) AP** documents a software feature.
3. **Process AP** documents how to do things around here with increased efficiency.
4. **Informational AP** documents useful information.

### 3.2. AP and Repository

1. **Informational and Process APs** are always located in agathis-project repo,
  under their respective AP folder; *AP-?.md* is the main text file,
  markdown formated.

2. **Development APs**  are born as ideas in agathis-project repo then moved and
  grown under their own repo:
    - while hosted in agathis-project repo, they are located in their respective
    AP folder, where *AP-?.md* is the main text file, markdown formated.
    - after they pass the idea review, development APs are moved in their own
    repo with *AP-?.md* file becoming *readme.md* in the repo's root.

3. the **master** (default) branch can be modified only through merging pull
  requests; actual work shall be done on a non-master branch.

4. all merges in agathis-project repo are done by admins only.

5. the merges in development repos are done by their respective authors with
  admin rights.

### 3.3. Informational and Process AP Workflow

Note: the workflows for HW and SW APs are described in their respective docs.

***

### Workflow Overview

![AP Workflow](AP-8-1p1.png)

Process and Informational APs have three main states: **Idea, Draft and Release**.

#### 3.3.1. Idea State

![AP Workflow](AP-8-1p2.png)

1. **Someone (called author herein) got an idea:** to engage the
   Agathis Project, the author should get an AP number.
    1. go to agathis-project repo and **open an new issue** labelled **New idea**.
    2. **title** it with intended AP title.
    3. fill in the comments area with the **abstract of the idea**.
    4. append **@admin** tag at the end of the abstract.
    5. **submit** the issue.

2. **This issue will trigger the admin response:**
    1. check AP title and summary for sanity; if the idea is insane skip to
       step 5.
    2. create a new AP folder with an AP document template; fill in preamble
       and abstract; the AP number should be taken as the next available in the
       AP Index.
    3. list the new AP at *idea* state in the AP Index.
    4. create a branch named *AP-?-Title-Idea*.
    5. comment the issue and close it.

3. **The author prepares the idea for review:**
    1. work on branch *AP-? Title*
    2. not too much, not too little: just enough for the team to get the idea
      and comment - before too much work may get to waste or block team
      contributions.
    3. commit as needed.

4. **Idea Pull Request**
    1. the author starts a pull request when ready.
    2. discuss and fix issues, comments.
    3. commit as needed.

5. **Idea Vote** -- see **Vote** chapter at the end of the this doc.

#### 3.3.2. Draft State

![AP Workflow](AP-8-1p3.png)

1. **Entering the Draft State:** if review vote is passed.
    - the admin merge the AP as voted with the preamble state updated to Draft.
    - the admin updates the state to "Draft" in AP-0 AP Index.

2. **Work on the draft:**
    - the author creates a branch named *AP-?-Title-Draft* and edit the AP on this branch.
    - commit as needed.


3. **Draft Pull Request**
    - the author starts a pull request when ready.
    - discuss and fix issues, comments.
    - commit as needed.

4. **Draft Vote** -- see **Vote** chapter at the end of the this doc.

#### 3.3.3. Released State

![AP Workflow](AP-8-1p4.png)

1. **Entering the Released State:** if the review vote is passed
    - the admin merge the AP branch with the preamble state updated to Released.
    - the admin updates the AP state to "Release" in AP Index.


2. **Work on the release:**
    - issues accumulating.
    - the author creates a branch *AP-?-Title-Release*.
	
3. **every commit** in the release state should refer to an issue; in other words,
no commits without issues.

4. **Release Pull Request**
    - the author starts a pull request when ready.
    - discuss comments and fix issues.
    - commit as needed.

5. **Release Vote** -- see **Vote** chapter at the end of the this doc.

Note1: for Informational and Process AP, at any time, there is only one valid
release: the master (default branch) - is the latest and the greatest.

Note2: *AP-0 AP Index* is always edited on the master branch.

Note3: Workflows already in progress should adapt on-the-fly to latest relevant
APs.

Note4: The admin updates the Agathis Project community with one announcement
for each workflow event (branches, pull requests, merges, reviews and state
changes).

### 3.4. AP Structure

- **Preamble**
  - headers containing meta-data about the AP as listed.

```
AP:      [AP number]
Title:   [title]
Repo:    [agathis-project]
State:   [Idea | Draft | Release]
Type:    [Informational | Process]
License: [license]
Author:  [github username]
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

  - list the attachments; include prints for non-text files.
  - note the application software used for each non-text source.

### 3.5. AP Formatting Rules

Th AP documents use [markdown](https://en.wikipedia.org/wiki/Markdown) for formatting.
The following rules are recommended:

- use spaces **NOT tabs**, Please make sure your text editor is configured te replace tabs with spaces.
There is no rule for how many spaces per tab, just try to be consistent

- there should be an **empty line** after a header

- if you write a list and you don't know if it should be ordered or unordered
error on the side of ordered lists.

- 80 characters per line (this is not absolute, i.e. it is allowed to finish the word)

### 3.6. Changing AP Author

1. the author is a responsibility, not a title; fulfilling the author's role
   requires, beside the creativity for the initial idea, time and effort to
   complete the AP and maintain it through its lifecycle.

2. the author responsibility is measured through the way the issues are
   addressed.

3. the author should seek replacement when needed:
    1. the author open an issue titled AP-?-Title-Author Replacement.
    2. the admin makes a community announcement.
    3. anyone interested in taking the author responsibility  should comment on
       the issue.
    4. the admin decides about the new author and assign the rights to the repo.

4. APs are declared orphaned if open issues are not commented by author within
  30 days:
    1. the admin open an issue titled AP-?-Title-Author Replacement in the AP's
       repo and makes a community announcement.
    2. anyone interested in taking the author responsibility  should comment on
       the issue.
    3. the admin decides about the new author and assign the rights to the repo.

5. the author change is effective when the author in the AP preamble is updated
   by the admin.

  
### 3.6. Editing recommendations:

1. **Numbered versus bulet list:** use bulet list is the items are less than 3
  and numbered list otherwise.

2. **Limit the number of caracters per row to 80**; this is a soft recommendation.

3. **Avoid tabs at any cost**

### 3.7. Voting

1. After all was said and done during a state change pull request, the author 
  ask the project community to vote the pull request by opening an issue titled
  "Pull Request Vote".

2. The author proposes the voters list in the comment area (use @voter_name 
  tag); the admin ammends this list as needed.

3. The voters comment the issue with +1 (approve) or -1 (reject) within 5 days 
  limit.

4. After voting is closed, the admin does the followings:
    - counts the votes; if the counting is undecided, the admin has the last 
	word. 
	- comments the *Pull Request Vote* issue declaring the result as *approved*
	or *rejected*.
	- merges the pull request if approved.

## 4. References

1. [Github Flow] http://scottchacon.com/2011/08/31/github-flow.html
2. [Pro Git book] https://git-scm.com/book/en/v2
3. [Github Help] https://help.github.com/

## 5. License

- This work is licensed under Creative Commons Attribution-ShareAlike 4.0
  International License.

## 6. Attachments

- AP-1-1
  - files:
    1. AP-1-1.odg (source)
    2. AP-1-1p1.png (presentation, image)
    3. AP-1-1p2.png (presentation, image)
    4. AP-1-1p3.png (presentation, image)
    5. AP-1-1p4.png (presentation, image)
  - content: flowchart diagrams
  - editor: LibreOffice Draw 3.3.3

    AP: AP-8
    Title: AP Purpose and Guidelines
    Type: Process
    License: CC-BY-SA
    State: Draft
    Author: md-agathisproject
    Issue-Tracker:	
	

## AP Purpose and Guidelines


###1. What is AP?


- AP stands for Agathis Proposal. An AP is a document providing
  information or describing a development feature, a process or an environment
  for Agathis Project.

- The AP is developed and maintained as text file with attachments files where
  needed. While the text files are sufficient to document firmware or
  software features, there are places where text files are not sufficient.
  Use attachments as needed for better clarifying and understanding of AP.

### 2. AP Types

- **Development AP** describes a new feature or implementation for 
  Agathis Project.

- **Informational AP** provides general guidelines or information to the 
  Agathis Project community (not a feature) with the goals of improved 
  communications and creative productivity.

- **Process AP** describes a process within Agathis Project community with the
  purpose of increasing development productivity and communication quality.

### 3. APs and Work Flow

- The AP process begins with a new idea.

- Small enhancements or patches often don't need a AP and can be injected into
  the Agathis Project development workflow with a pull request on github.

- Keep the AP focused. Unfocused APs will be amended by Agathis Project 
  community. If in doubt, split AP into several well-focused ones.

- Each AP have an author (champion or owner) -- someone who writes the AP
  using the proper style and format, leads the discussions and builds community
  consensus around the idea.

- Author releases AP idea to repository and post a review request.
  - Get an AP number from the Agathis Project Admin Team.
  - Set AP *State* to Idea;
  - List the attachments in the "Attachments" chapter and have them ready
    for commit in appropriate folder structure.
  - Commit the AP file(s) with following message to the agathis-project repo in
    the ap-idea folder: 
	  - **AP-?: Released to Idea State**

- Author initiates the review process using the **Issue** feature in github

- Author fixes and reconciles all findings found during review.

- Author decides about the draft phase path; choose either:
  - draft (for most of the *informational* and *process* APs)
  - draft.design then draft.implementation (for most of the *developmental* 
    APs)

- The workflow described below is for the **draft** path; the workflow for
  **draft.design** then **draft.implementation** is very similar and
  not detailed here to preserve simplicity of this document.

- Set state to *Draft*

- Commit AP with message:
  - *AP-?: Released to Draft State*
  - *[list of changes]**

- Complete the outstanding work; commit when ready for review.

- Change the AP *State* to Final.

- Commit the AP file(s) with message:
  - *AP-?: Released to Final State*
  - *[list of changes]**

- The AP in Final state is deployed as:
  - sub-part of a software release
  - new product or product change
  - new process or process change

- The term of *deployment* means or triggers:
  - start using the AP (an Informational or Process AP)
  - tell the world the AP is available
  - ship a HW piece or a system.
  - release software that incorporates the change.

- As the AP is used by the community, unresolved issues start to accumulate.

- As the time passes, other competing AP may start to be developed.

- The overall status of the AP quality is monitored by Agathis Project 
  community.

- The Agathis Project community decides to:
  - do a change process (this workflow continues).
  - replace the AP (this workflow stops).
  - reject the AP (this workflow stops).

- Do the Change Process (CP). (The CP is only briefly described here;
  a subsequent AP will be dedicated to CP.)

- Review the CP.

- If findings are not cleared, then reject the AP.

- Release the AP to Final.

- Deploy the AP.

#### 3.1. AP states

- **Ide** Idea
 - decided by the author.
 - triggers the idea review.

- **Dra** Draft
  - Informational and Process AP only
  - decided after idea review.
  - triggers the work on the draft.

- **DD** Draft.Design
  - Development AP only
  - decided after idea review.
  - triggers the work on the draft.design

- **DI** Draft.Implementation
  - Development AP only
  - decided after the review of completed work on draft.design.
  - triggers the work on the draft.implementation.

- **Dpl** Deployed
  - decided after the review of completed work on draft.implementation,
    draft or change process.
  - triggers the deployment.

- **CP** Change Process
  - decided after the review of accumulationg issues and competing APs.
  - triggers the work on change process.

- **Def** Deferred
  - decided based on resource availability.
  - it means the AP is set aside.
  - re-evaluate the environment and history before restarting the work.
  - this state occurs during actual work.

- **Rej (Rejected)**
  - decided based on AP relevance and quality.
  - it means the AP is junked.
  - this state concurs during review.

- **Rpl (Replaced)**
  - decided after the evaluation of accumulating issues and competing issues.
  - it means the AP is junked with replacement.
  - this state occurs during review.

### 4. AP Structure


- **Preamble**
  - headers containing meta-data about the AP.

- **Abstract**

- **Motivation and Rationale**

- **Compatibility**

- **Design Specifications**
  - describe the technical details
    and parameters of the new feature; describe the interface with the existing
    system. Use attachments as needed and list them in the main AP.

- **Implementation**
  - implement the specification in real code or HW prototype and test it.
    Use attachments as needed and list them in the main AP.

- **Resources**
  - optional

- **References**
  - optional

- **License**
  - list the license(s): type and where used.

- **Attachments**
  - list the attachments

### 5. AP Formats and Templates

- The text part of the AP is written in markdown. This format allows
  for rich markup supported by github.

### 6. AP Header Preamble

Each AP begins with headers preamble as listed below

    AP: [AP number]
    Title: [AP title]
    Type: [type]
    License: [license]
    State: [state]
    Author: [names, emails, CSV]
    Issue-Tracker: [Issue Tracker URL]

- **AP: [AP number]**
  - Defined by admin on author's request.

- **Title: [title]**
  - Defined by the author; it may change during idea phase; never after.

- **Type: [type]**
  - Defined by the author
  - Informational
  - Development
  - Process

- **License: [license]**
  - Defined by the author.

- **State: [state]**
  - Defined by the author.

- **Author: [names, emails, csv]**
  - Defined by the author.
  - List the name(s) and email(s) of the author(s).

- **Issue-Tracker: [Issue Tracker URL]**
  - Defined by the author.
  - Indicates the web address of the Issue Tracker used to monitor the issues
    related to this AP.

### 7. Attachments

- Attachments are files that complement the main AP. AP may include source code,
  diagrams, schematics, bill of materials, PCB design, test reports etc;
  in short, the attachments contain the information that can't fit in the
  formal structure of the AP and within a reasonable number of lines.

- The non-text attachments are provided in two forms: source and presentation.
  The source form needs a specialized (CAD) application to edit/change its
  content. The presentation form is easy to read by common applications
  (pdf reader, web browser).

- The attachments can be grouped in folder/directories as needed to make
  the attachment list AND the development work easy manageable.

- The naming of the attachments follows the convention:

  AP-x-[y|z].ext, where:
 - y is the index for the attachment (1, 2...); use as many digits as needed,
   but no more.
 - z is the acronym or name of the file or folder (package of files)
 - use y or z as needed for easy files naming management
 - ext is the file extension

### 8. Reporting AP Issues

- While the AP is in review use the code review feature (if supported by
  the project hosting) or else the *Mailing List*.

- While the AP is Draft, Final, Deferred, Rejected or EOL
  use the *Issue Tracker*.

### 9. Changing the AP

- Any AP changes will follow the change process described in subsequent AP(s).

### 10. Transferring AP Ownership

- Sometimes it becomes necessary to transfer ownership of APs to a new
  champion/owner/author. Where possible - it is recommended to retain the
  original author as a co-author of the transferred AP.

- A good reason to transfer ownership is because the original author is
  no longer available.

- A bad reason to transfer ownership is because of disagreement with the
  direction of the AP. It is advisable to build consensus around a AP,
  but if that's not possible, then submit a competing AP.

- If someone is interested in assuming ownership of a AP, send a message
  to the *Mailing List*.

### 11. AP Editing Checklist

- Overall compliance with AP-8 (this doc)

- Title accurately describes the content.

- Edit the AP for language (spelling, grammar, sentence structure, etc.),
  markup and code style.

- Assign a AP number (the next available number).

- List the AP in AP-0.


### 12. References and Footnotes

- this document is inspired from http://www.python.org/dev/peps/pep-0001/

### 13. License

- This work is licensed under Creative Commons Attribution-ShareAlike 4.0
  International License.

### 14. Attachments

- AP-1-1
  - AP-1-1.odg (source)
  - AP-1-1.png (presentation, image)
  - content: flowchart
  - editor: LibreOffice Draw 3.3.3

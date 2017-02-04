    AP: AP-9
    Title: AP Review Process
    Type: Process
    License: CC-BY-SA
    State: Draft
    Author: jonsnow1357
    Issue-Tracker:


## AP Review Process

### 1. Summary and Assumptions

This document aims to describe the review process followed for this project (agathis). Any mention of review process in other documents produces by the project can be referenced to this AP.

Since this project is hosted on [github](https://github.com/agathis-project) it will try to use the existent features on this site. We will also try to describe how to use these features rather tha assume familiarity with them.

### 2. Review Process

#### 2.1 Start

To start a review, the relevant AP documents have to be in github, be clearly identified (in a separate repository or a specific folder of a repository) and have 0 pull requests opened.

A [**issue**](https://guides.github.com/features/issues/) has be opened by the person responsible for changing the state of the AP. We'll refer to this as the *start issue*.

Since github has **labels** and **milestones** to allow for the easy sorting of issues it is recommended that the start issue has the **label**: **review** and **milestone**: the name of the target state of the review process.

#### 2.2 Contribute

Contributing to a review can be made in different ways. For small changes or targeted comments related to the AP in review you can comment directly to the *start issue*, or open a different issue with the same **label** and **milestone**.

Opening another issue allows tracking of everything related to the review and declutters the *start issue* from multiple discussions going on in parralel.

For big changes the recommended way is to [fork](https://guides.github.com/activities/forking/) the AP documents in review, make the changes and then initiate a pull request. It is recommended to reference the *start issue* when you create the pull request.

#### 2.3 End

To close an review the default policy is to assume that if there are no comments then the review is done. This can translate in the following algorithm:

- if there are any pull requests for the AP documents resolve and merge them.
- filter the issues to show only the ones with the **label** and **milestone** that refer to the review
- if there are any other issues opened close them
- if for 5 days only the *start issue* is in the filtered list then the review can be closed by sclosing the **start issue*

### 3. License

- This work is licensed under Creative Commons Attribution-ShareAlike 4.0
  International License.

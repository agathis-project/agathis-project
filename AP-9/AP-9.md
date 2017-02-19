    AP: AP-9
    Title: AP Review
    Type: Process
    License: CC-BY-SA
    State: Draft
    Author: jonsnow1357
    Issue-Tracker:

## AP Review

### 1. Definitions

- **project** is the [Agathis Project](https://github.com/agathis-project)
- **review** is the process that takes place when transitioning between the states defined in [AP-8](https://github.com/agathis-project/agathis-project/blob/master/AP-8/AP-8.md)
- **admin** refers to members of the project administration team
- **AP** [Agathis Proposal](https://github.com/agathis-project/agathis-project/blob/master/AP-8/AP-8.md#1-abstract)

### 2. Summary

This document aims to describe the *review* followed for this *project*. Any mention of *review* in other documents produced by the project can be referenced to this *AP*.

Since this *project* is hosted on [github](https://github.com/agathis-project) it will try to use the existent features on this site. We will also try to describe how to use these features rather than assume familiarity with them.

All changes to an *AP* ([**issues**](https://guides.github.com/features/issues/) or [**pull requests**](https://guides.github.com/activities/forking/)) that happen without changing the state of the *AP* during the normal [github flow](https://guides.github.com/introduction/flow/) are not the object of this document.

### 3. Review

#### 3.1 Start

To start a *review*, the relevant *AP* documents have to be in github, be clearly identified (in a separate repository or a specific folder of a repository) and have 0 pull requests and 0 issues opened.

An issue has to be opened by the person responsible for changing the state of the *AP*. We'll refer to this as the *review issue*. Since github has **labels** to allow for the easy sorting of issues it is recommended that the *review issue* has the following labels: **review**, **AP-???** (the name of the *AP*) and **current state** (the current state the *AP* is in).

During the *review* there should be **NO MORE** commits to the *AP* documents. Any commit that happens in the period since the opening of the *review issue* to its closing will automatically invalidate the *review*.

#### 3.2 Voting

It is recommended that there is a time limit specified in the *review issue* but he author. If it's not there the default time limit is 5 days.

Once the *review issue* is opened it is expected that the interested parties **will** vote on changing the state of the *AP*. however the vote is open to everybody. The voting should follow the [apache voting process](https://www.apache.org/foundation/voting.html) and it should be done as comments to the *review issue*.

If the vote is negative a reason for this should be given in the comments (because we assume that the opposition to the state change actually has some arguments behind). Negative votes without explanations **can** be ignored in the vote count.

#### 3.3 End

After the time limit expires the votes are counted and the result shows if the state change is accepted or not. Any disagreements about the vote counts should be resolved by the *admin*.

In case of vote tie, the state change is considered rejected.

The *review issue* will be closed after the vote count, and regular development can continue.

#### 3.4. Review Example(s)

Suppose AP-314 is in state *Draft* and after work and discussions with the team the author is ready to change the state to *Release*.

The author opens the *review issue* with the labels: **review**, **AP-314** and **Draft** and specifies a time limit of 10 days for voting.

At the end of the voting period there were three votes expressed : +1, -0.5 and 0. In this case the *AP* will change the state to *Release*.

### 4. License

- This work is licensed under Creative Commons Attribution-ShareAlike 4.0 International License.

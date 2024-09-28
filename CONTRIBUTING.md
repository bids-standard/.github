# Contributing to BIDS

These contributing guidelines should apply
to most, if not all, the repositories in the BIDS github organization.

Each repository may also have more specific guidelines.

These guidelines are designed to make it as easy as possible
for you to get involved.
If you have any questions that aren't discussed below,
please let us know
by [opening an issue](#understanding-issues).

## Joining the community

BIDS - the [Brain Imaging Data Structure](https://bids.neuroimaging.io/) -
is a growing community of neuroimaging enthusiasts,
and we want to make our resources accessible
to and engaging for as many researchers as possible.

How do you know that you're a member of the BIDS community?
You're here!
You know that BIDS exists!
You're officially a member of the community.
It's THAT easy! Welcome!

Most of our discussions take place here in
[GitHub issues](#understanding-issues).
We also have a
[bids-discussion](https://groups.google.com/forum/#!forum/bids-discussion)
Google Group, although this is largely now an archive of previous conversations.

<!-- TODO update link -->
Moving forward, we encourage all members to contribute here
on [GitHub](https://github.com/bids-standard/bids-specification)
or on the [NeuroStars](https://neurostars.org/tags/bids) Discourse Forum,
under the `bids` tag.

To keep on top of new posts,
please see this guide for setting
your [topic notifications](https://meta.discourse.org/t/discourse-new-user-guide/96331#heading--topic-notifications).

As a reminder,
we expect that all contributions adhere to our [Code of Conduct](CODE_OF_CONDUCT.md).

## Contributing through GitHub

[Git](https://git-scm.com/) is a really useful tool for version control.

[GitHub](https://github.com/) sits on top of git and supports collaborative and
distributed working.

We know that it can be daunting to start using git and GitHub
if you haven't worked with them in the past,
but the BIDS maintainers are here to help you
figure out any of the jargon or confusing instructions you encounter!

In order to contribute via GitHub you'll need
to set up a free account and sign in.
Here are some
[instructions](https://help.github.com/articles/signing-up-for-a-new-github-account/)
to help you get going.
Remember that you can ask us any questions you need to along the way.

## Understanding issues

<!-- TODO update link -->
Every project on GitHub uses
[issues](https://github.com/bids-standard/bids-specification/issues)
slightly differently.

The following outlines how BIDS developers think
about communicating through issues.

**Issues** are individual pieces of work that need to be completed,
or decisions that need to be made to move the project forwards.

!!! note "General guideline"

    If you find yourself tempted to write a great big issue
    that is difficult to describe as one unit of work,
    please consider splitting it into two or more issues.

Issues are assigned [labels](#issue-labels)
that explain how they relate to the overall project's goals
and immediate next steps.

### Issue labels

<!-- TODO update links -->
The current list of labels are
[here](https://github.com/bids-standard/bids-specification/labels) and include:

-   [![Help wanted](https://img.shields.io/badge/-help%20wanted-159818.svg)](https://github.com/bids-standard/bids-specification/labels/help%20wanted)
    _These issues contain a task that a member of the team has determined we need additional help with._

    If you feel that you can contribute to one of these issues,
    we especially encourage you to do so!

-   [![Opinions wanted](https://img.shields.io/badge/-opinions%20wanted-84b6eb.svg)](https://github.com/bids-standard/bids-specification/labels/opinions%20wanted)
    _These issues hold discussions where we're especially eager for feedback._

    Ongoing discussions benefit from broad feedback.
    This label is used to highlight issues
    where decisions are being considered,
    so please join the conversation!

-   [![Community](https://img.shields.io/badge/-community-%23ddcc5f.svg)](https://github.com/bids-standard/bids-specification/labels/community)
    _These issues are related to building and supporting the BIDS community._

    In addition to the specification itself,
    we are dedicated to creating a healthy community.
    These issues highlight pieces of work
    or discussions around how we can support our members
    and make it easier to contribute.

## Using pre-commit hooks

> Git hook scripts are useful for identifying simple issues before submission to code review.

For more information on Git hooks and pre-commit, check the pre-commit [documentation](https://pre-commit.com/).

Several of the BIDS repositories have a `.pre-commit-config.yaml` configuration
at the root of the repository.

Contributors to those repositories can optionally make use of this
to run systemacially run style-checkers and linters
with every commit.

To use pre-commit this way:

Install `pre-commit` and then install the 'hooks' for that repository.

```bash
pip install pre-commit
pre-commit install
```

To uninstall the pre-commit hooks, run `pre-commit uninstall`.

## Making a change with a pull request

We appreciate all contributions to BIDS.
**THANK YOU** for helping us build these useful resources.

### 1. Comment on an existing issue or open a new issue referencing your addition

This allows other members of the BIDS team to confirm
that you aren't overlapping with work that's currently underway
and that everyone is on the same page
with the goal of the work you're going to carry out.

### 2. [Fork](https://help.github.com/articles/fork-a-repo/) [this repository](https://github.com/bids-standard/bids-specification) to your profile

This is now your own unique copy of a repository.
Changes here won't affect anyone else's work,
so it's a safe space to explore edits to the specification!

Make sure to [keep your fork up to date](https://help.github.com/articles/syncing-a-fork/) with the upstream repository,
otherwise you can end up with lots of dreaded [merge conflicts](https://help.github.com/articles/about-merge-conflicts/).

### 3. Make the changes you've discussed

Try to keep the changes focused.
If you submit a large amount of work in all in one go,
it will be much more work for whomever is reviewing your pull request.
Please detail the changes you are attempting to make.

### 4. Submit a [pull request](https://help.github.com/articles/about-pull-requests/)

Please keep the title of your pull request short
but informative in case it appears in a changelog.

Use one of the following prefixes in the title of your pull request:

-   `[ENH]` - enhancement of the repository
    that adds a new feature

-   `[FIX]` - fix of a typo, a bug, or language clarification

-   `[INFRA]` - changes to the infrastructure:
    for example automating the specification release.

-   `[MISC]` - everything else that cannot fit into another category

-   `[REF]` - Refactoring

-   `[SCHEMA]` - changes to the BIDS schema and/or related code

-   `[STY]` - Stylistic change or code formatting.

If you are opening a pull request to obtain early feedback,
but the changes are not ready to be merged
(also known as a "work in progress" pull request,
sometimes abbreviated by `WIP`)
please use a
[draft pull request](https://github.blog/2019-02-14-introducing-draft-pull-requests/).

A member of the BIDS Specification team will review your changes
to confirm that they can be merged into the main codebase.

A [review](https://help.github.com/articles/about-pull-request-reviews/)
will usually consist of a few questions
to help clarify the work you've done.
Keep an eye on your GitHub notifications
and be prepared to join in that conversation.

You can update your [fork](https://help.github.com/articles/about-forks/)
of the repository you are working on
and the pull request will automatically update with those commits.
You don't need to submit a new pull request
when you make a change in response to a review.

GitHub has a [nice introduction](https://help.github.com/articles/github-flow/)
to the pull request workflow,
but please [get in touch](#get-in-touch) if you have any questions.

## Example pull request

<img align="center" src="https://i.imgur.com/s8yELfK.png" alt="Example-Contribution" width="800"/>

## Commenting on a pull request

Our primary method of adding to or enhancing BIDS occurs in the form of
[pull requests](https://help.github.com/articles/about-pull-requests/).

BIDS Extension Proposals
([BEPs](https://docs.google.com/document/d/1pWmEEY-1-WuwBPNy5tDAxVJYQ9Een4hZJM06tQZg8X4/))
are submitted as pull requests,
and commenting on pull requests is an important way of participating in the BIDS community.

This section outlines how to comment on a pull request.

### Navigating to open pull requests

<!-- TODO update link -->
The list of pull requests can be found by clicking on the "Pull requests" tab
in the [BIDS-Specification repository](https://github.com/bids-standard/bids-specification).

![BIDS-mainpage](commenting_images/BIDS_GitHub_mainpage.png "BIDS_GitHub_mainpage")

### Selecting an open pull request

In this example we will be navigating to our
[BIDS common derivatives pull request](https://github.com/bids-standard/bids-specification/pull/265).

![BIDS-pr-list](commenting_images/BIDS_pr_list.png "BIDS_pr_list")

### Pull request description

Upon opening the pull request we see a detailed description
of what this pull request is seeking to address.
Descriptions are important for reviewers and the community
to gain context into what the pull request is achieving.

![BIDS-pr](commenting_images/BIDS_pr.png "BIDS_pr")

### Generally commenting on a pull request

At the bottom of the pull request page,
a comment box is provided for general comments and questions.

![BIDS-comment](commenting_images/BIDS_comment.png "BIDS-comment")

### Specific comments on a pull request

The proposed changes to the text of the specification
can be seen in the "Files changed" tab.
Proposed additions are displayed on a green background with a `+`
before each added line.
Proposed deletions are displayed on a red background with a `-`
before each removed line.
To comment on a specific line,
hover over it and click the blue plus sign (pictured below).
Multiple lines can be selected by clicking and dragging the plus sign.

![BIDS-specific-comment](commenting_images/BIDS_file_comment.png "BIDS-specific-comment")

#### Suggesting text

Comments on lines can contain "suggestions",
which allow you to propose specific wording for consideration.
To make a suggestion, click the plus/minus (±) icon
in the comment box (pictured below).

![BIDS-suggest-box](commenting_images/BIDS_suggest.png "BIDS-suggest")

Once the button is clicked the highlighted text will be copied
into the comment box and formatted as a
[Markdown code block](https://help.github.com/en/github/writing-on-github/creating-and-highlighting-code-blocks).

![BIDS-suggest-text](commenting_images/BIDS_suggest_text.png "BIDS-suggest-box")

The "Preview" tab in the comment box will show your suggestion
as it will be rendered.
The "Suggested change" box will highlight the differences
between the original text and your suggestion.

![BIDS-suggest-change](commenting_images/BIDS_suggest_change.png "BIDS-suggest-change")

A comment may be submitted on its own by clicking "Add single comment".
Several comments may be grouped by clicking "Start a review".
As more comments are written, accept them with "Add review comment",
and submit your review comments as a batch by clicking the "Finish your review" button.

## Accepting suggestion from a review

When others are making [suggestions to your pull request](#suggesting-text),
you have the possibility to accept directly the changes
suggested during the review through the github interface.
This can often be faster and more convenient
than making the changes locally
and then pushing those changes to update your pull request.
Moreover it gives the opportunity to give credit to the reviewers for their contribution.

To do this, you must click on the `Files changed` tab
at the top of the page of a pull request.

![BIDS_pr_files_changed](commenting_images/BIDS_pr_files_changed.png "BIDS_pr_files_changed")

From there you can browse the different files changed
and the 'diff' for each of them (what line was changed and what the change consist of).
You can also see comments and directly change suggestions made by reviewers.

You can add each suggestion one by one or group them together in a batch.

![BIDS_pr_accept_comment](commenting_images/BIDS_pr_accept_comment.png "BIDS_pr_accept_comment")

If you decide to batch the suggestions to add several of them at once,
you must scroll back to the top of the 'Files changed' page
and the `commit suggestions` button will let you add all those suggestions
as a single commit.

![BIDS_pr_commit_batch](commenting_images/BIDS_pr_commit_batch.png "BIDS_pr_commit_batch")

Once those suggestions are committed the commit information should mention the
reviewer as a co-author.

![BIDS_pr_reviewer_credit](commenting_images/BIDS_pr_reviewer_credit.png "BIDS_pr_reviewer_credit")

## Recognizing contributions

We aim to follow the [allContributors specification](https://allcontributors.org/docs/en/specification),
so we welcome and recognize a broad list of contributions types
from documentation to testing to code development.

For more concrete examples, contributions can take the form of any of the following (but are not just restricted to those):

-   contribution to the BIDS specification content,
    the BIDS schema or their maintenance
    (for example helping with the rendering of the specification, the documentation of the schema...),

-   leading or contributing to a BIDS extension proposal
    even it has not been merged,

-   developing OR contributing to a BIDS tool
    (like the BIDS validator, a converter, a BIDS app or any other type of BIDS friendly tool...),

-   regularly answering questions on Neurostars on BIDS related topics
    (for example: BIDS, fmriprep, BIDS conversion...),

-   improving the documentation around BIDS
    (like improving the BIDS website, creating a tutorial for BIDS or improving the doc of some BIDS tools...)

-   providing some example dataset to add to the BIDS examples repository...

For more ideas of what constitute a contribution,
see the [list of Emoji used by the allContributors project](https://allcontributors.org/docs/en/emoji-key)
to categorize contributions.

### Adding yourself as a BIDS contributor

If you have made any type of contributions to BIDS,
we encourage you to enter or update your information in the
[Contributors wiki page](https://github.com/bids-standard/bids-specification/wiki/Recent-Contributors)
according to the instructions listed there.

### List of BIDS contributors

You can see a list of contributors in the
[contributors appendix](https://bids-specification.readthedocs.io/en/stable/appendices/contributors.html)
of the BIDS specification.

## Thank you!

You're awesome.

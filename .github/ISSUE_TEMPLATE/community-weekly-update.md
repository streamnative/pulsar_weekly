---
name: community-weekly-update
about: Community Weekly Update Template
title: "Community Weekly Update (YYYY-MM-DD ~ YYYY-MM-DD)"
labels: ''
assignees: ''
---

> This template provides the instructions for writing a weekly update for the Pulsar community.
> Please check the items once you finish them.

The weekly updates are posted on Monday every week.

## Begin of the week

- [ ] Open a `community-weekly-update` issue under [pulsar_weekly](https://github.com/streamnative/pulsar_weekly) repo. The title of the issue is named as `Community Weekly Update (YYYY-MM-DD ~ YYYY-MM-DD)`.
- [ ] Create a [HackMD note](https://hackmd.io/0Qil4oBnS5mTWpT5etX8-Q?both) using the [community weekly update template](https://github.com/streamnative/pulsar_weekly/blob/master/template.md).
- [ ] Share the HackMD link in the issue: [LINK TO HACKMD NOTE]
    - [ ] Left a comment in this issue with the link
    - [ ] Replace `[LINK TO HACKMD NOTE]` with the link

## Contribute to the weekly update

> Fill up the weekly update note by collecting information from different channels.

### Pulsar Development

- Collect the discussions happened in the mailing lists.
- Collect the updates related to PIP development.

### Notable Bug Fix

- Go through the git log to collect the bug fixes in this week that are impacting Pulsar users.

### Notable Features

- Go through the [Pulsar Pull Requests](https://github.com/apache/pulsar/pulls) open in this week and find out the pull requests are new features.

### Ecosystem

This section is used for collecting the updates about Pulsar ecosystem, for example, Pulsar tools, integrations, and resources.
Twitter is a great channel for collecting these updates.

If you find a new tool or integration, feel free to add it to [awesome-pulsar](https://github.com/streamnative/awesome-pulsar) repo.

### Event/News

This section is used for collecting the events, meetups, and conferences related to Pulsar. Twitter and mailing lists are two great channels to learn the news.

### Blog/Article

This section is used for collecting the blog posts and articles about Pulsar, such as tutorials, best practices, user stories.

## End of the week

- [ ] Finalize the weekly update.

## On Monday

- [ ] Submit a PR to request a review, that is:
    - [ ] Create a markdown file with the name `Community Weekly Update (YYYY-MM-DD ~ YYYY-MM-DD)`.
    - [ ] Copy the contents of the HackMD note to the markdown file.
    - [ ] Push the markdown file to the [pulsar_weekly](https://github.com/streamnative/pulsar_weekly) repo.
- [ ] Incorporate comments, finalize the contents, and merge the PR.
- [ ] Post the community weekly update to the following channels:
  - [ ] Mailing list
  - [ ] Twitter
  - [ ] WeChat
- [ ] Open an issue for the next week.

# FreeIPA on OpenShift: Community Engagement plan

## Context

*FreeIPA on OpenShift* is a project to bring FreeIPA to the
OpenShift Container Platform.  High-level goals are:

- Enable organisations to host their FreeIPA identity infrastructure
  on OpenShift, to provide identity services to clients (either
  on-cluster or off-cluster, or both).

- [Operator][]-driven deployment and management of FreeIPA
  installations (consisting of multiple servers).  The operator will
  manage topology, scaling, monitoring, upgrades and backup/restore.

- Support popular cloud infrastructure providers.

- Use non-privileged workloads for secure multi-tenancy.

- Enable FreeIPA managed service offerings.

- Integrate with solutions that address other parts of the identity
  management problem space, such as Keycloak/RHSSO.
  
[Operator]: https://kubernetes.io/docs/concepts/extend-kubernetes/operator/

## Purpose of this document

This document outlines a community engagement plan, including:

- Clear communication of our project "why", including use cases.

- Transparent communication about the project goals, roadmap, status
  and challenges.

- Raise awareness of the project within the broader FreeIPA,
  OpenShift and open source identity management communities.

- Establish communication channels for interested people to engage
  with the project and its developers.

- Encourage community contributions in various forms including
  testing, bug reports, code, documentation and ideas.


## Implementation

### Project name

The initial name of the community project is *FreeIPA on OpenShift*.
This name reflects the close association with FreeIPA and leverages
the brand value.

Other names that were considered include:

- **IDMOCP** (internal name of the team at Red Hat)
- **CloudIPA**

### Code of Conduct

The project must have a code of conduct, and we should make it clear
what that is, and how violations will be dealt with.

We have agreed with the main FreeIPA project that we shall operate
under the [FreeIPA code of conduct][freeipa-coc].  We have also
confirmed that the reporting address is monitored.

[freeipa-coc]: https://github.com/freeipa/freeipa/blob/master/CODE_OF_CONDUCT.md

### Communication channels

#### IRC

FreeIPA has an established IRC channel (`#freeipa` on `libera.chat`)
used by the community.

IDMOCP will also use this channel.  If we outgrow it, then will we
look at starting a standalone channel.


#### Slack

Slack is popular in the OpenShift community.  Slack has the
advantage of keeping a permanent, searchable record of messages
exchanged, and is a more expressive medium than IRC (links,
attachments, images, etc).

We shall create a Slack channel for the IDMOCP project (channel name
to be determined).

#### Telegram

Telegram is widely used by the Kubernetes community.  We should
consider establishing a Telegram channel for our project.  It may
make sense to bridge Telegram to IRC and/or Slack.

#### Mailing list

The IDMOCP community project shall initially use the public
`freeipa-users@` and `freeipa-devel@` mailing lists.

If the IDMOCP-related traffic starts to overwhelm other FreeIPA
topics on these lists, then we will create dedicated mailing lists.


### Web resources

Establish a web "front page" for this project, which must:

- Outline the project goals and use cases, linking to pages or
  resources with more detail

- Point to the offical communication channels

- Mention and link to the **Code of Conduct**

- Contain (or link to) a **contributer guide** (see below)

- Link to recent and/or important blog posts, talks, demos, that
  give people another way to understand what the project is about.

**DECIDE** where to host this:

- Page(s) on the main FreeIPA site, with in-links from repos and the
  FreeIPA front page

- Host the site on github, e.g.
  `https://freeipa.github.io/freeipa-openshift`.

- Somewhere else?

### Contributor guide

We must publish a contributor guide that includes:

- comprehensive list of code and container image repositories

- how-tos for building and running every part of the project
  (container, operator, deployment tools, etc)

- how to raise issues, feature requests or other proposals, what
  those proposals need to contain (design, test plan, etc), and how
  they will be reviewed

- how to test / how to write tests

- style guide (`gofmt` does a fair bit of work for us here)

### Code, issues and pull requests, artifacts

- All team code repositories should be public.  (Repositories that
  are currently private should be carefully checked for secrets in
  the history, scrubbing them before making them public.)  We will
  host our code repositories on **GitHub**.

- Operator code and the FreeIPA container code are licensed under
  **Apache License 2.0.**  Licenses for other programs (e.g.
  deployment tools) shall be decided separately and transparently.

- Create issue and pull request templates to assist contributors to
  more easily provide the information we want to receive.

- We will host container images on **Quay.io**.

### Building awareness and engagement

- **Blog posts:** team members are encouraged to blog about their
  work, challenges and results.  Posts can be shared on public
  mailing lists and websites.  Developer blogs can be added to the
  http://planet.freeipa.org/ blog roll.  Seek opportunities to
  publish articles on blogs with large audiences, such as
  https://developers.redhat.com.

- **Conference and user-group presentations:** team members are
  encouraged to propose (and if accepted, deliver) conference
  presentations about the project.  These will raise awareness and
  prompt discussion, sharing of ideas, and testing.

- **Demos:** when possible, record or deliver live demos of
  progress.  These can be shared, and can be linked or embedded on
  the web site.

- **Workshops:** develop workshops or walkthrough for people to test
  and experiment with the software.  Make sure that feedback
  channels are clearly advertised.  If delivering workshops in
  person, a quick follow-up survey may be a good idea.


### Recognition of contributions

Ensure that contributions are properly recognised.  This can take
the form of:

- Prompt word of thanks for every kind of contribution (issues, PRs,
  ideas/suggestions)

- `CONTRIBUTORS` file in the repository which was contributed to

- "Credits" page on the web site

- Acknowledgement of bigger contributions in blog posts or similar.

- Anything else that seems appropriate.


### Transparency

- Documents about the roadmap, progress and project operations
  should be public.  The web pages or code repos (or both) are the
  sensible place to document these things.

- Where possible, documents should be in version control so that
  community members can both observe the history, and propose
  changes.


## Evaluation

After implementation, we must periodically evaluate whether or how
well each implemented measure helps to achieve the goals.  Data that
may be useful in the evaluation could include:

- The number of distinct organisations or individuals participating
  in the project, via the various channels.  Note that there is a
  project-wide and per-channel aspect to the assessment.  Channels
  that did not show significant engagement may be dead weight.

- The number of distinct use cases that have emerged via issues,
  questions/discussions, pull requests, etc.

- Feedback received about the project and developed resources.

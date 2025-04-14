# Awesome Release Management [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of tools, resources, and best practices for effective and modern software release management.

**Release Management** is a critical process in the software delivery lifecycle. It encompasses the planning, scheduling, coordination, and deployment of software releases across various environments. This list aims to provide developers, DevOps engineers, and release managers with high-quality resources to improve automation, reliability, traceability, and strategy in their release workflows.

Inspired by [awesome](https://github.com/sindresorhus/awesome).

---

## Contents

- [Fundamentals](#fundamentals)
- [Guides & Best Practices](#guides--best-practices)
- [Release Management Tools](#release-management-tools)
  - [Automated Release Tools](#automated-release-tools)
  - [Semantic Versioning](#semantic-versioning)
  - [Changelog Generators](#changelog-generators)
  - [Orchestration & CD](#orchestration--cd)
- [CI/CD Integrations](#cicd-integrations)
- [Version Control Strategies](#version-control-strategies)
- [Case Studies & Postmortems](#case-studies--postmortems)
- [Books & Courses](#books--courses)
- [Community](#community)
- [Related Awesome Lists](#related-awesome-lists)

---

## Fundamentals

- [Release Management (Wikipedia)](https://en.wikipedia.org/wiki/Release_management)
- [Software Release Life Cycle](https://en.wikipedia.org/wiki/Software_release_life_cycle)
- [How ITIL Release Management works](https://www.knowledgehut.com/blog/it-service-management/itil-release-management)
- [ITSM Release Management](http://www.project-open.com/en/process-itsm-release-management)
- [Release Management in Devops](https://www.peerbits.com/blog/complete-guide-to-release-management-in-devops.html))

---

## Guides & Best Practices

- [Release Strategy for Devops](https://www.pmi.org/disciplined-agile/process/release-management/devops-strategies)
- [7 Ways to improve your Software Release Management](https://www.cio.com/article/276415/developer-7-ways-to-improve-your-software-release-management.html)
- [Release Management Explained: Dev To Prod Deployment Process](https://devopscube.com/release-management-explained/)

---

## Release Management Tools

### Automated Release Tools

- [semantic-release](https://github.com/semantic-release/semantic-release) - Fully automated version management and changelog generation based on semantic commits.
- [Release Please](https://github.com/googleapis/release-please) - GitHub automation for managing releases with changelogs.
- [changesets](https://github.com/changesets/changesets) - A release tool specifically built for monorepos.

### Semantic Versioning

- [SemVer.org](https://semver.org/)
- [Conventional Commits](https://www.conventionalcommits.org/)
- [Commitizen](https://github.com/commitizen/cz-cli) - Tool to guide developers in writing proper commit messages.

### Changelog Generators

- [Keep a Changelog](https://keepachangelog.com/)
- [auto-changelog](https://github.com/CookPete/auto-changelog)
- [github-changelog-generator](https://github.com/github-changelog-generator/github-changelog-generator)

### Orchestration & CD

- [GitHub Actions](https://github.com/features/actions)
- [GitLab CI/CD](https://docs.gitlab.com/ee/ci/)
- [CircleCI](https://circleci.com/)
- [Jenkins](https://www.jenkins.io/)
- [Argo CD](https://argo-cd.readthedocs.io/en/stable/) - Declarative GitOps CD for Kubernetes.
- [FluxCD](https://fluxcd.io/) - Kubernetes-native continuous delivery.

---

## CI/CD Integrations

- [Publishing Node.js Packages with GitHub Actions](https://docs.github.com/en/actions/publishing-packages/publishing-nodejs-packages)
- [GitLab Releases](https://docs.gitlab.com/ee/user/project/releases/)
- [Docker CI/CD with GitHub Actions](https://docs.docker.com/ci-cd/github-actions/)

---

## Version Control Strategies

- [Git Flow](https://nvie.com/posts/a-successful-git-branching-model/)
- [Trunk-Based Development](https://trunkbaseddevelopment.com/)
- [Monorepo vs Polyrepo](https://monorepo.tools/)

---

## Case Studies

- [Google SRE Workbook: Release Engineering](https://sre.google/sre-book/release-engineering/)

---

## Books & Courses

**Books**

- [*The DevOps Handbook*](https://www.amazon.com/DevOps-Handbook-World-Class-Reliability-Organizations/dp/1950508404/) by Gene Kim, Jez Humble, Patrick Debois, John Willis
- [*The Phoenix Project*](https://www.amazon.com/The-Phoenix-Project-audiobook/dp/B00VATFAMI/) by Gene Kim, Kevin Behr, George Spafford
- [*Site Reliability Engineering*](https://www.amazon.com/Site-Reliability-Engineering-Production-Systems/dp/B08VKWBJFS/) by Betsy Beyer, Chris Jones, Jennifer Petoff, Niall Richard Murphy

**Courses**

- [Pluralsight: Release Management](https://www.pluralsight.com/courses/release-management)
- [Udemy: CI/CD and Release Management](https://www.udemy.com/course/devops-ci-cd-release-management/)
- [Microsoft Learn: Introduction to Release Pipelines](https://learn.microsoft.com/en-us/training/modules/introduction-release-pipelines/)

---

## Community

- [r/devops on Reddit](https://www.reddit.com/r/devops/)
- [DevOps Stack Exchange](https://devops.stackexchange.com/)
- [semantic-release Discussions](https://github.com/semantic-release/semantic-release/discussions)

---

## Related Awesome Lists

- [awesome-devops](https://github.com/tiimgreen/awesome-devops)
- [awesome-ciandcd](https://github.com/cicdops/awesome-ciandcd)
- [awesome-gitops](https://github.com/weaveworks/awesome-gitops)
- [awesome-sre](https://github.com/dastergon/awesome-sre)

---

## Misc

- [Release Management in Open Source projects](http://oss-watch.ac.uk/resources/releasemanagement)
- [Should I deploy today?](https://shouldideploy.today/)

---

## Contributing

Contributions are welcome! Please see [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

---

## License

[MIT](LICENSE)

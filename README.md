# Awesome Release Management [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of tools, resources, and best practices for effective and modern software release management.

**Release Management** is a critical process in the software delivery lifecycle. It encompasses the planning, scheduling, coordination, and deployment of software releases across various environments. This list aims to provide developers, DevOps engineers, and release managers with high-quality resources to improve automation, reliability, traceability, and strategy in their release workflows.

Inspired by [awesome](https://github.com/sindresorhus/awesome).

---

## Contents

* [Fundamentals](#fundamentals)
* [Guides & Best Practices](#guides--best-practices)
* [Release Management Tools](#release-management-tools)
  + [Automated Release Tools](#automated-release-tools)
  + [Semantic Versioning](#semantic-versioning)
  + [Release Monitoring & EOL Tracking](#release-monitoring--eol-tracking)
  + [Changelog Generators](#changelog-generators)
  + [Orchestration & CD](#orchestration--cd)
* [CI/CD Integrations](#cicd-integrations)
* [Feature Flags & Progressive Delivery](#feature-flags--progressive-delivery)
* [Deployment Strategies](#deployment-strategies)
* [Release Metrics](#release-metrics)
* [Database Migrations](#database-migrations)
* [Dependency Management](#dependency-management)
* [Version Control Strategies](#version-control-strategies)
* [Case Studies & Postmortems](#case-studies--postmortems)
* [Books & Courses](#books--courses)
* [Community](#community)
* [Related Awesome Lists](#related-awesome-lists)

---

## Fundamentals

* [Release Management (Wikipedia)](https://en.wikipedia.org/wiki/Release_management)
* [Software Release Life Cycle](https://en.wikipedia.org/wiki/Software_release_life_cycle)
* [How ITIL Release Management works](https://www.knowledgehut.com/blog/it-service-management/itil-release-management)
* [ITSM Release Management](http://www.project-open.com/en/process-itsm-release-management)
* [Release Management in Devops](https://www.peerbits.com/blog/complete-guide-to-release-management-in-devops.html)

---

## Guides & Best Practices

* [Release Strategy for Devops](https://www.pmi.org/disciplined-agile/process/release-management/devops-strategies)
* [7 Ways to improve your Software Release Management](https://www.cio.com/article/276415/developer-7-ways-to-improve-your-software-release-management.html)
* [Release Management Explained: Dev To Prod Deployment Process](https://devopscube.com/release-management-explained/)
* [Continuous Delivery Patterns and Anti-Patterns](https://continuousdelivery.com/implementing/patterns/) - Reference patterns for building reliable release pipelines.
* [Google's Engineering Practices: Release Engineering](https://abseil.io/resources/swe-book/html/ch24.html) - Chapter from the Software Engineering at Google book.

---

## Release Management Tools

### Automated Release Tools

* [semantic-release](https://github.com/semantic-release/semantic-release) - Fully automated version management and changelog generation based on semantic commits.
* [Release Please](https://github.com/googleapis/release-please) - GitHub automation for managing releases with changelogs.
* [changesets](https://github.com/changesets/changesets) - A release tool specifically built for monorepos.
* [GoReleaser](https://goreleaser.com/) - Build, package, and release Go projects with a single command. Supports Docker, Homebrew, Snapcraft, and more.
* [release-drafter](https://github.com/release-drafter/release-drafter) - Drafts your next release notes as pull requests are merged into the default branch.
* [Nx Release](https://nx.dev/features/manage-releases) - First-class release management for monorepos, including versioning, changelog generation, and publishing.

### Release Monitoring & EOL Tracking

* [ReleaseRun](https://releaserun.com) - Track software releases, breaking changes, and EOL dates across 13+ tech stacks (Node.js, Python, Go, Kubernetes, PostgreSQL, and more). Free daily briefings and a release index.
* [endoflife.date](https://endoflife.date/) - Quickly checks EOL dates and support cycles for software, frameworks, and operating systems.

### Semantic Versioning

* [SemVer.org](https://semver.org/)
* [Conventional Commits](https://www.conventionalcommits.org/)
* [Commitizen](https://github.com/commitizen/cz-cli) - Tool to guide developers in writing proper commit messages.

### Changelog Generators

* [Keep a Changelog](https://keepachangelog.com/)
* [auto-changelog](https://github.com/CookPete/auto-changelog)
* [github-changelog-generator](https://github.com/github-changelog-generator/github-changelog-generator)
* [git-cliff](https://github.com/orhun/git-cliff) - Highly customizable changelog generator based on conventional commits.

### Orchestration & CD

* [GitHub Actions](https://github.com/features/actions)
* [GitLab CI/CD](https://docs.gitlab.com/ee/ci/)
* [CircleCI](https://circleci.com/)
* [Jenkins](https://www.jenkins.io/)
* [Argo CD](https://argo-cd.readthedocs.io/en/stable/) - Declarative GitOps CD for Kubernetes.
* [FluxCD](https://fluxcd.io/) - Kubernetes-native continuous delivery.
* [Tekton](https://tekton.dev/) - Cloud-native CI/CD framework for Kubernetes, part of the CD Foundation.
* [Spinnaker](https://spinnaker.io/) - Multi-cloud continuous delivery platform built for enterprise scale (originally by Netflix).
* [Harness](https://harness.io/) - AI-powered software delivery platform with built-in deployment verification and rollback.
* [Azure DevOps Pipelines](https://azure.microsoft.com/en-us/products/devops/pipelines) - Cloud-hosted pipelines for building, testing, and releasing software.
* [AWS CodePipeline](https://aws.amazon.com/codepipeline/) - Fully managed continuous delivery service in AWS.
* [Buildkite](https://buildkite.com/) - Scalable CI/CD platform that runs agents on your own infrastructure.

---

## CI/CD Integrations

* [Publishing Node.js Packages with GitHub Actions](https://docs.github.com/en/actions/publishing-packages/publishing-nodejs-packages)
* [GitLab Releases](https://docs.gitlab.com/ee/user/project/releases/)
* [Docker CI/CD with GitHub Actions](https://docs.docker.com/ci-cd/github-actions/)
* [Release assets with GoReleaser + GitHub Actions](https://goreleaser.com/ci/actions/)

---

## Feature Flags & Progressive Delivery

Feature flags decouple deployment from release, enabling dark launches, A/B testing, and instant rollbacks without redeployment.

* [Feature Toggles (Martin Fowler)](https://martinfowler.com/articles/feature-toggles.html) - Seminal article on feature toggle patterns and pitfalls.
* [OpenFeature](https://openfeature.dev/) - Open standard for feature flag management, backed by the CNCF.
* [LaunchDarkly](https://launchdarkly.com/) - Enterprise-grade feature management platform with SDKs for every major language.
* [Unleash](https://github.com/Unleash/unleash) - Open source feature flag service with a self-hosted option.
* [Flagsmith](https://github.com/Flagsmith/flagsmith) - Open source feature flag and remote config service.
* [GrowthBook](https://github.com/growthbook/growthbook) - Open source feature flags and A/B testing platform.
* [Flipt](https://github.com/flipt-io/flipt) - Self-hosted, GitOps-friendly feature flag solution.

---

## Deployment Strategies

Patterns for releasing software safely with minimal user impact.

* [Blue-Green Deployments](https://martinfowler.com/bliki/BlueGreenDeployment.html) - Martin Fowler's definition and rationale for zero-downtime environment switching.
* [Canary Releases](https://martinfowler.com/bliki/CanaryRelease.html) - Gradually roll out changes to a subset of users before full deployment.
* [Argo Rollouts](https://argo-rollouts.readthedocs.io/) - Kubernetes controller for advanced deployment strategies including canary, blue-green, and A/B.
* [Flagger](https://flagger.app/) - Progressive delivery operator for Kubernetes with automated canary analysis and rollback.
* [Octopus Deploy](https://octopus.com/) - Deployment automation with first-class support for multi-environment release pipelines.
* [Deployment Strategies Explained](https://dev.to/mostlyjason/intro-to-deployment-strategies-blue-green-canary-and-more-3a3) - Practical overview of rolling, canary, shadow, and blue-green strategies.

---

## Release Metrics

Measuring your release process is the only way to improve it.

* [DORA Metrics](https://dora.dev/) - The four key metrics: Deployment Frequency, Lead Time for Changes, Change Failure Rate, and Time to Restore Service.
* [Four Keys](https://github.com/dora-team/fourkeys) - Open source project by Google to measure DORA metrics from your CI/CD pipelines.
* [SPACE Framework](https://queue.acm.org/detail.cfm?id=3454124) - A multi-dimensional developer productivity framework from Microsoft Research and GitHub.
* [Sleuth](https://www.sleuth.io/) - DORA metrics tracking tool that integrates with GitHub, Jira, and PagerDuty.
* [LinearB](https://linearb.io/) - Engineering metrics platform with automated workflow benchmarks tied to release health.
* [Accelerate: Key Metrics](https://itrevolution.com/articles/accelerate-key-metrics/) - Summary of the research-backed metrics from the *Accelerate* book.

---

## Database Migrations

Coordinating schema changes safely across releases is one of the hardest parts of release management.

* [Evolutionary Database Design](https://martinfowler.com/articles/evodb.html) - Martin Fowler's foundational article on schema changes in continuous delivery.
* [Flyway](https://flywaydb.org/) - Version-controlled database migrations with strong CI/CD integration.
* [Liquibase](https://www.liquibase.org/) - Open source database schema change management with XML/YAML/JSON/SQL support.
* [Atlas](https://atlasgo.io/) - Modern, declarative database schema-as-code tool with drift detection.
* [Expand-Contract Pattern](https://openpracticelibrary.com/practice/expand-and-contract-pattern/) - Pattern for backward-compatible schema migrations that enable zero-downtime releases.

---

## Dependency Management

Keeping dependencies up-to-date is integral to healthy, predictable releases.

* [Renovate](https://github.com/renovateapp/renovate) - Automated dependency updates with highly configurable grouping, scheduling, and automerge.
* [Dependabot](https://docs.github.com/en/code-security/dependabot) - GitHub-native dependency updates and security alerts.
* [Snyk](https://snyk.io/) - Developer security platform that catches vulnerable dependencies before they reach production.
* [OWASP Dependency-Check](https://owasp.org/www-project-dependency-check/) - Identifies known vulnerabilities in project dependencies.

---

## Version Control Strategies

* [Git Flow](https://nvie.com/posts/a-successful-git-branching-model/)
* [GitHub Flow](https://docs.github.com/en/get-started/using-github/github-flow) - Lightweight, branch-based workflow recommended for teams deploying regularly.
* [GitLab Flow](https://about.gitlab.com/topics/version-control/what-is-gitlab-flow/) - Balances Git Flow's structure with the simplicity of Trunk-Based Development.
* [Trunk-Based Development](https://trunkbaseddevelopment.com/)
* [Monorepo vs Polyrepo](https://monorepo.tools/)
* [Ship / Show / Ask](https://martinfowler.com/articles/ship-show-ask.html) - A branching strategy that categorizes changes by the level of review they require.

---

## Case Studies & Postmortems

* [Google SRE Workbook: Release Engineering](https://sre.google/sre-book/release-engineering/)
* [GitHub Engineering Blog](https://github.blog/tag/engineering/) - Posts covering major incidents and lessons learned.
* [AWS Post-Event Summaries](https://aws.amazon.com/premiumsupport/technology/pes/) - Official summaries of significant AWS service events.
* [Netflix Tech Blog: Deployment](https://netflixtechblog.com/tagged/deployment) - Case studies on progressive delivery, canary analysis, and release automation at scale.
* [Honeycomb Production Excellence](https://www.honeycomb.io/blog) - Articles on observability-driven deployments and release practices.

---

## Books & Courses

**Books**

* [*The DevOps Handbook*](https://www.amazon.com/DevOps-Handbook-World-Class-Reliability-Organizations/dp/1950508404/) by Gene Kim, Jez Humble, Patrick Debois, John Willis
* [*The Phoenix Project*](https://www.amazon.com/The-Phoenix-Project-audiobook/dp/B00VATFAMI/) by Gene Kim, Kevin Behr, George Spafford
* [*Accelerate*](https://www.amazon.com/Accelerate-Software-Performing-Technology-Organizations/dp/1942788339/) by Nicole Forsgren, Jez Humble & Gene Kim — Data-driven research on what separates high-performing software delivery teams.
* [*Continuous Delivery*](https://www.amazon.com/Continuous-Delivery-Deployment-Automation-Addison-Wesley/dp/0321601912/) by Jez Humble & David Farley — The foundational text on automated, reliable software releases.
* [*Site Reliability Engineering*](https://www.amazon.com/Site-Reliability-Engineering-Production-Systems/dp/B08VKWBJFS/) by Betsy Beyer, Chris Jones, Jennifer Petoff, Niall Richard Murphy
* [*Team Topologies*](https://teamtopologies.com/book) by Matthew Skelton & Manuel Pais — How team structures affect deployment flow and release frequency.

**Courses**

* [Skillsoft: Build & Release Engineering Best Practices](https://www.skillsoft.com/course/build-release-engineering-best-practices-release-management-2a3707c5-7cd2-468a-b950-7fc86264a898)
* [Pluralsight: Agile Release Management](https://www.pluralsight.com/courses/agile-release-management)
* [Linux Foundation: CI/CD with Tekton](https://training.linuxfoundation.org/training/introduction-to-tekton-lfs268/) - Free course on building cloud-native pipelines.

---

## Community

* [r/devops on Reddit](https://www.reddit.com/r/devops/)
* [DevOps Stack Exchange](https://devops.stackexchange.com/)
* [semantic-release Discussions](https://github.com/semantic-release/semantic-release/discussions)
* [CD Foundation](https://cd.foundation/) - Vendor-neutral home for CI/CD projects (Tekton, Jenkins, Spinnaker, etc.).
* [CNCF Slack — #ci-cd channel](https://slack.cncf.io/) - Active community around cloud-native delivery tooling.
* [DevOpsDays](https://devopsdays.org/) - Community-driven events held worldwide, covering release practices, culture, and tooling.

---

## Related Awesome Lists

* [awesome-devops](https://github.com/wmariuss/awesome-devops)
* [awesome-ciandcd](https://github.com/cicdops/awesome-ciandcd)
* [awesome-gitops](https://github.com/weaveworks/awesome-gitops)
* [awesome-sre](https://github.com/dastergon/awesome-sre)
* [awesome-chaos-engineering](https://github.com/dastergon/awesome-chaos-engineering) - Chaos and resilience testing are increasingly part of release validation.

---

## Misc

* [Release Management in Open Source projects](http://oss-watch.ac.uk/resources/releasemanagement)
* [Should I deploy today?](https://shouldideploy.today/)
* [Is it Friday?](https://isitfriday.org/) - The eternal question every release manager must answer.

---

## Contributing

Contributions are welcome! Please see [CONTRIBUTING.md](https://github.com/miguelsalva/awesome-release-management/blob/master/CONTRIBUTING.md) for guidelines.

---

## License

[Creative Commons Attribution Share Alike 4.0 International](https://github.com/miguelsalva/awesome-release-management/blob/master/LICENSE)

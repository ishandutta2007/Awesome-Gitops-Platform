# Awesome-Gitops-Platform

## Top GitOps Platforms Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**

*Focused on Declarative Continuous Delivery, Kubernetes Reconciliation, Multi-Cluster GitOps & Progressive Delivery*

**Last updated: September 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **GitOps**. These systems continuously reconcile Kubernetes (and related) desired state from Git, enabling declarative continuous delivery, multi-cluster management, and progressive delivery workflows.



**Examples** include Argo CD Enterprise, Flux CD Enterprise, Codefresh GitOps, Akuity, Rafay Kubernetes Operations, Harness GitOps, Weave GitOps, Humanitec, Qovery, and Spectro Cloud (the category leaders).



**Open-source emphasis**: GitOps is built on outstanding open-source foundations. **Argo CD** and **Flux** (both CNCF graduated) are the dominant open engines; most commercial platforms build on or integrate them. This section is heavily expanded.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-products)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms

- **[Argo CD Enterprise / Akuity](https://akuity.io/)**  

  Enterprise distribution and managed offerings around Argo CD, providing support, multi-cluster control planes, and operational features for production GitOps.



- **[Flux CD Enterprise / Weave GitOps](https://www.weave.works/)**  

  Enterprise and commercial offerings built on Flux and the GitOps Toolkit, with additional UI, policy, and platform features.



- **[Codefresh GitOps](https://codefresh.io/)**  

  GitOps platform built on Argo CD with rich pipelines, UI, and enterprise continuous delivery capabilities.



- **[Harness GitOps](https://www.harness.io/)**  

  GitOps capabilities within the Harness continuous delivery platform, typically using Argo CD as the reconciler.



- **[Rafay Kubernetes Operations Platform](https://rafay.co/)**  

  Kubernetes operations and GitOps-oriented platform for multi-cluster management, policy, and application delivery.



- **[Humanitec](https://humanitec.com/)**  

  Internal developer platform with strong GitOps and score-based application deployment patterns on Kubernetes.



- **[Qovery](https://www.qovery.com/)**  

  Developer-centric deployment platform with GitOps-style workflows for applications on Kubernetes and cloud infrastructure.



- **[Spectro Cloud Palette](https://www.spectrocloud.com/)**  

  Kubernetes management platform with GitOps-driven cluster and application lifecycle capabilities.



- **[Other enterprise GitOps / IDP offerings](https://www.example.com/)**  

  Additional commercial platforms that productize Argo CD, Flux, or similar reconciliation engines with support and governance.



## Open-Source GitHub Projects

- **[Argo CD](https://github.com/argoproj/argo-cd)**  

  Leading open-source declarative continuous delivery tool for Kubernetes—Git as source of truth, rich UI, multi-cluster support, ApplicationSets, and strong ecosystem (CNCF graduated).



- **[Flux (Flux2 / GitOps Toolkit)](https://github.com/fluxcd/flux2)**  

  Open and extensible continuous delivery solution for Kubernetes powered by the GitOps Toolkit—composible controllers for sources, Kustomize, Helm, image automation, and notifications (CNCF graduated).



- **[Argo Rollouts](https://github.com/argoproj/argo-rollouts)**  

  Open-source progressive delivery controller for Kubernetes (canary, blue-green) that integrates tightly with Argo CD.



- **[Flagger](https://github.com/fluxcd/flagger)**  

  Open-source progressive delivery tool that works with Flux (and others) for canary, A/B, and blue-green deployments.



- **[Argo Workflows](https://github.com/argoproj/argo-workflows)**  

  Open-source workflow engine for Kubernetes often used alongside Argo CD for CI and complex delivery pipelines.



- **[Weave GitOps OSS / related UIs](https://github.com/)**  

  Open-source UIs and developer-platform components built on Flux for simplified GitOps experiences.



- **[Config and policy open tools (Kyverno, OPA, etc.)](https://github.com/)**  

  Open policy engines commonly paired with GitOps for admission control and compliance.



- **[Secrets management open tools (SOPS, External Secrets, etc.)](https://github.com/)**  

  Open solutions for managing secrets in GitOps workflows without storing plaintext in Git.



- **[Image update and automation controllers](https://github.com/)**  

  Open components (including Flux image automation) that detect new container images and open PRs or update Git.



- **[Multi-cluster and ApplicationSet open patterns](https://github.com/)**  

  Community examples and tools for managing many clusters and tenants with Argo CD or Flux.



### Additional Strong Open-Source Options

- Choosing **Argo CD** when you want a rich UI, application-centric model, and centralized multi-cluster control.

- Choosing **Flux** when you prefer a lightweight, Kubernetes-native, composable controller architecture.

- Combining **Argo CD + Argo Rollouts** or **Flux + Flagger** for progressive delivery.

- Layering open policy and secrets tools on top of either engine for production hardening.

- Accepting that enterprise support, hosted control planes, advanced RBAC/UI, and commercial SLAs still drive adoption of platforms built on these open cores (Akuity, Codefresh, Harness, Weave, etc.).

- Focusing open-source efforts on portability, Git as single source of truth, and avoiding proprietary reconciliation lock-in.



**Frameworks for building custom systems**: Store desired state in Git → run Argo CD or Flux controllers in cluster(s) → reconcile continuously → add progressive delivery with Rollouts/Flagger → enforce policy with Kyverno/OPA → manage secrets with SOPS/External Secrets. Suitable for any team running Kubernetes. Most production GitOps deployments are powered by Argo CD or Flux, with commercial platforms providing support and extra features on top.



## How to Contribute

1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.

- GitOps systems control production deployments. Misconfiguration can cause outages or security issues. Proper RBAC, secrets handling, and change control are essential. This list is not operational or security advice.



---

**Made for platform engineers, SREs, and Kubernetes teams practicing declarative continuous delivery.**

Let's keep GitOps open, reliable, and community-driven.

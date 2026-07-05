<div align="center">

# Hamza Hassanain

**Cloud &amp; Full-Stack Engineer** · AWS Certified Solutions Architect – Associate
TypeScript · Node · AWS · the code-execution infrastructure behind **Repovive**
Cairo, Egypt 🇪🇬 · 2× ACPC Finalist

[![AWS SAA](https://img.shields.io/badge/AWS_Certified-Solutions_Architect_–_Associate-FF9900?style=flat-square&logo=amazonwebservices&logoColor=white)](https://www.credly.com/badges/f0ec63f3-e2ce-4173-bfdd-902bc72cbb0a/public_url)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/hamza-hassanain-ha067)
[![X](https://img.shields.io/badge/X-0A0A0A?style=flat-square&logo=x&logoColor=white)](https://x.com/HamzaHassanain0)
[![Dev.to](https://img.shields.io/badge/Dev.to-0A0A0A?style=flat-square&logo=devdotto&logoColor=white)](https://dev.to/hamzahassanain0)
[![Codeforces](https://img.shields.io/badge/Codeforces-Hmzaawy-1F8ACB?style=flat-square&logo=codeforces&logoColor=white)](https://codeforces.com/profile/Hmzaawy)
[![GitLab](https://img.shields.io/badge/GitLab-HamzaHassanain-FC6D26?style=flat-square&logo=gitlab&logoColor=white)](https://gitlab.com/HamzaHassanain)

</div>

I build **cloud and full-stack systems** — TypeScript/Node backends on **AWS**, with Redis, MongoDB, and
Express — and the **code-execution infrastructure behind [Repovive](https://github.com/Repovive)**, an online
judge built on top of Judge0. I'm an **AWS Certified Solutions Architect – Associate**. I also contribute
upstream to **LLVM/Clang, Swift NIO, and GitLab**, and build low-level systems projects — a memory allocator,
a POSIX shell, a C++ web framework — to understand how the layers underneath actually work.

---

## 🎓 Certification

[![AWS Certified Solutions Architect – Associate](https://img.shields.io/badge/AWS%20Certified-Solutions%20Architect%20–%20Associate-FF9900?style=for-the-badge&logo=amazonwebservices&logoColor=white)](https://www.credly.com/badges/f0ec63f3-e2ce-4173-bfdd-902bc72cbb0a/public_url)

**AWS Certified Solutions Architect – Associate** — Amazon Web Services · [verify on Credly ↗](https://www.credly.com/badges/f0ec63f3-e2ce-4173-bfdd-902bc72cbb0a/public_url)

---

## 💼 Experience

### Repovive — Backend &amp; Infrastructure Engineer <sub>· competitive-programming judge &amp; contest platform</sub>

- Led end-to-end design and build of Repovive's **judge infrastructure** (`judge1`, built on **Judge0**) — a code-execution and auto-grading system with isolated sandboxes, multi-language compilation, and agentic test-case generation — scaling concurrent executions **~10× (50 → 500+)**.
- Re-architected the platform from **serverless to a self-managed Docker / Nginx / Redis stack**, cutting infrastructure cost **~95%** while increasing throughput.
- Sandboxed **20+ languages** with resource-limited Docker images; redesigned the data layer to serve **50 MB+** premium contest test-case sets.
- Built a **real-time collaborative workspace** — WebSockets + **Yjs CRDTs** for conflict-free sync and a Monaco-based editor for live multi-user editing.
- **Co-founded Repovive Build v2**, an AI-assisted IDE for problem authoring: an event-driven agent pipeline of **28 tools**, guarded by server-side execution locks + atomic cancellation, sustaining **10-minute streaming agent sessions**.

---

## 🛠️ Featured projects

### ☁️ Cloud, full-stack &amp; infrastructure

<table>
<tr>
<td width="50%" valign="top">

#### [CP Judge — AWS Reference Architecture](https://github.com/HamzaHassanain/Competitive-Programming-Judge-AWS-Reference-Architecture)
A full **AWS reference architecture** for a contest judge (Manara AWS SAA capstone): Judge0 `isolate` on ECS-on-EC2, Fargate orchestrator, Spot mixed-ASG scaled on queue depth, Step Functions + Bedrock cheating-detection. 7 views · 9 design decisions.

![AWS](https://img.shields.io/badge/AWS-Well--Architected-232F3E?logo=amazonwebservices&logoColor=white) ![SAA](https://img.shields.io/badge/Solutions-Architect-FF9900?logo=amazonaws&logoColor=white)

</td>
<td width="50%" valign="top">

#### [Distributed Code Runner](https://github.com/HamzaHassanain/distributed-code-runner-)
A **shared-nothing distributed code-execution platform** — Next.js client, an API gateway, and a sandboxed Judge0 execution cluster behind a managed load balancer.

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white) ![Judge0](https://img.shields.io/badge/Judge0-sandbox-f59e0b)

</td>
</tr>
<tr>
<td width="50%" valign="top">

#### [SigmaLoop](https://github.com/sigma-loop) &nbsp;·&nbsp; [live ↗](https://sigmaloop.dpdns.org/)
A personalized **AI tutor** that generates entire programming-and-math curricula on demand — code graded in a Judge0 sandbox, math proofs by a confidence-scored LLM, hints from a self-fine-tuned **Qwen2.5-Coder-7B**. *(Team project.)*

![React 19](https://img.shields.io/badge/React-19-2dd4bf?logo=react&logoColor=white) ![Node](https://img.shields.io/badge/Node-Express-6366f1?logo=nodedotjs&logoColor=white) ![AI](https://img.shields.io/badge/AI-Qwen%20%2F%20DeepSeek-3b82f6)

</td>
<td width="50%" valign="top">

#### [Polyman](https://github.com/HamzaHassanain/polyman) &nbsp;![stars](https://img.shields.io/github/stars/HamzaHassanain/polyman?style=flat-square&label=%E2%AD%90&color=f59e0b)
A **CLI for Codeforces problem setters** — create, test, and push problems to Polygon without leaving the terminal.

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white) ![CLI](https://img.shields.io/badge/CLI-tool-black)

</td>
</tr>
</table>

### 🔩 Systems — built from scratch to learn the fundamentals

<table>
<tr>
<td width="33%" valign="top">

#### [HAllocator](https://github.com/HamzaHassanain/HAllocator)
STL-compatible **C++23 memory allocator** — red-black-tree best-fit + free-block coalescing, GoogleTest-covered.

![C++23](https://img.shields.io/badge/C%2B%2B-23-00599C?logo=cplusplus&logoColor=white)

</td>
<td width="33%" valign="top">

#### [Hesh](https://github.com/HamzaHassanain/hesh)
A **POSIX shell** from scratch — process control, pipes, redirection, raw syscalls.

![C++](https://img.shields.io/badge/C%2B%2B-00599C?logo=cplusplus&logoColor=white)

</td>
<td width="33%" valign="top">

#### [cppress](https://github.com/HamzaHassanain/cppress)
An **Express-style web framework for C++**, on my own [socket](https://github.com/HamzaHassanain/hamza-socket-lib) / [HTTP](https://github.com/HamzaHassanain/hamza-http-server-lib) / [JSON](https://github.com/HamzaHassanain/hamza-json-parser) libs.

![C++](https://img.shields.io/badge/C%2B%2B-00599C?logo=cplusplus&logoColor=white)

</td>
</tr>
</table>

<sub>Also: <b><a href="https://github.com/HamzaHassanain/Leetcode_SQL_50_Study_Plan">LeetCode SQL 50</a></b> ⭐46 · <b><a href="https://github.com/HamzaHassanain/CP_Templates">CP Templates</a></b> ⭐18</sub>

---

## 🔩 Upstream open-source contributions

> Every link below is a **merged** pull/merge request — they survive the click.

### <img src="https://img.shields.io/badge/GitLab-FC6D26?logo=gitlab&logoColor=white" height="20"/> &nbsp;11 merged MRs across 3 `gitlab-org` projects

- **[Go SDK — `client-go`](https://gitlab.com/gitlab-org/api/client-go)** — 6 MRs adding typed group-integration support to GitLab's official Go client: **Slack, Jira, Microsoft Teams, Mattermost, Harbor**, and **Discord / Telegram / Matrix / Google Chat**.
- **[Terraform provider](https://gitlab.com/gitlab-org/terraform-provider-gitlab)** — 3 MRs: new `gitlab_group_integration_harbor` &amp; `gitlab_group_integration_mattermost` resources, plus a group-SAML-identity attribute.
- **[GitLab monorepo](https://gitlab.com/gitlab-org/gitlab)** — 2 code-quality fixes (`Gitlab::Json.safe_parse` hardening; Vue `require-name-property` compliance).

### <img src="https://img.shields.io/badge/LLVM%20%2F%20Clang-262D3A?logo=llvm&logoColor=white" height="20"/> &nbsp;compiler codegen &amp; tooling

| PR | Area | Contribution |
| :-- | :-- | :-- |
| [#169980](https://github.com/llvm/llvm-project/pull/169980) | X86 / Clang | constexpr evaluation of `cvtpd2ps` intrinsics |
| [#178885](https://github.com/llvm/llvm-project/pull/178885) | AArch64 | Convert CLS intrinsics to the generic `ISD::CTLS` node |
| [#178430](https://github.com/llvm/llvm-project/pull/178430) | ARM | Replace manual CLS expansion with `ISD::CTLS` |
| [#173473](https://github.com/llvm/llvm-project/pull/173473) | LLDB | SWIG Python-extension tests for `SBTarget` |

### <img src="https://img.shields.io/badge/Apple%20Swift%20NIO-F05138?logo=swift&logoColor=white" height="20"/>

[`#3410`](https://github.com/apple/swift-nio/pull/3410) — idempotent directory creation in `NIOFileSystem`.

<details>
<summary><b>All 11 GitLab merge requests →</b></summary>

<br>

**`gitlab-org/api/client-go` · Go SDK**

| MR | Contribution |
| :-- | :-- |
| [!2692](https://gitlab.com/gitlab-org/api/client-go/-/merge_requests/2692) | Slack integration — structs + `GetGroupSlackSettings` / `SetGroupSlackSettings` / `DisableGroupSlack` |
| [!2691](https://gitlab.com/gitlab-org/api/client-go/-/merge_requests/2691) | Discord / Telegram / Mattermost / Matrix / Google Chat structs + read-only `GetGroup*Settings` methods |
| [!2679](https://gitlab.com/gitlab-org/api/client-go/-/merge_requests/2679) | Microsoft Teams integration structs + typed return; fixed the `microsoft-teams` endpoint path |
| [!2677](https://gitlab.com/gitlab-org/api/client-go/-/merge_requests/2677) | Jira integration structs + typed `GetGroupJiraSettings` return |
| [!2675](https://gitlab.com/gitlab-org/api/client-go/-/merge_requests/2675) | Group Mattermost notifications + slash-commands — structs and `Get`/`Set`/`Delete` methods |
| [!2670](https://gitlab.com/gitlab-org/api/client-go/-/merge_requests/2670) | Harbor integration structs + typed `GetGroupHarborSettings` return |

**`gitlab-org/terraform-provider-gitlab` · IaC**

| MR | Contribution |
| :-- | :-- |
| [!2909](https://gitlab.com/gitlab-org/terraform-provider-gitlab/-/merge_requests/2909) | New `gitlab_group_integration_mattermost` resource (Plugin-Framework CRUD + acceptance test) |
| [!2881](https://gitlab.com/gitlab-org/terraform-provider-gitlab/-/merge_requests/2881) | New `gitlab_group_integration_harbor` resource (CRUD + import + acceptance test) |
| [!2852](https://gitlab.com/gitlab-org/terraform-provider-gitlab/-/merge_requests/2852) | Group SAML identity attribute on the `gitlab_group_membership` data source |

**`gitlab-org/gitlab` · monorepo**

| MR | Contribution |
| :-- | :-- |
| [!221163](https://gitlab.com/gitlab-org/gitlab/-/merge_requests/221163) | Ruby — `Gitlab::Json.parse` → `safe_parse` in the discussions-diff highlight cache |
| [!221158](https://gitlab.com/gitlab-org/gitlab/-/merge_requests/221158) | Vue — `require-name-property` compliance across deployment UI components |

</details>

---

## 🏆 Competitive programming

- **2× ACPC Finalist** (Arab Collegiate Programming Contest)
- **Problem setter &amp; tester** for **ECPC** and **ACPC**
- Codeforces — **[Hmzaawy](https://codeforces.com/profile/Hmzaawy)**

---

## 🧰 Tech

- **Cloud &amp; DevOps** — AWS (Solutions Architect – Associate), Docker, Nginx, Redis, Terraform, GitHub Actions, CI/CD
- **Backend &amp; full-stack** — TypeScript, Node.js, Express, MongoDB, PostgreSQL, React, WebSockets / CRDTs
- **Systems &amp; languages** — C++ (17/23), Rust, Go, LLVM/Clang, CMake, Linux internals *(where I go for depth)*

---

## ✍️ Writing

I write about systems programming — currently working through *What Every Programmer Should Know
About Memory* — on **[Dev.to](https://dev.to/hamzahassanain0)**.

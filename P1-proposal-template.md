# P1 Proposal Deck — Research Hub
**CSE 3412 SAD Lab · Section B · Fall 2026 · Presentation: 8 minutes**

> Replace all bracketed team and evidence fields with real project details before presenting.

| # | Slide | What to show | Rubric |
|---:|---|---|---|
| 1 | **Research Hub — Publish, Discover, Collaborate, and Review** | **Team:** Banka<br>**Members:** Farajana Atker Limu, Zabir Zakwan, Tabassum Sultana, Anik Chakraborty<br>**Supervisor:** Rajwan Ahmed<br>**One-line problem:** University researchers and students need one secure web platform for papers, projects, feedback, and review. | – |
| 2 | **The problem is fragmented research activity** | **Who suffers:** Researchers, students, supervisors, reviewers, and administrators.<br>**Current problem:** Publications, project discussions, document versions, and review decisions are scattered across email, shared drives, and messaging applications.<br>**Cost:** Slow feedback, difficult discovery, repeated communication, unclear review status, and potential unauthorized access to private work.<br>**Scope:** The SRS defines a web application for one university. | 1 |
| 3 | **Evidence: interviews** | **Interviewees:** [Add 3+ real interviewees by role, not name].<br>**Example participant roles:** undergraduate student, postgraduate researcher, supervisor/faculty member, administrator.<br>**Top pain points:** finding relevant papers, locating the latest version, tracking review decisions, and sharing project-only documents safely.<br>**Illustrative quote:** “I need to search email and shared folders just to find feedback and the latest document.” | 1 |
| 4 | **Evidence: survey** | **Survey goal:** [Add sample size, participant roles, and response count].<br>**Chart 1:** Most frequently used tools for sharing research work.<br>**Chart 2:** Time usually required to receive feedback or locate a paper.<br>**Chart 3:** Highest-priority needs: upload, discovery, project collaboration, or review workflow.<br>**Surprising finding:** [Add the single result that differs from the team's expectation]. | 1 |
| 5 | **Users and stakeholders** | **Guest:** browses public publications.<br>**Researcher/Student:** uploads publications, searches, collaborates, submits for review.<br>**Supervisor/Faculty:** manages projects and review activity.<br>**Reviewer:** evaluates submissions and records decisions.<br>**Administrator:** manages users, roles, categories, moderation, and reports.<br>**Stakeholder position:** supervisors and administrators have high control and high interest; researchers/reviewers have high interest and operational influence. | 2 |
| 6 | **The current process is disconnected** | **Current flow:** Search shared folders or external sources → email or message the author/supervisor → exchange files manually → review and approve in email → update status informally → retain decisions across separate records.<br>**Where it breaks:** no controlled publication visibility, no complete version history, weak search, no central review queue, and no auditable activity history.<br>**Research Hub replaces this chain with one authorized workspace.** | 1 |
| 7 | **Benchmark: alternatives cover only individual activities** | | 3 |

### Weighted benchmark matrix

| Alternative | Publication discovery (25%) | Project collaboration (20%) | Review workflow (20%) | Document version control (15%) | Role/privacy control (20%) | **Weighted total** |
|---|---:|---:|---:|---:|---:|---:|
| Email and shared folders | 1 | 2 | 2 | 2 | 1 | **40%** |
| Messaging applications | 1 | 4 | 1 | 1 | 1 | **37%** |
| Learning management system | 2 | 3 | 3 | 2 | 4 | **54%** |
| Research repositories | 5 | 1 | 2 | 4 | 3 | **66%** |
| **Research Hub** | **5** | **5** | **5** | **5** | **5** | **100%** |

*Illustrative scores: 1 = weak and 5 = excellent. Replace with evidence and verified comparison findings.*

| # | Slide | What to show | Rubric |
|---:|---|---|---|
| 8 | **Gaps and our edge** | **Competitors miss:** repositories focus on discovery, LMS platforms lack publication-oriented review, and files/email lack access control and traceability.<br>**Our edge:** Research Hub combines PDF publication management, authorized search, project workspaces, comments, a complete review workflow, notifications, and administration in one web platform.<br>**Unique value:** Students and researchers keep work visible to the right people while supervisors and reviewers receive structured feedback and status history. | 3 |
| 9 | **Proposed system: upload to approved publication** | **1. Register/login:** guest creates an account and requests a role; an administrator approves it.<br>**2. Upload:** researcher adds PDF metadata and visibility.<br>**3. Discover:** authorized users search, filter, view, and download.<br>**4. Collaborate:** project members share publications and comment.<br>**5. Submit:** author starts the review.<br>**6. Review:** reviewer submits comments, rating, and Approve/Revise/Reject.<br>**7. Notify:** system sends in-app and key email events.<br>**Supporting administration:** role approval, moderation, audit log, and reports. | 4 |
| 10 | **MoSCoW: protect the core and defer extras** | **Must:** account login/logout/password reset; role-based access; PDF upload and metadata; 25 MB and PDF validation; edit/delete/view; authorized search and pagination; administrator account/role/content control.<br>**Should:** email verification; profiles; visibility; tags; version history; filters/sorting; project groups/comments; review workflow; in-app notifications; audit log/categories.<br>**Could:** public profiles; bookmarks; citations; related publications; project tasks; public approval; email alerts/reminders; dashboard and CSV report.<br>**Won't:** native mobile app, plagiarism detection, real-time chat/video, external research database integration, payments, and multi-language interface. | 4 |
| 11 | **Feasibility and next steps** | **Technical:** responsive HTTPS web application, relational database, PDF/file storage, and SMTP email service.<br>**Operational:** pilot five roles: guest, researcher, supervisor, reviewer, and administrator; confirm role approval and moderation procedures.<br>**Economic:** use open-source frameworks and free-tier or low-cost hosting within semester constraints.<br>**Schedule:** requirements confirmed → wireframes/data model → prototype → unit/integration testing → five-role pilot → evaluation.<br>**Top risks:** semester scope, PDF security/privacy, and hosting limits; mitigate with fixed Must-have scope, 25 MB validation, RBAC, and tested backups. | – |
| 12 | **Q&A** | **Major prototype demo:** register/request a role → upload a PDF → search and open it → invite project members → submit for review → approve/revise/reject → verify notification and audit history. | 5 |

## Presenter notes

- Replace interview and survey statements with collected evidence before presenting.
- Explain the benchmark weights and cite each alternative.
- Keep the demo focused on the major workflow: upload, search, project collaboration, and review.
- Treat the PDF limit, 25 MB maximum, HTTPS, 30-minute session inactivity, and RBAC as key SRS constraints.
\# App-web-pro — Antigravity Workflow Skill



\## Overview

App-web-pro là một \*\*Workflow Skill (WFL)\*\* dành cho Antigravity AI nhằm chuẩn hóa toàn bộ vòng đời xây dựng \*\*Web Application\*\*:

từ \*\*ý tưởng ban đầu → MVP chạy thật → vận hành, bảo trì, mở rộng lâu dài\*\*.



Skill này được thiết kế để:

\- AI có thể \*\*tạo code, API, database, config\*\* một cách nhất quán

\- Team có thể \*\*onboard người mới nhanh\*\*

\- Việc \*\*fix bug / update / refactor\*\* luôn có điểm tựa rõ ràng, không phá hệ thống



---



\## Design Principles

1\. \*\*Workflow-driven\*\*: mọi thứ đi theo từng bước (step), không nhảy cóc.

2\. \*\*Deliverable-based\*\*: mỗi bước phải sinh ra tài liệu đầu ra rõ ràng.

3\. \*\*Traceability-first\*\*: mọi thứ đều truy ngược được (Use case → Story → Code → Release).

4\. \*\*AI + Human Friendly\*\*: vừa cho AI sinh code, vừa cho con người đọc hiểu.

5\. \*\*Maintenance-oriented\*\*: ưu tiên bảo trì hơn “viết cho nhanh”.



---



\## Required Inputs (Minimum)

Khi dùng skill này, người dùng cần cung cấp tối thiểu:

\- App name

\- Domain / industry

\- Primary user roles

\- Business goal / KPI

\- Team roles (PM, FE, BE, QA, DevOps – có thể gộp)



Nếu thiếu, AI được phép \*\*giả định hợp lý và ghi rõ “Assumption”\*\*.



---



\## Workflow Structure (WFL)



\### Step 00 — Project Map

\*\*Mục tiêu:\*\* tạo bản đồ dự án 1 trang để ai vào cũng hiểu.

\*\*Output:\*\* Project Map (links, modules, issue rules, release rules).



\### Step 01 — Define Problem \& Goal

\*\*Mục tiêu:\*\* chốt bài toán, user, KPI, phạm vi MVP.

\*\*Output:\*\* Product Brief 1 trang.



\### Step 02 — Research \& Benchmark

\*\*Mục tiêu:\*\* tránh làm mù, học từ thị trường.

\*\*Output:\*\* Benchmark table + Insights + MVP implications.



\### Step 03 — MVP Scope \& Roadmap

\*\*Mục tiêu:\*\* khóa phạm vi, chống scope creep.

\*\*Output:\*\* Must/Should/Nice + roadmap theo sprint.



---



\### Step 04 — Use Case \& User Flow

\*\*Mục tiêu:\*\* xương sống logic cho toàn bộ app.

\*\*Output:\*\* 

\- Use case inventory

\- MVP use cases

\- Flow chi tiết (main/alt/error)

\- Flow Coverage Map



---



\### Step 05 — User Stories \& Acceptance Criteria

\*\*Mục tiêu:\*\* biến use case thành backlog dev-ready.

\*\*Output:\*\* 

\- Epics

\- User stories (G/W/T)

\- Definition of Ready

\- Backlog summary



---



\### Step 06 — IA, Screen List \& Wireframe Spec

\*\*Mục tiêu:\*\* UI/FE/BE/QA cùng hiểu từng màn hình.

\*\*Output:\*\* 

\- Sitemap

\- Screen list

\- Screen specs (data, actions, states)



---



\### Step 07 — Data Model \& ERD

\*\*Mục tiêu:\*\* thiết kế dữ liệu chuẩn để AI sinh DB/ORM.

\*\*Output:\*\* 

\- Entity inventory

\- ERD

\- Data dictionary

\- Migration notes



---



\### Step 08 — API Contract

\*\*Mục tiêu:\*\* FE/BE/QA dùng chung 1 sự thật.

\*\*Output:\*\* 

\- API spec theo module

\- Request/Response schema

\- Error codes

\- Security notes



---



\### Step 09 — System Design \& DevOps

\*\*Mục tiêu:\*\* deploy được, debug được, scale được.

\*\*Output:\*\* 

\- Architecture

\- Environments

\- CI/CD

\- Logging \& monitoring



---



\### Step 10 — Dev Workflow \& Sprint Rules

\*\*Mục tiêu:\*\* code không loạn, AI không phá chuẩn.

\*\*Output:\*\* 

\- Branching

\- Commit rules

\- Code structure

\- Definition of Done



---



\### Step 11 — QA, UAT \& Release

\*\*Mục tiêu:\*\* test không mù, release không nổ.

\*\*Output:\*\* 

\- Test strategy

\- Test cases

\- UAT checklist

\- Severity rules



---



\### Step 12 — Runbook \& Maintenance (AI Mode)

\*\*Mục tiêu:\*\* fix bug có quy trình, AI sửa không phá.

\*\*Output:\*\* 

\- Runbook

\- Changelog rules

\- Incident flow

\- AI Maintenance Mode rules



---



\## How Antigravity Should Use This Skill

\- Mỗi lần chạy \*\*chỉ chạy 1 step\*\*

\- Không được chạy step tiếp theo nếu \*\*EXIT CRITERIA\*\* của step trước chưa đạt

\- Mọi output phải ghi rõ:

&nbsp; - Owner

&nbsp; - Version

&nbsp; - Last updated

\- Khi fix bug hoặc update:

&nbsp; - Bắt buộc dùng Step 12 (Maintenance Mode)



---



\## When This Skill Is Ideal

\- Xây app web mới từ đầu

\- Refactor app cũ đang loạn

\- Dự án cần giao cho team khác

\- Dùng AI để code nhưng vẫn muốn kiểm soát chất lượng



---



\## Explicit Non-Goals

\- Không dùng cho app mobile native

\- Không dùng cho landing page đơn giản

\- Không dùng cho script ngắn, tool 1 file



---



\## License / Usage

Skill này được thiết kế để:

\- Dùng nội bộ

\- Dùng cho team

\- Dùng để build SaaS / product thực tế



Không khuyến khích cắt xén workflow nếu muốn bảo trì dài hạn.




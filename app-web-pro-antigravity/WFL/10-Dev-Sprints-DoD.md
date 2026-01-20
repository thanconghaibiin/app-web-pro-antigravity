Bạn là Engineering Manager + Tech Lead.



Nhiệm vụ:



Chuẩn hoá cách code – review – merge – release



Định nghĩa rõ khi nào 1 ticket được coi là DONE



Thiết kế workflow để:



Dev mới vào làm được ngay



AI sinh code không phá chuẩn



Refactor không gây side effect



QUY TRÌNH BẮT BUỘC



Chuẩn hoá branching strategy



Chuẩn hoá code structure (FE + BE)



Chuẩn hoá naming conventions



Chuẩn hoá Definition of Done (DoD)



Chuẩn hoá Sprint workflow



Gắn traceability: Story → Commit → Release



OUTPUT FORMAT (AI CODE-READY)

\# Dev Workflow \& Sprint Rules — <App Name> (v0.1)

Owner:

Last updated:



\## 1) Branching Strategy

\- main: production

\- develop: staging

\- feature/<story-id>-short-desc

\- hotfix/<issue-id>



\## 2) Commit Message Convention

Format:

<type>(<module>): <short description>



Types:

\- feat

\- fix

\- refactor

\- chore

\- test

\- docs



Example:

feat(auth): add JWT refresh token



\## 3) Code Structure



\### Backend

/src

&nbsp; /modules

&nbsp;   /auth

&nbsp;     controller.ts

&nbsp;     service.ts

&nbsp;     dto.ts

&nbsp;     entity.ts

&nbsp;   /<module>

&nbsp; /shared

&nbsp; /config

&nbsp; /migrations



\### Frontend

/src

&nbsp; /pages

&nbsp; /modules

&nbsp; /components

&nbsp; /hooks

&nbsp; /services (API calls)

&nbsp; /types



\## 4) Naming Conventions

\- Entity: snake\_case

\- API path: kebab-case

\- Variables: camelCase

\- Constants: UPPER\_SNAKE\_CASE



\## 5) Definition of Done (DoD)

Một ticket chỉ được DONE khi:

\- \[ ] Code pass lint

\- \[ ] Unit test (nếu có logic)

\- \[ ] API contract không bị phá

\- \[ ] Migration backward-safe

\- \[ ] Update changelog

\- \[ ] Link story ID trong commit



\## 6) Sprint Workflow

\- Sprint length: 1–2 tuần

\- Sprint planning:

&nbsp; - Pull từ backlog đã DoR

\- Daily:

&nbsp; - Blocker

\- Sprint review:

&nbsp; - Demo theo use case

\- Retro:

&nbsp; - 1 cải tiến cho sprint sau



\## 7) Traceability Rules

\- Story ID xuất hiện trong:

&nbsp; - Branch name

&nbsp; - Commit message

&nbsp; - Changelog

\- Release note link tới list story



\## EXIT CRITERIA

\- \[ ] Dev workflow rõ

\- \[ ] DoD thống nhất

\- \[ ] AI sinh code theo chuẩn này


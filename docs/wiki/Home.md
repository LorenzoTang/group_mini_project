<a id="top"></a>

# 校园社团活动发布与报名应用
# Campus Club Activity Release and Registration App

**[中文](#zh) | [English](#en)**

[项目仓库 / Repository](https://github.com/LorenzoTang/group_mini_project) · [README](https://github.com/LorenzoTang/group_mini_project/blob/main/README.md) · [Wiki 首页 / Wiki Home](https://github.com/LorenzoTang/group_mini_project/wiki)

---

<a id="zh"></a>

## 中文

欢迎来到项目 Wiki！这里用于记录西南交通大学利兹学院 Mini Project 的需求分析、系统设计、开发决策、测试记录和团队协作过程。

首次了解项目，建议先阅读 [README 中文版](https://github.com/LorenzoTang/group_mini_project/blob/main/README.md#zh)。README 提供项目概览；Wiki 用于解释需求、设计依据以及实现与验证过程。

**本页导航：** [项目目标](#zh-goals) · [角色与流程](#zh-workflow) · [技术与约束](#zh-technical) · [文档规划](#zh-docs) · [协作与维护](#zh-collaboration)

[Switch to English](#en)

<a id="zh-goals"></a>

### 项目目标

为校园社团、学生和社团管理教师提供统一的活动发布、审核与报名平台，帮助学生发现校园活动，并让组织者管理活动与报名信息。

计划覆盖以下功能：

- **活动管理：** 创建、编辑和取消活动，设置地点、参与要求、报名截止时间与人数上限。
- **活动宣传：** 发布社团新闻和公告，生成活动报名二维码。
- **活动报名：** 浏览与搜索活动、扫码报名、查看已报名活动并设置提醒。
- **活动审核：** 由学校指定的社团管理教师审核，批准后才能公开发布。
- **身份认证：** 参照学校统一身份认证流程，采用适合课程项目的简化方案。

以上内容描述项目目标，不代表功能已完成；只有经过实现和测试的功能才应标记为已交付。

<a id="zh-workflow"></a>

### 角色与流程

| 角色 | 主要职责 |
|---|---|
| 学生 | 发现活动、报名、查看报名记录、设置提醒。 |
| 社团组织者 | 发布公告、创建和维护活动、查看报名情况。 |
| 社团管理教师 | 审核活动并决定是否批准发布。 |

核心流程：**社团创建活动 → 教师审核 → 批准后发布 → 学生浏览或扫码报名 → 查看报名信息与活动提醒。**

报名截止时间与人数上限应在报名时生效。活动编辑、取消以及审核未通过时的具体处理规则，需要在需求分析与设计文档中明确。

<a id="zh-technical"></a>

### 技术与约束

| 项目 | 当前规划 |
|---|---|
| 编程语言 | Kotlin |
| 后端框架 | Ktor |
| 数据存储 | 可使用本地 TXT / CSV 文件，具体方案随设计确定。 |
| 身份认证 | 无需完整接入学校统一身份认证基础设施。 |
| 图片与资源 | 下载并保存在本地。 |
| 版本管理 | Git 与 GitHub |
| 验证要求 | 已交付功能应经过测试，并能在学期末展示中演示。 |

具体依赖版本、构建命令和运行步骤将在项目配置确定后补充至 [README 的快速开始章节](https://github.com/LorenzoTang/group_mini_project/blob/main/README.md#zh-start)。

<a id="zh-docs"></a>

### 文档规划

会议记录：[第一次小组会议：初步任务分工](https://github.com/LorenzoTang/group_mini_project/wiki/Meeting-01)。

以下是建议逐步建立的文档内容，目前不代表已有对应独立 Wiki 页面。页面创建后，可在此表中补充链接。

| 文档主题 | 应记录的内容 |
|---|---|
| 需求分析 | 用户故事、功能需求、约束、验收标准和需求变更。 |
| 系统设计 | 模块职责、架构、界面流程和关键设计决策。 |
| 数据设计 | 活动、用户与报名记录的数据结构，以及存储与校验规则。 |
| 迭代计划 | 每次迭代的目标、任务分工、进度和交付结果。 |
| 测试记录 | 测试环境、测试步骤、预期结果、实际结果与缺陷修复情况。 |
| 会议纪要 | 会议日期、参与人员、讨论内容、决策和后续行动。 |
| 演示与回顾 | 已完成功能、演示步骤、已知限制和改进方向。 |

<a id="zh-collaboration"></a>

### 协作与维护

- 需求或设计发生变化时，同步更新相关文档，并记录变更原因。
- 测试记录应关联对应功能和代码版本，区分计划、实现与验证结果。
- 会议纪要应明确行动项、负责人和目标完成时间。
- 新增 Wiki 页面后更新首页导航，保持中英文内容一致。
- 团队成员与分工确定后，补充到项目文档；当前成员名单仍待确认。

可通过 [提交历史](https://github.com/LorenzoTang/group_mini_project/commits/main) 查看代码与仓库文档变更，通过 [Pull Requests](https://github.com/LorenzoTang/group_mini_project/pulls) 查看合并请求与评审。

[返回顶部](#top) · [Switch to English](#en)

---

<a id="en"></a>

## English

Welcome to the project Wiki! This space documents requirements analysis, system design, development decisions, testing records, and team collaboration for the SWJTU–Leeds Joint School Mini Project.

New to the project? Start with the [English README](https://github.com/LorenzoTang/group_mini_project/blob/main/README.md#en). The README provides an overview; the Wiki explains requirements, design rationale, implementation, and verification.

**On this page:** [Project Goals](#en-goals) · [Roles and Workflow](#en-workflow) · [Technology and Constraints](#en-technical) · [Documentation Plan](#en-docs) · [Collaboration and Maintenance](#en-collaboration)

[切换到中文](#zh)

<a id="en-goals"></a>

### Project Goals

Provide a shared platform for student clubs, students, and club management teachers to publish, review, and register for campus activities. Help students discover events and organisers manage activities and registration information.

Planned capabilities include:

- **Activity management:** Create, edit, and cancel activities; set locations, participant requirements, registration deadlines, and capacity limits.
- **Activity promotion:** Publish club news and announcements, and generate registration QR codes.
- **Activity registration:** Browse and search activities, register by scanning QR codes, view registered activities, and set reminders.
- **Activity review:** Require approval from a university-assigned club management teacher before publication.
- **Authentication:** Follow the university's unified authentication workflow using a simplified approach appropriate for the coursework.

These are project goals, not claims of completed functionality. Only implemented and tested features should be marked as delivered.

<a id="en-workflow"></a>

### Roles and Workflow

| Role | Main Responsibilities |
|---|---|
| Students | Discover activities, register, view registration records, and set reminders. |
| Club Organisers | Publish announcements, create and maintain activities, and monitor registrations. |
| Club Management Teachers | Review activities and decide whether to approve publication. |

Core workflow: **Club creates an activity → Teacher reviews it → Approved activity is published → Students browse or scan to register → Students view registration information and activity reminders.**

Registration deadlines and capacity limits should be enforced during registration. Detailed rules for activity edits, cancellations, and rejected submissions need to be defined in the requirements and design documentation.

<a id="en-technical"></a>

### Technology and Constraints

| Area | Current Plan |
|---|---|
| Language | Kotlin |
| Backend framework | Ktor |
| Data storage | Local TXT / CSV files may be used; details will be decided during design. |
| Authentication | Full integration with the university's authentication infrastructure is not required. |
| Images and assets | Download and store locally. |
| Version control | Git and GitHub |
| Verification | Delivered features should be tested and demonstrable at the end of the semester. |

Dependency versions, build commands, and execution steps will be added to the [Getting Started section of the README](https://github.com/LorenzoTang/group_mini_project/blob/main/README.md#en-start) once the project configuration is established.

<a id="en-docs"></a>

### Documentation Plan

Meeting notes: [Meeting 01: Initial Task Allocation](https://github.com/LorenzoTang/group_mini_project/wiki/Meeting-01).

The following topics are proposed for incremental documentation. They do not imply that separate Wiki pages already exist. Add links to this table as pages are created.

| Topic | Information to Record |
|---|---|
| Requirements Analysis | User stories, functional requirements, constraints, acceptance criteria, and requirement changes. |
| System Design | Module responsibilities, architecture, interface flows, and key design decisions. |
| Data Design | Structures for activities, users, and registrations, plus storage and validation rules. |
| Iteration Planning | Iteration goals, task ownership, progress, and delivered outcomes. |
| Testing Records | Test environment, steps, expected and actual results, and defect resolution. |
| Meeting Notes | Dates, attendees, discussions, decisions, and follow-up actions. |
| Demonstration and Retrospective | Completed features, demonstration steps, known limitations, and improvements. |

<a id="en-collaboration"></a>

### Collaboration and Maintenance

- Update relevant documentation when requirements or designs change, and record the reasons.
- Link test records to the relevant feature and code version, distinguishing plans, implementation, and verification results.
- Record action items, owners, and target completion dates in meeting notes.
- Update homepage navigation when adding Wiki pages, and keep both language versions aligned.
- Add team members and responsibilities to the documentation once agreed; the member list remains to be confirmed.

Use the [commit history](https://github.com/LorenzoTang/group_mini_project/commits/main) to review code and repository documentation changes, and [Pull Requests](https://github.com/LorenzoTang/group_mini_project/pulls) to view proposed merges and reviews.

[Back to top](#top) · [切换到中文](#zh)
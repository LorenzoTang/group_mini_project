<a id="top"></a>

# 校园社团活动发布与报名应用 / Campus Club Activity Release and Registration App

**语言 / Language： [中文](#zh) | [English](#en)**

<a id="zh"></a>

## 中文

[Switch to English](#en)

本应用面向西南交通大学校园活动管理，旨在帮助学生社团发布活动、管理报名，并加强与同学之间的互动。

**目录：** [项目概述](#zh-overview) · [功能介绍](#zh-features) · [用户角色](#zh-roles) · [项目范围与约束](#zh-scope) · [技术栈](#zh-stack) · [项目结构](#zh-structure) · [快速开始](#zh-start) · [测试](#zh-testing) · [项目文档](#zh-docs) · [开发方式](#zh-development) · [团队](#zh-team) · [许可证](#zh-license)

<a id="zh-overview"></a>

### 项目概述

西南交通大学拥有超过 100 个学生社团，涵盖文学、音乐、体育、程序设计竞赛等多种兴趣领域。高效管理社团活动和学生报名，对促进校园活动参与至关重要。

**校园社团活动发布与报名应用**旨在提供一个便捷的平台，让社团发布活动与公告、学生发现并报名参加活动，同时让校方工作人员在活动发布前进行审核。

本项目是西南交通大学利兹学院软件工程课程的小组项目。

<a id="zh-features"></a>

### 功能介绍

#### 1. 活动发布与管理

- 创建活动，填写活动描述、地点、参与要求、报名截止时间和人数上限。
- 为每项活动生成报名二维码。
- 编辑活动信息，包括地点、报名截止时间和人数上限。
- 在必要时取消活动。
- 发布社团新闻与公告，用于活动宣传和招募新成员。

#### 2. 活动发现与报名

- 浏览和搜索可参加的校园活动。
- 扫描活动二维码进行报名。
- 在**已报名活动**中查看报名信息。
- 为已报名的活动设置提醒。

#### 3. 活动审核与批准

- 活动发布前须获得学校指定的社团管理教师批准。
- 提供审核流程，确保活动在公开发布前经过检查。

#### 4. 用户身份认证

- 参照学校统一身份认证系统设计登录流程。
- 采用适合本课程项目范围的简化认证方式，无需完整接入学校的身份认证基础设施。

<a id="zh-roles"></a>

### 用户角色

| 角色 | 职责 |
|---|---|
| 学生 | 浏览活动、报名参加活动、查看已报名活动并设置提醒。 |
| 社团组织者 | 发布社团公告、创建和管理活动，并查看报名情况。 |
| 社团管理教师 | 审核活动，并在发布前批准活动。 |

<a id="zh-scope"></a>

### 项目范围与约束

项目实现以课程项目要求为依据。

- **数据存储：** 可以使用本地文本文件或 CSV 文件，无需完整集成数据库。
- **身份认证：** 无需完整接入学校统一身份认证系统。
- **活动审批：** 活动必须经过审核才能发布。
- **本地资源：** 应用中使用的图片应下载并保存在本地，避免直接引用远程图片。
- **测试：** 每项已开发功能都应经过测试，并能够在学期末展示中正常演示。

<a id="zh-stack"></a>

### 技术栈

技术栈将随项目开发进展更新。

- **编程语言：** Kotlin
- **后端 / 框架：** Ktor
- **数据存储：** 本地 TXT / CSV 文件（如适用）
- **测试：** 根据实际实现的功能确定
- **版本控制：** Git 和 GitHub

<a id="zh-structure"></a>

### 项目结构

以下目录结构仅作为建议的起点，应根据仓库实际情况调整。

```text
.
├── src/                    # 应用源代码
├── tests/                  # 自动化测试或功能测试
├── data/                   # 本地数据文件（如适用）
├── assets/                 # 本地图片及资源
├── docs/                   # 项目文档
├── README.md               # 项目概述与说明
└── .gitignore              # 版本控制忽略规则
```

<a id="zh-start"></a>

### 快速开始

应用结构与运行流程确定后，将补充具体的配置说明。

#### 环境要求

- 项目要求版本的 JDK
- Kotlin 和 Gradle 构建环境
- 项目配置中指定的其他依赖

#### 安装与运行

1. 克隆仓库。

   ```bash
   git clone <repository-url>
   cd <repository-directory>
   ```

2. 使用熟悉的 IDE 打开项目，例如 IntelliJ IDEA，或已配置 Kotlin 工具的 Visual Studio Code。
3. 安装或解析项目依赖。
4. 按照项目配置提供的构建与运行说明启动应用。

> 注意：应用具备运行条件后，应将这些初步说明替换为经过验证的命令。

<a id="zh-testing"></a>

### 测试

测试将重点验证已实现功能的行为是否符合预期。

可能的测试范围包括：

- 创建和编辑活动。
- 执行报名截止时间与人数上限限制。
- 报名参加活动并查看报名记录。
- 生成和处理活动二维码。
- 在活动发布前进行审核与批准。
- 取消活动并更新其状态。
- 保存和读取本地存储中的数据。

只有已完成且经过测试的功能，才能标记为已实现。

<a id="zh-docs"></a>

### 项目文档

GitHub 仓库用于存放应用源代码与项目资源。

配套的 **GitHub Wiki** 用于记录团队的设计工作、需求分析、会议纪要及其他项目决策。

<a id="zh-development"></a>

### 开发方式

项目将在整个学期内采用增量开发方式推进。每次迭代的目标是交付一项与已确定需求相关且经过测试的功能，逐步构建可在学期末演示的完整应用。

<a id="zh-team"></a>

### 团队

**课程：** 西南交通大学利兹学院 Mini Project

**项目：** 校园社团活动发布与报名应用

**团队成员：** 待补充

<a id="zh-license"></a>

### 许可证

待确定。

[返回顶部](#top) · [Switch to English](#en)

---

<a id="en"></a>

## English

[切换到中文](#zh)

### Campus Club Activity Release and Registration App

A campus activity management application designed to help student clubs at Southwest Jiaotong University publish events, manage registrations, and engage with students.

**Contents:** [Overview](#en-overview) · [Features](#en-features) · [User Roles](#en-roles) · [Project Scope and Constraints](#en-scope) · [Technology Stack](#en-stack) · [Project Structure](#en-structure) · [Getting Started](#en-start) · [Testing](#en-testing) · [Project Documentation](#en-docs) · [Development Approach](#en-development) · [Team](#en-team) · [License](#en-license)

<a id="en-overview"></a>

### Overview

Southwest Jiaotong University has more than 100 student clubs covering a wide range of interests, including literature, music, sports, and programming competitions. Managing club activities and student registrations efficiently is essential to encouraging campus participation.

The **Campus Club Activity Release and Registration App** aims to provide a convenient platform for clubs to publish activities and announcements, for students to discover and register for events, and for university staff to review activities before publication.

This project is developed as a mini-project for the SWJTU–Leeds Joint School software engineering coursework.

<a id="en-features"></a>

### Features

#### 1. Activity Publication and Management

- Create activities with descriptions, locations, participant requirements, registration deadlines, and capacity limits.
- Generate a registration QR code for each activity.
- Edit activity details, including the location, registration deadline, and participant capacity.
- Cancel activities when necessary.
- Publish club news and announcements to promote events and recruit new members.

#### 2. Activity Discovery and Registration

- Browse and search available campus activities.
- Scan an activity's QR code to register.
- View registration information in the **Registered Activities** section.
- Set reminders for registered activities.

#### 3. Activity Review and Approval

- Require approval from a university-assigned club management teacher before an activity is published.
- Support a review process to help ensure that activities are checked before becoming publicly available.

#### 4. User Authentication

- Design the login workflow around the university's unified identity authentication system.
- Use a simplified authentication approach suitable for the scope of the mini-project, without requiring full integration with the university's authentication infrastructure.

<a id="en-roles"></a>

### User Roles

| Role | Responsibilities |
|---|---|
| Students | Browse activities, register for events, view registered activities, and set reminders. |
| Club Organisers | Publish club announcements, create and manage activities, and monitor registration status. |
| Club Management Teachers | Review activities and approve them before publication. |

<a id="en-scope"></a>

### Project Scope and Constraints

The implementation is designed around the requirements of the mini-project specification.

- **Data storage:** Local text or CSV files may be used instead of a fully integrated database.
- **Authentication:** Full integration with the university's unified identity authentication system is not required.
- **Activity approval:** Activities must be reviewed before publication.
- **Local assets:** Images used in the application should be downloaded and stored locally rather than hotlinked.
- **Testing:** Each developed feature should be tested and functional enough to demonstrate during the end-of-semester presentation.

<a id="en-stack"></a>

### Technology Stack

The technology stack will be updated as the project develops.

- **Language:** Kotlin
- **Backend / Framework:** Ktor
- **Data Storage:** Local TXT / CSV files, if applicable
- **Testing:** To be specified according to the implemented features
- **Version Control:** Git and GitHub

<a id="en-structure"></a>

### Project Structure

The directory structure below is a suggested starting point and should be adjusted to match the actual repository.

```text
.
├── src/                    # Application source code
├── tests/                  # Automated or feature tests
├── data/                   # Local data files, if applicable
├── assets/                 # Locally stored images and resources
├── docs/                   # Project documentation
├── README.md               # Project overview and instructions
└── .gitignore              # Files excluded from version control
```

<a id="en-start"></a>

### Getting Started

Setup instructions will be added once the application structure and execution workflow have been finalised.

#### Prerequisites

- JDK version required by the project
- Kotlin and Gradle build environment
- Any additional dependencies specified by the project configuration

#### Installation and Execution

1. Clone the repository.

   ```bash
   git clone <repository-url>
   cd <repository-directory>
   ```

2. Open the project in your preferred IDE, such as IntelliJ IDEA or Visual Studio Code with the appropriate Kotlin tooling.

3. Install or resolve the project dependencies.

4. Run the application using the build and execution instructions provided by the project configuration.

> Note: Replace these preliminary instructions with verified commands once the application is runnable.

<a id="en-testing"></a>

### Testing

Testing will focus on verifying that the implemented features behave as expected.

Potential test areas include:

- Creating and editing activities.
- Enforcing registration deadlines and participant capacity limits.
- Registering for activities and viewing registration records.
- Generating and processing activity QR codes.
- Reviewing and approving activities before publication.
- Cancelling activities and updating their status.
- Saving and retrieving data from local storage.

Only completed and tested features should be reported as implemented.

<a id="en-docs"></a>

### Project Documentation

The GitHub repository contains the application source code and project resources.

The accompanying **GitHub Wiki** is intended to document the team's design work, requirements analysis, meeting notes, and other project decisions.

<a id="en-development"></a>

### Development Approach

The project will be developed incrementally throughout the semester. Each iteration aims to deliver a tested feature related to the identified requirements, building towards a functional application that can be demonstrated at the end of the semester.

<a id="en-team"></a>

### Team

**Module:** SWJTU–Leeds Joint School Mini Project

**Project:** Campus Club Activity Release and Registration App

**Team Members:** To be added

<a id="en-license"></a>

### License

To be determined.

[Back to top](#top) · [切换到中文](#zh)

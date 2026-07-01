# Provenance Tool v0.3.1

> A local browser-based workspace for creating, verifying, and comparing portable provenance records for documents, source files, media, archives, and project folders.

<p align="left">
  <a href="https://xufentu.com/provenance-tool/">
    <img src="https://img.shields.io/badge/version-0.3.1-111111?style=flat-square" alt="Version 0.3.1">
  </a>
  <a href="https://xufentu.com/provenance-tool/">
    <img src="https://img.shields.io/badge/processing-local%20browser-f2f2f2?style=flat-square" alt="Local browser processing">
  </a>
  <a href="https://xufentu.com/provenance-tool/">
    <img src="https://img.shields.io/badge/integrity-SHA--256-f2f2f2?style=flat-square" alt="SHA-256 integrity">
  </a>
  <a href="https://xufentu.com/provenance-tool/">
    <img src="https://img.shields.io/badge/modes-create%20%7C%20verify%20%7C%20compare-f2f2f2?style=flat-square" alt="Create Verify Compare">
  </a>
</p>

## 🌐 Public Access

| Item | Link |
|---|---|
| Official website | [https://xufentu.com/provenance-tool/](https://xufentu.com/provenance-tool/) |

---

## ✦ Overview

Provenance Tool helps users create, preserve, verify, and compare portable file records before or after a work is released, delivered, archived, or cited.

Users can add documents, source files, images, audio, video, datasets, compressed archives, or project folders, enter essential record information, calculate SHA-256 locally, and save one portable provenance ZIP package.

> [!IMPORTANT]
> Selected files are processed locally inside the browser and are not automatically uploaded to the website server.

| Designed for | Use |
|---|---|
| Independent authors | Preserve publication and version records |
| Researchers | Keep file integrity and release information together |
| Creators | Create portable records for media and project files |
| Developers | Record source files, archives, and project folders |
| Organizations | Preserve project, delivery, and internal records |
| Project maintainers | Compare versions and verify saved records |

---

## ⚙️ Core Functions

| Mode | Purpose | Result |
|---|---|---|
| **Create Record** | Create a portable record for files or project folders | One provenance ZIP package |
| **Verify Record** | Check current files against a previously saved record | Matching or changed file status |
| **Compare Versions** | Compare a previous version with a current version | Unchanged, changed, added, and removed files |

---

## 📁 Create Record

| Step | Action |
|---|---|
| **01** | Add one file, multiple files, or a project folder |
| **02** | Enter essential record information |
| **03** | Calculate SHA-256 locally |
| **04** | Save one portable provenance ZIP package |

### Record Information

| Field | Description |
|---|---|
| **Title** | Name of the work or project |
| **Author or entity** | Author, organization, or responsible entity |
| **Version** | Current version |
| **Date** | Record or release date |
| **Type** | General content or project type |
| **Classification** | Public, Internal, Confidential, or Restricted |
| **Official link** | Optional public link |

### Record Classifications

| Classification | Intended Use |
|---|---|
| **Public** | Publicly released or publicly referenced work |
| **Internal** | Internal working files or project records |
| **Confidential** | Sensitive files intended for controlled access |
| **Restricted** | Files intended for limited authorized access |

### Generated Result

| Result | Description |
|---|---|
| File count | Number of selected files |
| Total size | Combined size of selected files |
| SHA-256 | File integrity values |
| Record status | Confirmation that the package is ready |
| Provenance package | One downloadable ZIP file |

---

## 📦 Generated Package

| File | Purpose |
|---|---|
| `metadata.json` | Basic information about the work and record |
| `provenance.json` | General provenance record |
| `file-integrity-records.json` | SHA-256 and file integrity information |
| `release-manifest.json` | Package content overview |
| `citation.txt` | Suggested citation for eligible public records |
| `README.md` | Human-readable package description |

### File Records

| Recorded Item | Description |
|---|---|
| Filename | Original file name |
| Relative path | File location inside the selected project |
| File type | Browser-recognized content type |
| File size | File size in bytes |
| Last modified | Local file modification time |
| SHA-256 | Reproducible file integrity value |

> [!NOTE]
> The structured records remain inside one portable ZIP package. Users do not need to download or organize separate JSON files individually.

---

## 🔐 Public and Non-Public Records

| Classification | Result Behavior |
|---|---|
| **Public** | May include a suggested citation and official public link |
| **Internal** | Uses concise record information |
| **Confidential** | Uses concise record information |
| **Restricted** | Uses concise record information |

### Example Record Information

| Example | Use |
|---|---|
| `Project Title · Version 1.0 · Confidential · 3 files · SHA-256` | Private project log, delivery record, archive note, or internal documentation |

The complete provenance ZIP package remains the primary record to preserve.

---

## ✅ Verify Record

| Required Item | Purpose |
|---|---|
| Current file or files | Files being checked now |
| Previously saved provenance ZIP or `file-integrity-records.json` | Earlier integrity reference |

### Verification Results

| Result | Meaning |
|---|---|
| **Unchanged** | The current file matches the saved SHA-256 record |
| **Changed** | The current file no longer matches the saved record |
| **Added** | A file exists in the current set but not in the saved record |
| **Removed** | A file existed in the saved record but is missing from the current set |

> Verification is performed locally inside the browser.

---

## ↔️ Compare Versions

| Version | Purpose |
|---|---|
| Previous version | Earlier files or project folder |
| Current version | Newer files or project folder |

### Comparison Results

| Result | Meaning |
|---|---|
| **Unchanged** | File content is identical |
| **Changed** | File content has changed |
| **Added** | File exists only in the current version |
| **Removed** | File existed only in the previous version |

### Common Use Cases

| Use Case | Example |
|---|---|
| Publications | Compare draft and release files |
| Repositories | Review project folder changes |
| Archives | Check preserved versions |
| Deliveries | Compare previous and current delivery packages |
| Internal systems | Review controlled file changes |

---

## #️⃣ SHA-256 Integrity

| SHA-256 Result | Meaning |
|---|---|
| Matching value | The compared file content is identical |
| Different value | The compared file content has changed |

### SHA-256 Does Not Independently Prove

| Boundary | Status |
|---|---|
| Authorship | Not proven |
| Legal ownership | Not proven |
| Originality | Not proven |
| First publication | Not proven |
| Original creation time | Not proven |

---

## 🛡️ Local Processing and Privacy

| Item | Status |
|---|---|
| File processing | Local browser |
| Automatic source-file upload | No |
| Integrity algorithm | SHA-256 |
| Package generation | Local browser |
| Package saving | User-controlled |
| Public publishing | User-controlled |

> [!CAUTION]
> Sensitive files and non-public provenance packages should not be uploaded to public repositories or public storage unless the user intentionally chooses to publish them.

---

## ⚖️ Tool Boundary

### Supported

| Supported Function | Status |
|---|---|
| Basic provenance documentation | Supported |
| Version continuity | Supported |
| File integrity records | Supported |
| Record verification | Supported |
| Version comparison | Supported |
| Portable project archiving | Supported |
| Citation continuity for public records | Supported |

### Not Provided

| Not Provided | Boundary |
|---|---|
| Proof of originality | Not provided |
| Legal ownership determination | Not provided |
| Truth verification | Not provided |
| Plagiarism detection | Not provided |
| AI-generation detection | Not provided |
| Authorship dispute resolution | Not provided |
| Copyright registration | Not provided |
| Independent trusted timestamp | Not provided |
| Replacement of human judgment | Not provided |

---

## 🧾 Project Information

| Item | Record |
|---|---|
| **Tool version** | `0.3.1` |
| **Status** | Public browser-based provenance workspace |
| **Working modes** | Create · Verify · Compare |
| **Processing** | Local browser processing |
| **Integrity algorithm** | `SHA-256` |
| **Result format** | One portable ZIP package |
| **Record classifications** | Public · Internal · Confidential · Restricted |
| **Concept and authorship** | Xufen Tu |
| **Public access** | [https://xufentu.com/provenance-tool/](https://xufentu.com/provenance-tool/) |

> **Automation can support structure, but responsibility remains visible.**

---

# 溯源工具 v0.3.1

> 一个面向文档、源代码、媒体文件、压缩文件和项目文件夹，用于创建、验证和前后比较可携带溯源记录的浏览器本地工作台。

<p align="left">
  <a href="https://xufentu.com/provenance-tool/">
    <img src="https://img.shields.io/badge/版本-0.3.1-111111?style=flat-square" alt="版本 0.3.1">
  </a>
  <a href="https://xufentu.com/provenance-tool/">
    <img src="https://img.shields.io/badge/处理方式-浏览器本地-f2f2f2?style=flat-square" alt="浏览器本地处理">
  </a>
  <a href="https://xufentu.com/provenance-tool/">
    <img src="https://img.shields.io/badge/完整性-SHA--256-f2f2f2?style=flat-square" alt="SHA-256 完整性">
  </a>
  <a href="https://xufentu.com/provenance-tool/">
    <img src="https://img.shields.io/badge/模式-创建%20%7C%20验证%20%7C%20对比-f2f2f2?style=flat-square" alt="创建 验证 对比">
  </a>
</p>

## 🌐 公开地址

| 项目 | 链接 |
|---|---|
| 官方工具地址 | [https://xufentu.com/provenance-tool/](https://xufentu.com/provenance-tool/) |

---

## ✦ 工具概述

Provenance Tool 用于在作品发布、项目交付、长期存档或对外引用之前及之后，创建、保存、验证和比较能够跟随文件长期保存的记录。

使用者可以添加文档、源代码、图片、音频、视频、数据集、压缩文件或项目文件夹，填写必要信息，在浏览器本地计算 SHA-256，并保存一个完整的溯源 ZIP 记录包。

> [!IMPORTANT]
> 所选择的原始文件在浏览器本地处理，不会自动上传到网站服务器。

| 适用对象 | 用途 |
|---|---|
| 独立作者 | 保存作品发布与版本记录 |
| 研究人员 | 统一保存文件完整性和发布信息 |
| 创作者 | 为媒体与项目文件建立可携带记录 |
| 开发者 | 记录源代码、压缩包和项目文件夹 |
| 机构 | 保存项目、交付和内部记录 |
| 项目维护者 | 核对已保存记录并比较版本变化 |

---

## ⚙️ 核心功能

| 模式 | 作用 | 结果 |
|---|---|---|
| **创建记录** | 为文件或项目文件夹创建可携带记录 | 一个完整的溯源 ZIP 记录包 |
| **验证记录** | 将当前文件与以前保存的记录进行核对 | 文件一致或发生变化的结果 |
| **前后对比** | 比较旧版本与新版本 | 未变化、已修改、新增和删除文件 |

---

## 📁 创建记录

| 步骤 | 操作 |
|---|---|
| **01** | 添加单个文件、多个文件或项目文件夹 |
| **02** | 填写必要记录信息 |
| **03** | 在浏览器本地计算 SHA-256 |
| **04** | 保存一个完整的溯源 ZIP 记录包 |

### 记录信息

| 项目 | 说明 |
|---|---|
| **标题** | 作品或项目名称 |
| **作者或机构** | 作者、机构或维护主体 |
| **版本** | 当前版本 |
| **日期** | 记录日期或发布日期 |
| **类型** | 内容或项目类型 |
| **记录级别** | 公开、内部、机密或受限 |
| **官方链接** | 选填的公开链接 |

### 记录级别

| 记录级别 | 适用情况 |
|---|---|
| **公开** | 已公开发布或准备公开引用的内容 |
| **内部** | 内部工作文件或项目记录 |
| **机密** | 需要控制访问的敏感文件 |
| **受限** | 仅限授权人员访问的文件 |

### 生成结果

| 结果 | 说明 |
|---|---|
| 文件数量 | 当前选择的文件数量 |
| 文件总大小 | 所有文件的合计大小 |
| SHA-256 | 文件完整性值 |
| 记录状态 | 确认记录包已经准备完成 |
| 溯源记录包 | 一个可以保存的 ZIP 文件 |

---

## 📦 生成的记录包

| 文件 | 作用 |
|---|---|
| `metadata.json` | 作品与记录的基础信息 |
| `provenance.json` | 基础溯源记录 |
| `file-integrity-records.json` | SHA-256 与文件完整性信息 |
| `release-manifest.json` | 记录包内容概览 |
| `citation.txt` | 适用于公开记录的建议引用 |
| `README.md` | 方便阅读的记录包说明 |

### 文件记录内容

| 记录项目 | 说明 |
|---|---|
| 文件名 | 原始文件名称 |
| 相对路径 | 文件在项目中的位置 |
| 文件类型 | 浏览器识别的内容类型 |
| 文件大小 | 文件字节大小 |
| 最后修改时间 | 本地文件修改时间 |
| SHA-256 | 可以重复核对的文件完整性值 |

> [!NOTE]
> 这些结构化记录统一保存在一个 ZIP 包中，使用者不需要分别下载或管理多个 JSON 文件。

---

## 🔐 公开记录与非公开记录

| 记录级别 | 结果方式 |
|---|---|
| **公开** | 可以包含建议引用和官方公开链接 |
| **内部** | 提供简洁记录信息 |
| **机密** | 提供简洁记录信息 |
| **受限** | 提供简洁记录信息 |

### 记录信息示例

| 示例 | 用途 |
|---|---|
| `项目标题 · 版本 1.0 · 机密 · 3 个文件 · SHA-256` | 私有项目记录、交付清单、存档备注或内部说明 |

需要长期保存的主要结果仍然是完整的溯源 ZIP 记录包。

---

## ✅ 验证记录

| 所需内容 | 作用 |
|---|---|
| 当前文件 | 现在需要检查的文件 |
| 以前保存的溯源 ZIP 或 `file-integrity-records.json` | 作为之前的完整性参照 |

### 验证结果

| 结果 | 含义 |
|---|---|
| **未变化** | 当前文件与以前保存的 SHA-256 一致 |
| **已修改** | 当前文件内容已经与原记录不同 |
| **新增** | 当前文件中出现了原记录没有的文件 |
| **删除** | 原记录中的文件在当前文件中已经不存在 |

> 验证过程在浏览器本地完成。

---

## ↔️ 前后版本对比

| 版本 | 作用 |
|---|---|
| 旧版本 | 以前的文件或项目文件夹 |
| 新版本 | 当前的文件或项目文件夹 |

### 对比结果

| 结果 | 含义 |
|---|---|
| **未变化** | 文件内容完全相同 |
| **已修改** | 文件内容发生变化 |
| **新增** | 文件只存在于新版本中 |
| **删除** | 文件只存在于旧版本中 |

### 常见场景

| 场景 | 示例 |
|---|---|
| 出版内容 | 比较草稿与正式发布文件 |
| 仓库项目 | 查看项目文件夹变化 |
| 长期存档 | 核对保存的不同版本 |
| 项目交付 | 比较前后交付文件 |
| 内部系统 | 检查受控文件变化 |

---

## #️⃣ SHA-256 完整性

| SHA-256 结果 | 含义 |
|---|---|
| 哈希一致 | 被比较的文件内容完全相同 |
| 哈希不同 | 被比较的文件内容已经发生变化 |

### SHA-256 不能单独证明

| 边界 | 状态 |
|---|---|
| 作者身份 | 不能证明 |
| 法律所有权 | 不能证明 |
| 原创性 | 不能证明 |
| 首次发布时间 | 不能证明 |
| 最初创作时间 | 不能证明 |

---

## 🛡️ 本地处理与隐私

| 项目 | 状态 |
|---|---|
| 文件处理 | 浏览器本地 |
| 自动上传原始文件 | 否 |
| 完整性算法 | SHA-256 |
| 记录包生成 | 浏览器本地 |
| 记录包保存 | 由使用者决定 |
| 是否公开发布 | 由使用者决定 |

> [!CAUTION]
> 涉及内部系统、方法文件或其他敏感内容时，不应把生成的记录包上传到公开仓库或公共存储位置，除非使用者明确决定公开。

---

## ⚖️ 工具边界

### 可以支持

| 支持内容 | 状态 |
|---|---|
| 基础溯源记录 | 支持 |
| 版本连续性 | 支持 |
| 文件完整性记录 | 支持 |
| 已有记录验证 | 支持 |
| 前后版本比较 | 支持 |
| 可携带项目存档 | 支持 |
| 公开记录的引用连续性 | 支持 |

### 不能提供

| 不提供的内容 | 边界 |
|---|---|
| 证明原创性 | 不提供 |
| 判断法律所有权 | 不提供 |
| 验证内容真实性 | 不提供 |
| 识别抄袭 | 不提供 |
| 判断内容是否由 AI 生成 | 不提供 |
| 解决作者争议 | 不提供 |
| 完成版权登记 | 不提供 |
| 提供独立可信时间戳 | 不提供 |
| 代替人类判断 | 不提供 |

---

## 🧾 项目信息

| 项目 | 记录 |
|---|---|
| **工具版本** | `0.3.1` |
| **当前状态** | 浏览器本地溯源记录工作台 |
| **工作模式** | 创建 · 验证 · 前后对比 |
| **处理方式** | 浏览器本地处理 |
| **完整性算法** | `SHA-256` |
| **结果形式** | 一个完整 ZIP 记录包 |
| **记录级别** | 公开 · 内部 · 机密 · 受限 |
| **概念与作者** | Xufen Tu |
| **公开地址** | [https://xufentu.com/provenance-tool/](https://xufentu.com/provenance-tool/) |

> **自动化可以支持结构，但责任必须保持可见。**

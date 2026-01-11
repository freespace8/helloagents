---
name: templates
description: 文档模板集合；创建Wiki或方案包文件时读取；包含所有知识库模板和方案文件模板
---

# 文档模板集合

使用方式：
1. 先读本文件确定要用的模板文件
2. 再只读取本目录下对应的模板文件（如 `plan-why-template.md` / `wiki-api-template.md`）并填充 `[...]`
3. 输出格式规范：以 `../SKILL.md` 的 G6.1~G6.4 为准（`output-format.md` 仅做指引）

语言规范：严格遵循 G1；除例外清单外，所有自然语言内容按{OUTPUT_LANGUAGE}生成。

---

## 模板索引

### 知识库（SSOT：`helloagents/`）

- `changelog-template.md` → `helloagents/CHANGELOG.md`
- `project-template.md` → `helloagents/project.md`
- `history-index-template.md` → `helloagents/history/index.md`
- `wiki-overview-template.md` → `helloagents/wiki/overview.md`
- `wiki-arch-template.md` → `helloagents/wiki/arch.md`
- `wiki-api-template.md` → `helloagents/wiki/api.md`
- `wiki-data-template.md` → `helloagents/wiki/data.md`
- `wiki-module-template.md` → `helloagents/wiki/modules/<module>.md`

### 方案包（`helloagents/plan/` 与 `helloagents/history/`）

- `plan-why-template.md` → `helloagents/plan/YYYYMMDDHHMM_<feature>/why.md`
- `plan-how-template.md` → `helloagents/plan/YYYYMMDDHHMM_<feature>/how.md`
- `plan-task-template.md` → `helloagents/plan/YYYYMMDDHHMM_<feature>/task.md`

### 辅助映射/规则

- `version-source-map.md`（供 G7 解析主模块/自动推断版本号用）

---

## 维护规则（强制）

- 模板正文的唯一真源是上述模板文件（如 `plan-why-template.md`）；禁止在本文件复制/内嵌模板正文（避免双源漂移）。

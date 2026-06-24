# Project_loop_001_阶段测试审查

## 模块概述

项目级阶段测试与审查技能。在每一阶段/任务完成开发后，强制执行五步测试审查流程，确保质量达标。

## 文件说明

| 文件 | 职责 |
|------|------|
| `SKILL.md` | 主技能文件，定义五步流程、验收标准、闭环规则 |
| `references/test-report-template.md` | 测试报告模板，Step 5 使用 |
| `README.md` | 本文件 |

## 五步流程

1. 全量回归测试 → `pytest tests/ -v`
2. QA 用例验证 → 按 QA 文档逐条执行
3. A/B 性能对比 → 按 A/B 文档执行对比
4. 代码审查 → 调用 `code-reviewer` 技能
5. 生成测试报告 → 输出到 `docs/test-reports/`

## 依赖

- 外部技能：`code-reviewer`
- 测试框架：pytest
- 文档：`docs/qa/`、`docs/ab/` 中的对应阶段文档
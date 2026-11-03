# 公文全案一支笔（Gongwen Yizhibi）

> 公文全流程数字员工：写作 + 排版全案包圆，一条龙交付成稿。

一个 skill、两个引擎，覆盖公文生产完整流水线：

| 引擎 | 目录 | 解决什么 | 来源 |
|---|---|---|---|
| **写作引擎** | `writing/` | 写什么、怎么写像（数据驱动内容生成） | [lieflat-gongwen](https://github.com/larashero3-dotcom/lieflat-gongwen) |
| **排版引擎** | `formatting/` | 排成 GB/T 9704-2012 标准版式 | [gongwen-gbt9704-skill](https://github.com/mizzlelover/gongwen-gbt9704-skill) |

## 快速使用

入口见根目录 `SKILL.md`，按任务意图路由：

- **起草/改写/检查公文正文** → 写作引擎（六步工作流 + 参数自检 `python3 writing/scripts/check_params.py`）
- **把材料排成公文 DOCX** → 排版引擎（`node formatting/scripts/generate_gongwen_docx.mjs` + 校验器）
- **一步到位出成品** → 全流程模式（写作 → 排版 → 交付，见 SKILL.md 第四节）

## 目录结构

```
SKILL.md                    入口：双引擎路由 + 全流程 + 输出契约
LICENSE.md                  双许可声明
writing/                    写作引擎（lieflat-gongwen）
  ├── 参数卡.md              七文体参数一页表（每次必读）
  ├── 标题技法库.md / 句子对照库.md
  ├── scripts/              check_params.py 自检器 / strip_meta.py
  ├── 公文语料/ 党建语料/     DNA 文档 + _meta 数值统计
  ├── 示例/                  22 篇合成范文
  └── 参考/法定公文样例/      7 篇真实政策文件
formatting/                 排版引擎（gongwen-gbt9704-skill）
  ├── scripts/              generate_gongwen_docx.mjs / verify_gongwen_docx.mjs
  ├── references/           标准执行摘要 / 逐条执行矩阵 / 正式公文核验表
  └── tests/fixture.md       快速验证样例
```

## 许可

双许可合并：`writing/` 为 PolyForm Noncommercial（非商业），`formatting/` 为 MIT。详见 `LICENSE.md`。

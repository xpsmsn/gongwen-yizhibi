# Changelog

## 1.0.1 (2026-11-02)

- **排版引擎**：修复图片被 28 磅固定行距（exact）压扁/裁切的问题——图片段落自动改用自动行距并关闭文档网格对齐，避免图片行在版心网格下被拉伸或导致整段跨页留白（`formatting/scripts/generate_gongwen_docx.mjs`）。
- **文档**：SKILL.md 自检命令补充 Windows 下 `python` 替代写法。

## 1.0.0 (2026-10-20)

- 首次合并发布：写作引擎（lieflat-gongwen，PolyForm NC）+ 排版引擎（gongwen-gbt9704-skill，MIT）。

# LaTeX Template Collection

一个按用途整理的 LaTeX 模板库，包含会议投稿、书籍、笔记和社媒卡片版式。模板保留原有的文件名与发布年份，方便直接复制后开始写作。

## 目录

```
templates/
├── conferences/              # 按会议与年份分类
│   └── <venue>/<year>/
└── notes/                    # 非投稿用途的写作模板
    ├── adaptive-kit/         # XeLaTeX/LuaLaTeX：书籍、笔记、社媒卡片
    │   ├── content/          # 可复用示例内容
    │   ├── examples/         # 可直接编译的入口 .tex 文件
    │   └── styles/           # 版式与颜色等公共样式
    ├── book/                 # 中文书籍排版起始模板
    ├── social/               # 社媒知识内容模板
    │   └── xhsnote/          # 长图文式中文短笔记
    └── legacy/               # 保留兼容性的历史模板
        └── archive/          # 被新版替代的基础文章与旧书籍版
```

完整清单、入口文件和本机来源记录见 [CATALOG.md](CATALOG.md)。

## 延伸案例库

[Beautiful Data Viz](beautiful-dataviz/) 是仓库内独立维护的可视化设计案例库，收录数据新闻、地图、Dashboard、数据艺术与开源实现的拆解笔记。它不包含 LaTeX 模板，也不转载原作素材。

## 快速使用

1. 选择 `templates/conferences/<venue>/<year>/` 中的入口 `.tex` 文件，连同同目录的 `.sty`、`.cls`、`.bst` 和 `.bib` 文件一并复制到你的论文目录。
2. 使用会议官方要求的编译命令与提交规则；提交前请始终核对最新 Author Kit。
3. 自适应模板可用 XeLaTeX 编译：

   ```bash
   cd templates/notes/adaptive-kit
   xelatex -output-directory=build examples/book.tex
   xelatex -output-directory=build examples/note.tex
   xelatex -output-directory=build examples/cards.tex
   ```

## 模板选择

- 需要书籍、笔记和竖版卡片三种输出时，优先使用 `notes/adaptive-kit/`。
- 需要传统中文书籍版式时，使用 `notes/book/`。
- 需要小红书式长图文笔记时，使用 `notes/social/xhsnote/`。
- `notes/legacy/` 中的文件保留为兼容参考；`legacy/archive/` 是已由新版替代的历史版本，通常不建议作为新项目起点。

## 版权与更新

本仓库只对目录编排和说明文档作出贡献。会议模板中的 `.tex`、`.sty`、`.cls`、`.bst` 与 `.bib` 文件均保留原始版权和许可；它们不是由本仓库重新授权。使用前请阅读各文件头部说明，并以会议官网最新发布的 Author Kit 为准。

未收录本机中的论文草稿、个人研究项目、课程导出物、应用内置模板及其 PDF/Word 文件，避免混入投稿内容、重复文件或许可不明确的资源。

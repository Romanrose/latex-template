# Adaptive LaTeX Kit

一套从同一组知识单元出发，分别输出书籍、独立笔记与 3:4 竖版社媒卡片的 XeLaTeX 模板。

## 设计原则

- `styles/mi-core.sty`：跨载体共用的品牌颜色、字体、数学宏与信息盒子。
- `styles/mi-book.sty`：书籍版式（6 × 9 in、章节、目录、页眉页脚、封面）。
- `styles/mi-note.sty`：A4 独立笔记版式。
- `styles/mi-card.sty`：1080 × 1440 的小红书式 3:4 竖版卡片画布，带暖色背景、强标题、信息卡片与页码组件。
- `content/`：按知识单元保存正文。书籍/笔记可以复用完整推导；卡片版应另行编辑标题、节奏和拆页。

## 编译

需要 XeLaTeX 或 LuaLaTeX。以 XeLaTeX 为例：

```bash
xelatex -output-directory=build builds/book.tex
xelatex -output-directory=build builds/note.tex
xelatex -output-directory=build builds/cards.tex
```

卡片生成 PDF 后，可用下列命令导出 1080px 宽的图片：

```bash
pdftoppm -png -scale-to-x 1080 -scale-to-y -1 build/cards.pdf output/card
```

## 从一个主题开始

1. 在 `content/<topic>/` 写可复用的定义、公式、证明与结论。
2. 在 `builds/book.tex` 和 `builds/note.tex` 按需要 `\input` 对应单元。
3. 在 `content/<topic>/cards.tex` 重新组织为一张卡一个概念；不要把长文硬缩进图片。

示例主题为「典型集」。

# Adaptive Kit

同一套知识内容可生成三种 XeLaTeX/LuaLaTeX 输出：6 × 9 英寸书籍、A4 笔记和 3:4 竖版社媒卡片。

- `examples/`：编译入口；从这里开始编辑标题、作者和所引用的内容。
- `content/`：可按主题组织的可复用正文与卡片内容。
- `styles/`：跨载体共用的字体、颜色、数学宏和版式文件。

在此目录中运行：

```bash
xelatex -output-directory=build examples/book.tex
xelatex -output-directory=build examples/note.tex
xelatex -output-directory=build examples/cards.tex
```

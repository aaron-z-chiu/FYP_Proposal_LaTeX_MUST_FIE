# 澳科大毕设 Proposal LaTeX 模板

[英语版本 / English Version](README.md)

本仓库提供一个适用于 **澳门科技大学创新工程学院计算机科学与工程学院 Final Year Project Proposal** 的 LaTeX 模板。

该模板根据官方 Microsoft Word 模板进行重建，目标是在 XeLaTeX 中尽可能忠实地复现原始 Word 模板的版式与格式。

## 使用方法

本模板需要使用 **XeLaTeX** 编译。

### Overleaf

1. 将项目文件上传到 Overleaf。
2. 打开 **Menu → Settings**。
3. 将编译器设置为：

   ```text
   XeLaTeX
   ```

4. 将 `main.tex` 设置为主文件。
5. 重新编译项目。

*提示：由于需要加载字体文件，overleaf 免费版的编译时长可能不够，建议购买学生会员使用*

## 项目结构

```text
.
├── main.tex
├── must_proposal.sty
├── reference.bib
├── mustplain.bst
├── assets/
│   ├── image1.jpeg
│   └── water-fall.jpg
└── fonts/
```

- `main.tex`  
  主文档。项目基本信息以及 Proposal 正文内容均在此文件中修改。
- `must_proposal.sty`  
  定义页面尺寸、字体、封面、目录、章节标题、页码及其他格式。
- `mustplain.bst`
  定义参考文献格式
- `reference.bib`  
  用于存放 Proposal 中使用的 BibTeX 参考文献条目。可在 `main.tex` 中通过 `\cite{...}` 进行引用。参考文献列表会自动按照第一作者姓氏的字母顺序排列。
- `assets/`  
  存放模板所需的图片资源。
- `fonts/`  
  当编译环境中不存在模板所需字体时，可在此目录中放置本地字体文件。

## 字体

为了尽可能忠实地复现原始 Word 模板，本模板使用原模板中的字体。

其中，**Calibri 默认并未安装在 Overleaf 上**。

如果编译时提示找不到 Calibri，请自行通过合法来源获取对应字体文件，并将其放入 `fonts/` 目录。

模板预期使用以下文件名：

```text
fonts/calibri.ttf
fonts/calibrib.ttf
fonts/calibrii.ttf
fonts/calibriz.ttf
```

它们分别对应：

- `calibri.ttf`：Calibri Regular（常规）
- `calibrib.ttf`：Calibri Bold（粗体）
- `calibrii.ttf`：Calibri Italic（斜体）
- `calibriz.ttf`：Calibri Bold Italic（粗斜体）

由于版权限制，本仓库**不会分发这些字体文件**，请自行通过适当且合法的来源获取所需字体。

模板不会自动将 Calibri 替换为其他字体，因为字体替换可能导致换行、文字宽度、间距及整体版式发生变化。

## 修改 Proposal 内容

项目基本信息可在 `main.tex` 中修改，例如：

```latex
\projecttitle{...}
\studentname{...}
\studentno{...}
\supervisor{...}
\proposaldate{...}
```

Proposal 正文可在对应章节中编写，包括：

- Abstract
- Contributions
- Introduction
- Objectives
- Related Work
- Methodology
- Required Hardware and Software
- Project Planning
- References

## 说明

本模板的目标是尽可能还原官方 Word 模板。由于 Microsoft Word 与 XeLaTeX 使用不同的排版和 PDF 渲染引擎，最终输出仍可能存在极小的渲染差异。

除非确实需要修改模板格式，否则不建议直接修改 `must_proposal.sty`。

## 联系方式

如果在使用本模板时遇到任何问题，请联系：

**Aaron**: aaron.z.chiu@gmail.com 或 zechengq@student.must.edu.mo

## 免责声明

本仓库为对应 MUST Final Year Project Proposal 模板的非官方 LaTeX 重建版本，并不代表澳门科技大学官方发布或维护。

尽管本模板已尽可能按照官方 Microsoft Word 模板进行排版还原，但由于 Microsoft Word 与 XeLaTeX 使用不同的排版和渲染机制，无法保证最终输出与官方 Word 文档在所有情况下均达到 100% 一致。

使用本模板前，请自行核对学校当前有效的格式要求及提交规范。因使用本模板而产生的排版差异、格式不符合要求、提交问题或其他相关后果，由使用者自行承担。

澳门科技大学的名称及校徽归其相应权利人所有，本仓库仅将其用于复现学校学术模板。

Microsoft 字体（如 Calibri）不会随本仓库分发。用户应自行通过适当且合法的来源获取所需字体。

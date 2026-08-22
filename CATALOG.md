# Template Catalog

## Conference templates

| Venue | Year | Entry point | Notes |
| --- | --- | --- | --- |
| AAAI | 2026 | `templates/conferences/aaai/2026/AnonymousSubmission/LaTeX/anonymous-submission-latex-2026.tex` | Includes anonymous submission, camera-ready and reproducibility-checklist variants. |
| AAAI | 2027 | `templates/conferences/aaai/2027/AnonymousSubmission2027.tex` | Includes camera-ready and reproducibility-checklist entry points. |
| ACL | 2026 | `templates/conferences/acl/2026/acl2026.tex` | Includes `acl.sty` and `acl_natbib.bst`. |
| ACM Multimedia | 2026 | `templates/conferences/acm-mm/2026/acm_mm2026.tex` | Includes `acmart.cls` and `acm.bst`. |
| CVPR | 2026 | `templates/conferences/cvpr/2026/cvpr2026.tex` | Includes `cvpr.sty` and `cvpr.bst`. |
| ICLR | 2026 | `templates/conferences/iclr/2026/iclr2026.tex` | Includes the conference style and bibliography style. |
| ICML | 2026 | `templates/conferences/icml/2026/icml2026.tex` | Includes `icml2026.sty`. |
| IEEE | — | `templates/conferences/ieee/ieee_conference.tex` | Includes conference and journal examples plus `IEEEtran`. |
| IJCAI-ECAI | 2026 | `templates/conferences/ijcai-ecai/2026/ijcai26.tex` | Includes the required style and bibliography files. |
| NeurIPS | 2026 | `templates/conferences/neurips/2026/neurips2026.tex` | Includes `neurips_2026.sty`. |

## Notes and books

- `templates/notes/book/main.tex`：中文书籍排版示例。
- `templates/notes/legacy/`：中文、英文、文章、书籍与短笔记起始文件。
- `templates/notes/adaptive-kit/examples/book.tex`：6 × 9 英寸书籍示例。
- `templates/notes/adaptive-kit/examples/note.tex`：A4 独立笔记示例。
- `templates/notes/adaptive-kit/examples/cards.tex`：1080 × 1440 的竖版社媒卡片示例。

## Provenance

The conference files were collected from locally stored conference Author Kits and reference templates. The versions are intentionally preserved as named in the files. This repository is a convenience index, not an official distribution; always download the latest kit from the relevant conference before submission.

## Deliberately excluded local material

- Working papers and project copies, including Concept2Fable and AeroDocBench.
- TeXShop’s built-in templates and stationery, which are application-bundled resources.
- Generated course exports, dependency folders, caches, PDFs and Word documents.
- Duplicate copies of styles already represented by `templates/notes/adaptive-kit/`.

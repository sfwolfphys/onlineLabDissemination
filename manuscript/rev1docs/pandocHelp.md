# Pandoc Help

## Article [How to Convert from Latex to MS Word with 'Pandoc'](https://medium.com/@zhelinchen91/how-to-convert-from-latex-to-ms-word-with-pandoc-f2045a762293)

- Citations - Requires `pandoc-citeproc`

```
pandoc mydoc.tex --bibliography=myref.bib -o mydoc.docx
```

- Use template Word doc for formatting:

```
pandoc mydoc.tex --bibliography=myref.bib --reference-docx=IEEE_template.doc -o mydoc.docx
```

- Cross References (Requires [`pandoc-crossref`](https://github.com/lierdakil/pandoc-crossref/releases/tag/v0.3.4.0c))

```
pandoc mydoc.tex --filter pandoc-crossref --bibliography=myref.bib --reference-docx=IEEE_template.doc -o mydoc.docx
```


# Qubes OS Cheat Sheet

This cheat sheet contains commands and examples for [Qubes OS](https://www.qubes-os.org/).

## Downloads

- **Markdown (Text): [qubes-cheatsheet.md](https://github.com/Jeeppler/qubes-cheatsheet/blob/master/qubes-cheatsheet.md)**

- **PDF: [qubes-cheatsheet.pdf](https://github.com/Jeeppler/qubes-cheatsheet/raw/master/qubes-cheatsheet.pdf)**

- **HTML: [qubes-cheatsheet.html](https://htmlpreview.github.io/?https://github.com/Jeeppler/qubes-cheatsheet/blob/master/qubes-cheatsheet.html)**

- **Text: [qubes-cheatsheet.txt](https://github.com/Jeeppler/qubes-cheatsheet/raw/master/qubes-cheatsheet.txt)**

*The files are generated with the help of [`generate.sh`](https://github.com/Jeeppler/qubes-cheatsheet/blob/master/generate.sh)*

## Other formats

The PDF and HTML file is generated by using [Pandoc](http://pandoc.org/).

Pandoc can generate different files from one [markdown](http://daringfireball.net/projects/markdown/) text file.


```bash
# outputs the qubes cheat sheet as PDF file
pandoc metadata.yaml qubes-cheatsheet.md -s -o qubes-cheatsheet.pdf

# outputs the qubes cheat sheet as HTML (HTML5) file
pandoc metadata.yaml qubes-cheatsheet.md -s -S -t html5 -o qubes-cheatsheet.html

# outputs the qubes cheat sheet as plain text
pandoc qubes-cheatsheet.md -s -S -t plain -o qubes-cheatsheet.txt
```

`qubes-cheatsheet.md` is the input file and `qubes-cheatsheet.xxx` the output file.

`metadata.yaml` contains some additional metadata information for the PDF and HTML generation.

Pandoc is furthermore able to generate files for asciidoc, odt, docx, textile and many more. Please have a look at [Pandoc Demos](http://pandoc.org/demos.html).

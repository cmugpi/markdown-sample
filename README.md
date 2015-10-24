# Example Pandoc Markdown Document

This document presents part of the solution to the problem described in [this
repository][latex-sample] using Pandoc Markdown instead of plain LaTeX. If you
haven't browsed that repo yet, you should take a quick look.

Compare the readability of the [Markdown source][source] to the [LaTeX
source][latex-source] from that repo. In general, when using Pandoc Markdown
instead of LaTeX you can get by with much simpler text (though you sacrifice a
little power). You can also see the [compiled output](written.pdf), which looks 
basically the same as the PDF generated from before.

[latex-sample]: https://github.com/cmugpi/latex-sample

[source]: https://raw.githubusercontent.com/cmugpi/markdown-sample/master/written.md
[latex-source]: https://github.com/cmugpi/latex-sample/blob/master/written.tex

## Compiling

The `Makefile` contains a number of targets that let you compile the Markdown
file to a PDF if you have `pdflatex` and `pandoc` installed. In particular, you
can run `make view` to compile the PDF and open it in your default PDF viewer.

You can reuse this Makefile across Pandoc Markdown projects to compile them into 
PDFS. The only thing that you will have to change is the first line of it:

```make
TARGET=written
```

For this assignment, we've called our file `written.md`, and the value of
this `TARGET` variable is set appropriately. Just make sure to change it if you
call your LaTeX file something else.

## License

MIT License. See LICENSE.

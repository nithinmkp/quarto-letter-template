# [Quarto](https://quarto.org/) letter template example

This example shows how to create/adjust your own [Quarto](https://quarto.org/)
template so that you can write nice-looking letters in Markdown with logos and
stuff.


## Resources which I have used

- https://github.com/numbats/monash-quarto-letter used as inspiration but not used
  directly since it looked too sophisticated to me.
- Example logo from https://logoipsum.com/.



## Example

- This is the source file in Markdown:
  [letter.md](https://raw.githubusercontent.com/bast/quarto-letter-template/main/letter.md)
- And this is how the generated PDF looks: [letter.pdf](letter.pdf)


## How to build the PDF

```console
$ quarto render letter.md
```


## Meaning of the files

```
├── _extensions
│   └── letter                <- you can rename it but then also rename it inside letter.md
│       ├── _extension.yml    <- here you define which files are needed
│       ├── logo.png
│       ├── signature.png
│       └── template.tex      <- here you define the layout in LaTeX
├── letter.md                 <- you write this
├── letter.pdf                <- quarto generates this
├── LICENSE
└── README.md
```

The `_extensions` part you can reuse across letters. The idea is that the
extension defines all that is common for all your letters (logo, address,
layout). You can also share your extensions via [Quarto](https://quarto.org/)
(but I haven't tried it yet).

You can modify [template.tex](_extensions/letter/template.tex) to your heart's
content but it requires some know-how in LaTeX.

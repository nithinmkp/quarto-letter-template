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

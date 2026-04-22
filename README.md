# Grammaticality needs more than locality

A *Trends in Cognitive Sciences* Letter replying to Gibson (2026),
["Dependency syntax as the simplest theory of grammar"](https://doi.org/10.1016/j.tics.2026.03.002).

**Author:** Brett Reynolds (Humber Polytechnic & University of Toronto)

## The argument

Gibson's Letter advances two distinguishable claims: a representational one
(syntax is *just* dependency rules) and an explanatory one (dependency
locality is the single load-bearing mechanism behind processing and
word-order regularities). The locality case is strong and the Letter's
evidence supports it. The broader title claim (dependency grammar as
*the simplest theory of grammar*) is a scope overclaim.

Three dissociations push against a single-factor story:

1. **Form-meaning licensing.** English *I have 57 years* has the same
   dependency skeleton on a duration reading (licensed) and an age reading
   (not licensed in contemporary Standard English). The difference is
   conventional, not geometric.
2. **Selective island satiation.** Six of seven English islands satiate
   reliably under repeated exposure; the Left Branch Condition doesn't
   (Lu, Frank & Degen 2024). A single simplicity factor would predict
   roughly uniform relaxation.
3. **Grammatical asymmetry in agreement attraction.** Wagers, Lau &
   Phillips (2009) find attraction effects concentrated in ungrammatical
   strings. Memory-load alone would not predict this asymmetry.

Gibson's own concluding remarks describe dependency grammar as "the
simplest formalism for how words are connected to one another within
a sentence." That narrower claim is the one the evidence supports.

## Building

Requires **XeLaTeX** (not pdfLaTeX) and **biber**. The preamble uses
Charis SIL; the build will fall back if it's not installed but the PDF
will look different.

```bash
# Full build
xelatex main.tex
biber main
xelatex main.tex
xelatex main.tex

# Or via Makefile
make
```

## Repository structure

```
main.tex                      # the Letter
references-standalone.bib     # self-contained bibliography (8 entries)
.house-style/                 # LaTeX preamble + style conventions
Makefile                      # build automation
main.pdf                      # prebuilt output (for readers)
```

## Bibliography

The repo is self-contained. The house-style preamble prefers
`references-standalone.bib` when present, so clones don't need the
portfolio-wide central bibliography.

## Citation

If you wish to cite this Letter while it is under review, please use:

```
Reynolds, Brett. 2026. Grammaticality needs more than locality.
Preprint. https://github.com/BrettRey/Reply_to_Gibson_on_dependency_syntax
```

## AI-assisted drafting

Per Elsevier/Cell author policy, this Letter discloses the use of Claude
(Anthropic) during preparation for argument development, structural
review, and prose drafting. The author reviewed and revised all content
and takes full responsibility for the final text.

## License

[CC BY 4.0](LICENSE). Reuse and adaptation welcome with attribution.

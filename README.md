# Paper presentation template

## TODO

After cloning this template with
```bash
git clone --recursive "this repo URL here" ## the --recursive options is VERY important
```
one should rename a few files and edit some other files.

In particular, one should decide the presentation file name, and rename files accordingly.

Our conventions is as follows.
Given:
- the `i`-th author's surname initial `Ni`
- the acronym `VENUE` of the venue where the presentation will be held
- the current year `20XX`

The presentation file name should then be:

> `N1N2N3N4-VENUE-20XX-talk`

Accordingly, one should now:
1. rename file `abcd-venue-20XX-talk.bib` into `N1N2N3N4-VENUE-20XX-talk.bib`
2. rename file `abcd-venue-20XX-talk.sty` into `N1N2N3N4-VENUE-20XX-talk.sty`
3. rename file `abcd-venue-20XX-talk.tex` into `N1N2N3N4-VENUE-20XX-talk.tex`
4. replace line 10 of the `.tex` file from `\usepackage{abcd-venue-20XX-talk}` to `\usepackage{N1N2N3N4-VENUE-20XX-talk}`
5. replace line 249 of the `.tex` file from `\bibliography{abcd-venue-20XX-talk}` to `\bibliography{N1N2N3N4-VENUE-20XX-talk}`
6. replace line 16 of the `.github/workflows/compile.yml` file from `LATEX_ROOT: abcd-venue-20XX-talk` to `LATEX_ROOT: N1N2N3N4-VENUE-20XX-talk`
    + take care of _not_ changing any indentation in the `.yml` file
7. replace line 1 of the `.gitignore` file from `abcd-venue-20XX-talk.pdf` to `N1N2N3N4-VENUE-20XX-talk.pdf`
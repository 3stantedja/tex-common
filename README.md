# tex-common
Common custom packages used in TeX-based repos. Currently they are used in most of my TeX-based documents.

## Packages
### `problems`
This contains a baseline setup for me to start writing documents. Basically this aims to shorten the preamble portion of my TeX documents so that I could see its content without a lot of scrolling. As such, the package only contains all the packages that I would've imported as well as some formatting and package settings.

It was named as such because (as I would explain a bit later) I was primarily using this for doing my AUMAT 250 problems, and it got tedious copying the preamble every time I wanted to do more write-ups.

### `lg_jsylvest`
This contains all macros that were used in an older version of (Elementary Foundations)[https://sites.ualberta.ca/~jsylvest/books/EF/] textbook; during my time in AUMAT 250 I got too lazy to figure out which macros aliases to which sequence of commands in LaTeX as I was copying the questions and equations for my assignments at the time. A bit of sleuthing with Inspect Elements later, I found a complete set of macros that he used for the textbook, so they're reproduced here in full.

The name of the package was from both one of the (incomplete) prefixes that I saw at the time, and the professor that taught me AUMAT 250 both in Fall 2019 and Fall 2020, Jeremy Sylvestre. If you're reading this, hi! I hope you don't mind the macros being in this package. (also sorry for the trouble i've caused you!)

## How to use
Clone this repository as a submodule in your existing LaTeX repo (or as a separate repo nested in your project). Then adjust your `TEXINPUTS` path (in my case via `.latexmkrc`) so that your build system (in my case `latexmk`) will try to find it.

Now, add any of the packages in your preamble. Options are not available for now. Currently the only exposed "interfaces" (for a lack of a better term) is the title, date, and author name.

## Requirements
This requires a TeX distribution. I do recommend using `latexmk` as a build system if possible (as I've not tested other build system yet).

- `amsmath`
- `cancel`
- `mathrsfs`
- `microtype`
- (finish this list)

## Comtributing
Fork this repo to your local machine. Then add your changes and push it to your repo. After that add a pull request.

Additional instructions will be added later

## To-do
- [ ] add options to disable certain packages if necessary
- [ ] move command definitions to a separate .sty file
- [ ] add more detailed documentations here
    - [ ] finish up dependencies
    - [ ] add command line examples
    - [ ] add `.latexmkrc` example
    - [ ] add package descriptions (could be pulled straight from the packages?)

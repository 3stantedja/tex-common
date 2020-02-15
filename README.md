# tex-common
Common custom packages used in TeX-based repos. Currently they are used in `aumat250-problem-proving`.

## Packages
### `problems`

### `lg_jsylvest`

## How to use
Clone this repository as a submodule in your existing LaTeX repo (or as a separate repo nested in your project). Then adjust your `TEXINPUTS` path (in my case via `.latexmkrc`) so that your build system (in my case `latexmk`) will try to find it.

Now, add any of the packages in your preamble. Options are not available for now. Currently the only exposed "interfaces" (for a lack of a better term) is the title, date, and author name.

## Requirements
This requires a TeX distribution. I do recommend using `latexmk` as a build system if possible (as I've not tested other build system yet).

- `amsmath`
- `cancel`
- `microtype`
- (finish this list)

## Comtributing
Fork this repo to your local machine. Then add your changes and push it to your repo. After that add a pull request.

Additional instructions will be added later

## To-do
[ ] add options to disable certain packages if necessary
[ ] move command definitions to a separate .sty file
[ ] add more detailed documentations here
    [ ] finish up dependencies
    [ ] add command line examples
    [ ] add `.latexmkrc` example

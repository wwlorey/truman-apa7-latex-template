# truman-apa7-latex-template

A simple APA7 LaTeX template in a flavor defined by the Truman State University Counseling Program.

## Requirements

* `xelatex`
* `biber`
* the LaTeX packages in `truman-apa7-template.tex`

## Usage

1. Clone this repository.
2. Make your changes to `truman-apa7-template.tex`. Rename the file as desired.
3. Build a PDF using the `build` script. `build` looks for the first `.tex` file
found in your current directory and runs `xelatex` on it.
  ```bash
  ./build
  ```
  If making changes to references, build with the following command to incorporate those changes.
  ```bash
  ./build --bib
  ```
  The `--bib` flag searches for the first `.bcf` file in your current directory (which is
  generated from your `.bib` file) and runs `biber` on it.

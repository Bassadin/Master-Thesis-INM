# Master-Thesis-INM

My master's thesis in Computer Science during the summer semester 2023 about Localization in LoRa-based networks at [HFU Furtwangen University](https://www.hs-furtwangen.de/).
This repo will get updated during the semester.

## PDF

Ready-made PDFs available in the [Releases section](https://github.com/Bassadin/Master-Thesis-INM/releases)

## LaTeX

The LaTeX source code is located in the `thesis` folder.

### Building your own PDF

1. Install [TeX Live](https://www.tug.org/texlive/)
2. `cd thesis`
3. `make`
4. Enjoy your `main.pdf`!

### Useful regexes

- `^(?!%)(?<!\{)[A-Z]{2,}\b`: Find all abbreviations without latex abbreviation.
- `\.(?!\n|$)`: Find all dots without a following newline.
- Find all contractions that aren't in lines that are commented out: `(?<!%)(\b\w{1,3}'\w{1,3}\b)(?!%)`

### Useful commands

- When using LaTeX Workshop in VSCode
  - `CTRL+ALT+V` to open the PDF in the integrated PDF viewer
  - `CTRL+ALT+J` to jump to the corresponding position in the PDF

#### Word count

- `detex main.tex | Measure-Object -word`: Count words in `main.tex` (Windows PowerShell)
- `cd thesis` && `texcount -inc .\main.tex -total -sum`: Count several things in `main.tex`

## Other parts of this thesis

- [API/Backend](https://github.com/Bassadin/ttn-locator-backend)
- [Frontend](https://github.com/Bassadin/ttn-locator-frontend)
- [Other Code, e.g. for LoRaWAN clients, etc.](https://github.com/Bassadin/Master-Thesis-INM-Clients-Code)

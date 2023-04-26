# Master-Thesis-INM

My master's thesis in Computer Science during Summer Semester 2023 about Localization in LoRa-based networks at [HFU Furtwangen University](https://www.hs-furtwangen.de/).
The repo will get updated during the semester.

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

- `(?<!\\ac\{)(\b[A-Z]{2,}\b)(?!\})`: Find all abbreviation without `\ac{}`.

## Other parts of this thesis

- [API/Backend](https://github.com/Bassadin/ttn-locator-backend)
- [Frontend](https://github.com/Bassadin/ttn-locator-frontend)

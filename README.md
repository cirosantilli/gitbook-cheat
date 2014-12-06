# GitBook Cheat

## Command line

Source: <https://github.com/GitbookIO/gitbook>

Install:

    npm install gitbook -g

Develop:

    gitbook serve

Build PDF: first install Calibre. On Ubuntu 14.04:

    sudo apt-get install calibre

Then:

    gitbook build -f pdf

Upload: first create the project on `gitbook.io`. Then:

    git push https://git.gitbook.com/<username>/<project>.git

Git will ask for you username and password.

## Directory structure

TODO

-   `README.md`: automatically appears as the first chapter named `Introduction`.

    Does not need to be included in the `SUMMARY.md`.

-   `SUMMARY.md`: list of files to be included in the book.

    The sidebar index title contains the like content, not the `h1` of the files there.

    The URL of files is determined by their path alone.

    This file should contain a single list of lists or markdown links.

-   `cover.jpg` and `cover_small.jpg`

-   `d/README.md`, `d2/README.md`:

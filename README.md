# Books by TED Speakers — Verified Catalogue

Every book on Books Worth Reading that was written by a TED speaker, as one table: **1,278 books by 620 speakers** (snapshot of 17 November 2026).

- Canonical source and living version: https://www.books-worth-reading.com/dataset
- Methodology and analysis: https://www.books-worth-reading.com/study/ted-speaker-books

## Files

| File | Format |
|---|---|
| `data/ted-speaker-books.csv` | CSV, UTF-8, one row per book |
| `data/ted-speaker-books.json` | JSON, the same rows under `books`, plus snapshot metadata |

## Fields

| Field | Meaning |
|---|---|
| `title`, `subtitle` | Book title and subtitle |
| `speaker` | The TED speaker the book is attributed to |
| `all_authors` | All authors, separated by `; ` |
| `published_date` | Publication date or year, as recorded for the listed edition |
| `publisher` | Publisher of the listed edition |
| `category`, `subcategory` | Topic category (14 categories) and subcategory |
| `isbn10`, `isbn13` | ISBNs of the listed edition |
| `language` | Language code (all `en`) |
| `book_url` | The book's page on books-worth-reading.com |
| `speaker_url` | The speaker's page, with their TED talk |

## How the catalogue is built

A book enters the catalogue only when it passes the site's publication gate. The gate requires a confirmed match between the book's author and the TED speaker, an ISBN, a cover and an English-language edition. Namesake authors were removed in an audit with human review. Book descriptions are not part of this dataset.

## Known limitations

- The data describes one edition per book, which is not always the first edition. So `published_date` and `publisher` can belong to a later or foreign edition.
- A small number of rows have wrong publication dates.
- The catalogue changes over time. This repository is a snapshot. The living version is at the canonical source above.

## Licence and citation

The data is licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). You may share and adapt it, also commercially, if you credit **Books Worth Reading** and link to https://www.books-worth-reading.com/dataset.

Citation details are in `CITATION.cff`.

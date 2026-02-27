Contribution Guidelines
====

## Adding a book to the main list

Add books with this format:

```
### DATE - [BOOK NAME](BOOK URL)

<img src="gobooks/covers/COVER_FILENAME" width="120px"/>

BOOK DESCRIPTION

```

* Place cover images in `gobooks/covers/` with a slug filename (e.g. `book-name.jpg`).
* If book is free, add it after free books of that category and also add `*Free*` after book url.
* Add other books in ascending date order (newest last). Books without date go at the end of the list in that category.
* To keep track of the huge table of contents you can use a plugin like [Markdown VSCode plugin](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one)

## Adding a book in another language

If a Go book exists in a language that already has a page (`gobooks/README-<lang>.md`), add it to that file using the same format as the main list. Write the book description in that language. Cover images go in `gobooks/covers/` as usual.

## Adding a new language

If no page exists yet for a language:

1. Create `gobooks/README-<lang>.md` using the [ISO 639-1](https://en.wikipedia.org/wiki/List_of_ISO_639_language_codes) language code (e.g. `README-ja.md` for Japanese).
2. Use the title **Go Books** translated into that language as the page heading (e.g. `# Go ブックス`).
3. Write the introductory description in that language. Keep it simple: state that this is a complete list of Go books available in that language.
4. List books using the same card format as the main README. All descriptions must be written in that language.
5. For right-to-left languages (Arabic, Farsi, Hebrew, etc.), wrap the entire content in `<div dir="rtl"> ... </div>`.
6. Add a link to the new page in the language bar at the top of `README.md`:
   ```
   **Other languages:** ... · [Language name in its own script](gobooks/README-<lang>.md)
   ```

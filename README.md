# reader-library

Public-domain books in reader-markdown, for reading, annotating and, in time, citing and including from other documents ([reader#71](https://github.com/jzheaux/reader/issues/71)).

| Book | File | Cited by |
| --- | --- | --- |
| Jane Austen, *Pride and Prejudice* (1813; George Allen, 1894) | [austen/pride-and-prejudice.md](austen/pride-and-prejudice.md) | chapter.paragraph, and page |
| Herman Melville, *Moby-Dick* (1851) | [melville/moby-dick.md](melville/moby-dick.md) | chapter.paragraph |
| William Shakespeare, *Hamlet* | [shakespeare/hamlet.md](shakespeare/hamlet.md) | act.scene.line |
| William Shakespeare, *The Sonnets* (1609) | [shakespeare/sonnets.md](shakespeare/sonnets.md) | sonnet.line |
| Plato, *The Republic*, tr. Jowett | [plato/republic.md](plato/republic.md) | book.paragraph |
| Marcus Aurelius, *Meditations*, tr. Casaubon | [marcus-aurelius/meditations.md](marcus-aurelius/meditations.md) | book.section |
| Lao-Tse, *The Tao Teh King*, tr. Legge | [lao-tzu/tao-te-ching.md](lao-tzu/tao-te-ching.md) | chapter.verse |
| Sun Tzŭ, *The Art of War*, tr. Giles | [sun-tzu/art-of-war.md](sun-tzu/art-of-war.md) | chapter.verse |
| *The King James Version of the Bible* (1611) | [bible/king-james.md](bible/king-james.md) | book.chapter.verse |
| *The Book of Mormon* (1830) | [book-of-mormon/book-of-mormon.md](book-of-mormon/book-of-mormon.md) | book.chapter.verse |

## How a book is written

- **Front matter** says what it is: `title`, `author`, `translator`, `published`, the `edition` its page numbers are from, and `cite`, how a place in it is named.
- **Headings** for its parts: `##` for a book, act or chapter, `###` for what's under it.
- **A paragraph to a line.** Verse keeps its lines, each but the last ending in `\`, and an indented line is set in with no-break spaces. A play's speech is its speaker in bold on a line of its own, then the lines; stage directions are in italics.
- **Numbers that are the citation are kept in the text** as printed: verses (`1:1`, `3.`), sections (`IV.`). Paragraphs and lines are counted.
- **`{p.12}`** is where printed page 12 begins, in the edition named.
- Text reader would read as its own syntax is escaped with `\` (`\1.`, `\A:`), so it reads as printed.

## Where they come from

Converted from Project Gutenberg's HTML by reader-authors' [`author gutenberg`](https://github.com/jzheaux/reader-authors/tree/main/authors/gutenberg), each from its eBook number there, with pictures, contents pages and Gutenberg's own pages left out: 1342, 2701, 1524, 1041, 1497, 2680, 216, 132, 10 and 17. To bring them in again:

```
author gutenberg --all --out ../reader-library --force
```

The texts are in the public domain in the United States.

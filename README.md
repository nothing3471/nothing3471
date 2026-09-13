## nothing3471

I write small tools to solve my own problems. Windows, mostly Python, mostly
standard library — if a thing needs an install script before you can try it, I have
usually done something wrong.

Most of these start the same way: something I needed either did not exist or refused
to export.

### Out now

**[reddit-link-rot](https://github.com/nothing3471/reddit-link-rot)** — I archived
33,716 saved Reddit posts and 10,326 of them pointed at media that no longer loads.
So I measured how much was actually recoverable, ran the recovery, and scored the
forecast against what came back. At least 70% is recoverable at full quality, and
which host the link points at decides almost everything — 92% for direct imgur, 0%
for imgur albums. The write-up, the per-host numbers and the audit code.

**[steam-library-export](https://github.com/nothing3471/steam-library-export)** —
Steam has no export button and its library page is virtualised, so you cannot
copy-paste it either. One Python file, no dependencies, pulls the whole library
through the official Web API and writes CSV, a readable report, and the raw JSON.

**[docorg](https://github.com/nothing3471/docorg)** — points at a folder of PDFs and
EPUBs, extracts text and existing metadata, asks a locally-hosted model what each
document actually is, and writes the result back. Nothing leaves your machine. Built
against a real library of ~44,000 files, and most of the design is scar tissue from
that.

### Next

A Steam Deck diagnostic plugin.

A bulk media archiver: resumable, survives hard kills, classifies failures into
retry and dead. It is the most sophisticated thing here and the most entangled with
my own data, so it goes last.

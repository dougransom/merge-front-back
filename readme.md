# merge-front-back

Merge two single-sided scanned PDFs into a duplex document.

This command-line tool takes:
- `front.pdf`: odd-numbered pages scanned in forward order
- `back.pdf`: even-numbered pages scanned in reverse order

It interleaves the pages to produce a properly ordered duplex PDF.

## Features
- Automatic reversal of back pages
- CLI interface with `--verbose` and `--dry-run` options
- Error handling for page count mismatches

## Installation

This project uses [Flit](https://flit.pypa.io) and is compatible with [uv](https://github.com/astral-sh/uv).

```bash
uv venv
source .venv/bin/activate
uv pip install -e .

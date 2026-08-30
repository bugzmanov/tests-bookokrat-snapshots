# bookokrat-goldens

Golden screenshots for [bookokrat](https://github.com/bugzmanov/bookokrat)'s
VHS visual regression tests (real-terminal screenshot comparisons).

This lives outside the main repo so app clones stay light — PNGs don't
delta-compress and every re-bless would bloat the main repo's history forever.

## Usage

Clone into the main repo's golden directory (it is gitignored there):

    git clone https://github.com/bugzmanov/bookokrat-goldens vhs_tests/golden

Then run tapes as usual (`./vhs_tests/run.sh --terminal kitty`). Re-blessing
(`--update` / `--accept`) writes new PNGs here; commit and push them from this
directory.

Layout: `<terminal>/<tape>/<screenshot>.png`

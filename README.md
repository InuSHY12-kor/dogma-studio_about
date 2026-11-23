# Restriction enzyme data from REBASE

These two tables are the restriction enzyme data used by Dogma Studio. They come
from REBASE, the Restriction Enzyme Database, and are published here so that
information taken from REBASE remains open and accessible, as REBASE asks.

## Files

- `enzyme-sites.tsv` — 638 enzymes: recognition site, and where the cut
  falls on each strand.
- `enzyme-suppliers.tsv` — 1937 supplier-and-enzyme entries, across the
  14 companies REBASE lists: which company sells which enzyme, and the
  temperature it works at.

Both are tab-separated plain text with a comment header. They are written by
`tools/export-rebase-data.js` from the tables the program ships, so what is here
and what the program carries are the same.

## Citation

Roberts RJ, Vincze T, Posfai J, Macelis D. REBASE: a database for DNA restriction and modification: enzymes, genes and genomes. Nucleic Acids Research 2023;51(D1):D629-D630. doi:10.1093/nar/gkac975, PMID 36318248

REBASE asks to be cited by its latest review. If a newer one has appeared, that is
the one to cite.

## REBASE

<https://rebase.neb.com> — maintained by New England Biolabs.

> REBASE is an open database provided to benefit the scientific community.
> Adaptation or distribution of information from REBASE should also remain open
> and accessible to the public.

## What is not here

Buffer names and the activity of an enzyme in a supplier's buffers are not in
these files. REBASE carries no buffer information; that part comes from each
supplier's own published catalogue and is theirs, not REBASE's.

350 further supplier-and-enzyme entries are also left out, covering
6 companies REBASE does not list: CinnaGen, Enzynomics, GeNei, Jena Bioscience, NZYTech, Yeasen. They sell
restriction enzymes, but REBASE does not carry them, so what the program knows about
them did not come from REBASE and is not published here under its name.

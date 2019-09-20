# Week 4 Project Report (2019-09-19)

## Four-Up Status

### What's been done since the last update?

* Nick Mosher
  * Updated the project website with week3 updates.
  * Wrote up team process methodology.

### What's currently in progress?

* Nick Mosher
  * Writing the week 4 project updates.

### What do we need to accomplish our goals?

* Github repositories for the frontend and backend to be
  provisioned.
* Cloud resources for deploying our solution. AWS has been
  mentioned, is that being provided by the sponsor or will
  we be expected to pay for resources out of pocket?

### What are some risks we're facing?

* The desired data visualization strategy is not strongly
  defined. It seems we have some flexibility to "figure out
  what will be useful", but there's a risk that since we're
  not true domain experts we may have trouble identifying
  a visualization technique that's actually useful.
* This project seems like it is dealing with a sizeable
  dataset, yet we've been constrained to using
  Javascript/Typescript for the backend, languages which are
  known not to have great performance characteristics. We
  may experience latency in our application if the backend is
  not able to process queries fast enough.

## Project Synopsis

The team at Phoenix Bioinformatics provides services for the scientific
community by providing a curated dataset of information about the
Arabidopsis Thaliana genome. In order to provide these services, Phoenix
has built up a dataset of curated genetic information, the most atomic
unit of which is the annotation. At a high level, annotations link
specific genes to specific ontological terms. Ontological terms (from
here on referred to as GO terms, or Gene Ontology terms) are the tool
through which all genes (through annotations) are identified to either
the location within the cell, a specific molecular function, or a specific biological process.

With all of this raw information being curated and updated every week,
Phoenix needs to be able to expose it all to researchers in a way that
supports querying for and analyzing relevant information. At a high level,
all of this boils down to the ability to query for annotations (and through
them, gene products and genes) that match some potentially complex filter
(slim the Ontology to a much smaller subset of relevant terms, bin by
specific GO terms, pick preset slim and additional bins, filter by specific
evidence codes and/or method, etc). With this capability, researchers will
be able to perform both of the core tasks identified above: find research
relevant to their area of research (by filtering for relevant GO terms),
and identifying understudied areas of the genome by filtering by evidence
code *ND*, for no data available.

## Timesheet

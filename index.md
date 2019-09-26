# Project Synopsis

The team at Phoenix Bioinformatics provides services for the scientific
community by providing a curated dataset of information about the
Arabidopsis Thaliana genome. In order to provide these services, Phoenix
has built up a dataset of curated genetic information, the most atomic
unit of which is the annotation. At a high level, annotations link
specific genes to specific ontological terms. Ontological terms (from
here on referred to as GO terms, or Gene Ontology terms) are the tool
through which all genes (through annotations) are identified to either
the location within the cell, a specific molecular function, or a
specific biological process.

With all of this raw information being curated and updated every week,
Phoenix needs to be able to expose it all to researchers in a way that
supports exposing and querying for relevant information. At a high
level, all of this boils down to the ability to query for annotations
(and through them, gene products and genes) that match some potentially
complex filter (slim the Ontology to a much smaller subset of relevant
terms, bin by specific GO terms, pick preset slim and additional bins,
filter by specific evidence codes and/or method, etc). With this
capability, researchers will be able to perform both of the core tasks
identified above: find research relevant to their area of research (by
filtering for relevant GO terms), and identifying understudied areas of
the genome by filtering by evidence code ND, for no data available.

# Team Information

* Nick Mosher ([nicholastmosher@gmail.com])
  * Team Coordinator: In charge of managing the team's
    development process (Scrum) and ensuring that work
    is being accomplished in a timely manner.
  * Backend developer/Interface designer: Responsible for
    helping to implement the backend service as well as
    defining a specification for API endpoints to make the
    frontend and backend integrate smoothly.
* Chike Udenze ([chikeudenze@gmail.com])
  * Website Coordinator: In charge of posting status updates
    and non-code deliverables to the project website.
  * Backend developer/Data engineer: Repsonsible for
    implementing endpoints and data processing required to
    serve user requests made from the frontend, as well as
    designing database entities for storing and querying
    necessary data.
* Joseph Shearer ([jas8425@rit.edu])
  * Sponsor Communicator: In charge of being the primary
    point of contact for engaging with the project sponsor.
  * Frontend Lead: In charge of designing an intuitive user
    interface and leading its implementation.
* Tim Geary ([tdg9336@rit.edu])
  * Meeting Scribe: In charge of capturing important decisions
    made and topics discussed during team meetings.
  * QA Expert: In charge of designing testable acceptance
    criteria as well as regression tests to ensure the product
    always builds and functions as expected.

[nicholastmosher@gmail.com]: mailto:nicholastmosher@gmail.com
[chikeudenze@gmail.com]: mailto: chikeudenze@gmail.com
[jas8425@rit.edu]: mailto: jas8425@rit.edu
[tdg9336@rit.edu]: mailto: tdg9336@rit.edu

# Table of Contents

* Weekly Updates:
  * [Week 2]\: Time tracking and project organization
  * [Week 3]\: Project synopsis and development process
  * [Week 4]\: Project plan and domain model

[Week 2]: ./week2.md
[Week 3]: ./week3.md
[Week 4]: ./week4.md

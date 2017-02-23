# GOV.UK PaaS Team Manual

This project uses [MkDocs][]. It is automatically built and hosted by [Read
the Docs][] at the following URL:

- https://government-paas-team-manual.readthedocs.io/

[MkDocs]: http://www.mkdocs.org/
[Read the Docs]: https://readthedocs.org/

## Setup

You need the following things installed:
- pip
- libjpeg  (libjpeg-dev on ubuntu/Debian)

It is recommended that you use [virtualenv][] if you want to run the build
process locally.

[virtualenv]: https://virtualenv.pypa.io/en/latest/

To install the dependencies:

    pip install -Ur requirements.txt

## Preview

To preview your changes locally run:

    mkdocs serve

Then visit:

- http://127.0.0.1:8000

## Diagrams

Diagrams are generated by
[blockdiag](http://blockdiag.com/en/blockdiag/index.html) from `.diag` source
files in `diagrams/`.

To regenerate the diagrams:
- run `make` from the root directory
- preview the diagram
- commit the changes to the SVG file

If you've added a new diagram, you'll need to edit `diagrams/Makefile`.
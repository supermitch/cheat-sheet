Cheat-sheet
===========

Code snippets, handy examples, links, quotes and more.

---

## Bash Cheats

### Text Search

Recusive case insensitive text search of a certain file type only: ::

    find . "*.py" -exec grep -Hin "rph" {} \;

where:

    `-Hin` prints matched names, case insensitive, showing line numbers

Clearer, and faster?

    find . "*.py" -print0 | xargs -0 grep -in "rph"

where:

    `-print0` and `-0` are required to handle spaces in filenames.



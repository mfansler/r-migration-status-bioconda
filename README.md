## Tracking Bioconda dependencies in Conda Forge R migrations
This repository provides a GitHub workflow to run
[the Bioconda script from @aliciaaevans](https://github.com/bioconda/bioconda-recipes/blob/43b74f3753c37ec8bb4cb7b90d195a64b1025447/scripts/bioconductor/missingCranPackages.py)
that checks the migration status of Conda Forge R feedstocks that are dependencies of Bioconda packages.

Running the workflow will check against the migration set by `MIGRATION_ID` (currently **r_base45**)
and save the output under the corresponding migration folder using the date of the run for a file name.

The workflow is currently configured to be triggered manually.

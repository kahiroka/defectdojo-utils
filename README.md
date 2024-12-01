# defectdojo-utils

DefectDojo Utilities

# Prerequisite

    $ pip install defectdojo-utils-kahiroka

Then, setup environment variables. Please refer to [dot_env_sample](dot_env_sample).

# Usage

## Export Nessus scan

    $ defectdojo-utils --list-nessus
    44: example.com
    $ defectdojo-utils --export-nessus 44 -o sample.nessus

Note: Nessus REST API only supports list and download.

## Import the scan to DefectDojo

    $ defectdojo-utils --list-defectdojo
    3: example.com
    $ defectdojo-utils --import-defectdojo example.com -i sample.nessus

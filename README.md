csv2json
========

`csv2json` is simple wrapper script around the Python standard library `csv` and
`json` modules for converting CSV formatted data to JSON.

Synopsis
--------
    csv2json [OPTION...] [FILE]

Description
-----------

The `csv2json` script reads CSV formatted data and outputs it into an JSON array
of objects. The values in the first row of the CSV data will be used as
fieldnames.

Options
-------

Mandatory arguments for long options are mandatory for short options too

      -o, --outfile=OUTFILE  write output to OUTFILE
      -h, --help             show this help message and exit

Examples
--------
    csv2json < in.csv > out.json
    csv2json -o out.json in.csv

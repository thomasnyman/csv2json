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
of objects. By default the values in the first row of the CSV data will be used
as fieldnames.

Options
-------

Mandatory arguments for long options are mandatory for short options too

      -o, --outfile=OUTFILE        write output to OUTFILE
      -h, --help                   show this help message and exit
      -f, --fieldnames FIELDNAMES  comma separated list of field names, if omitted the
                                   first row of FILE will be used as fieldnames
      -i, --indent INDENT          integer specifying indent level for pretty-printing,
                                   if zero or negative only newlines will be inserted
      -e, --encoding ENCODING      use specified ENCODING [default UTF-8]

Examples
--------
    csv2json < in.csv > out.json
    csv2json -o out.json in.csv

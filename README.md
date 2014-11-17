blast_parser.py
============

Takes a .xml formatted BLAST results file as input and prints the query ID, hit ID, percentage identity, query length, alignment length and e value for sequences passing the thresholds passed via the command line arguments.

### Dependencies

Requires [Biopython](http://biopython.org) for parsing of BLAST .xml files.

### Usage

```bash
python blast_parser.py -i <results.xml> -e 1e-20 -p 97 -a 100 > parsed_results.txt
```

> ##### Arguments

> `-i` The BLAST results file (in .xml format) that you want to parse.

> `-e` e value threshold. Can be a float or integer value.

> `-p` Percentage identity cutoff. Can be a float or integer value between 0 and 100.

> `-a` Minimum alignment length cutoff. Can be a float or integer value.

> `-h` Displays help.

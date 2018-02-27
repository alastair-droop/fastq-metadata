# Extract Statistics from FASTQ File Headers

The `fastq-metadata` script allows basic statistics to be extracted from the headers of a set of `fastq` files. The script will process either `fastq` or `fastq.gz` files.

**NB: The script is basic; it will only analyse the first header.** 

## Usage

~~~
usage: fastq-metadata [-h] [-v] [-n] [-s] [-f {none,cassava18,cassava18full}]
                      [-c]
                      <filename> [<filename> ...]

Summarize Illumina FASTQ read header metadata based on the first read header

positional arguments:
  <filename>            FASTQ file(s) to process

optional arguments:
  -h, --help            show this help message and exit
  -v, --version         show program's version number and exit
  -n, --no-header       suppress column headers
  -s, --suppress-mismatch
                        suppress data for mismatching files
  -f {none,cassava18,cassava18full}, --format {none,cassava18,cassava18full}
                        the FASTQ header format
  -c, --csv             output data as CSV (ignores -n)
~~~

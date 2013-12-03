PDFjam-GS
=========

**pdfjamgs** is a shell script you can use to extract
pages from one or more PDFs and write them to a new
PDF file. It is a replacement for the script
[pdfjam by David Firth](http://www2.warwick.ac.uk/fac/sci/statistics/staff/academic-research/firth/software/pdfjam)
which uses Ghostscript instead of Latex as its pdf engine.

It doesn't support all of the features of the original though.

```
Usage: pdfjamgs [-iovhdp]

Available options:
-v                   Print script version.
-h                   Print the help text.
-d                   Enable debug output.
-i <file:pages>      Specify the input file and the pages to extract.
                     The pages must be specified as a comma separated
                     list of numbers, ranges are supported as well.
                     Examples:
                     -i foo.pdf:1,3,4  extract page 1, 3 and 4.
                     -i foo.pdf:2-6,9  extract page 2 to 6 and page 9.
                     The option -i can be specified multiple times.
-o <file>            Specify the output file. This parameter is
                     optional. If you omit it, the extracted pages
                     will be written to the current directory as
                     separate pdf files.
-p                   Print the number of pages of the input file.

```

Licensed under the GPLv3.

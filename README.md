## Description

Small helper script in python to determine the source (original strand or reverse complementary strand) of a read pair R1 and R2
obtained from a non-directional TWGBS protocol. For this R1 and R2 reads are eventually swapped based on comparing T/C and A/G ratios between R1 and R2
in an alignment-free way.

## Script execution

To execute the python script Python 2.7 is required. The script requires to specify R1 and R2 fastq files (gzip or fastq are both accepted) as well as
the output fastq files for R1 and R2 (gzip or fastq) and fastq filenames for the unassgined R1 and R2 reads.

```
./TWGBS_read_pair_reconstruction.py -h
usage: TWGBS_read_pair_reconstruction.py [-h] --R1_in R1_IN --R2_in R2_IN
                                         [--input_ascii] --R1_out R1_OUT
                                         --R2_out R2_OUT --R1_unassigned
                                         R1_UNASSIGNED --R2_unassigned
                                         R2_UNASSIGNED [--output_ascii]
                                         [--log LOG] [--debug]

Alignment-free program to reconstruct correct R1-R2 reads relation from T/C
and A/G base ratio in TWGBS data.

optional arguments:
  -h, --help            show this help message and exit
  --R1_in R1_IN         R1 input file
  --R2_in R2_IN         R2 input file
  --input_ascii         Set if input fastq files are *not* compressed
  --R1_out R1_OUT       R1 output file
  --R2_out R2_OUT       R2 output file
  --R1_unassigned R1_UNASSIGNED
                        Filename R1 for unassigned read pairs
  --R2_unassigned R2_UNASSIGNED
                        Filename R2 for unassigned read pairs
  --output_ascii        Set if output fastq files should be *not* compressed
  --log LOG             Write basic statistics to this file
  --debug               Debug and write more output to console
```

## License

Copyright (c) 2019 German Cancer Research Center

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

## Contact

Charles Imbusch <c.imbusch@dkfz.de>

## Last change

14-02-19

# TWGBS

## Description

## Script execution

./WGBS_read_pair_reconstruction.py -h
usage: WGBS_read_pair_reconstruction.py [-h] --R1_in R1_IN --R2_in R2_IN
                                        [--gzip_input] --R1_out R1_OUT
                                        --R2_out R2_OUT --R1_unassigned
                                        R1_UNASSIGNED --R2_unassigned
                                        R2_UNASSIGNED [--gzip_output]
                                        [--log LOG] [--debug]

Alignment-free program to reconstruct correct R1-R2 reads relation from T/C
and A/G base ratio in TWGBS data.

optional arguments:
  -h, --help            show this help message and exit
  --R1_in R1_IN         R1 input file
  --R2_in R2_IN         R2 input file
  --gzip_input          Set if input fastq files are compressed
  --R1_out R1_OUT       R1 output file
  --R2_out R2_OUT       R2 output file
  --R1_unassigned R1_UNASSIGNED
                        Filename R1 for unassigned read pairs
  --R2_unassigned R2_UNASSIGNED
                        Filename R2 for unassigned read pairs
  --gzip_output         Set if output fastq files should be compressed
  --log LOG             Write basic statistics to this file
  --debug               Debug and write more output to console

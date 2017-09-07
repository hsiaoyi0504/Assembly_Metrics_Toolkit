## Assembly Metrics Toolkit

### Dependencies:
 * Perl
 * Python 3.5

### Usage:
```
usage: python3.5 assembly_metrics_toolkit.py [-h] [-o output_path] scaffolds_file [contigs_file]

Calculate various assembly metrics

positional arguments:
  scaffolds_file  a fasta file of scaffolds (can be .gz)
  contigs_file    a fasta file of contigs (can be .gz)

optional arguments:
  -h, --help      show this help message and exit
  -o output_path  where a JSON output file will be generated at
```

### Example Output:

Example output messages can be found in [example_output_scaffolds_only.txt](example_output_scaffolds_only.txt) and [example_output_scaffolds_and_contigs.txt](example_output_scaffolds_and_contigs.txt). These two examples are generated by used `python3.5 ./assembly_metrics_toolkit.py ./sample_data/BCM-After-Atlas/Scaffolds/Clec_Bbug02212013.genome.fa.gz` and `python3.5 ./assembly_metrics_toolkit.py ./sample_data/BCM-After-Atlas/Scaffolds/Clec_Bbug02212013.genome.fa.gz ./sample_data/BCM-After-Atlas/Contigs/Clec_Bbug02212013.contigs.fa.gz`, repectively. Those data can be found in [here](https://i5k.nal.usda.gov/data/Arthropoda/cimlec-%28Cimex_lectularius%29/Current%20Genome%20Assembly/1.Genome%20Assembly/BCM-After-Atlas/). The generated json file is similar to those output examples, and can be found in [example_scaffolds_only.json](example_scaffolds_only.json) and [example_scaffolds_and_contigs.json](example_scaffolds_and_contigs.json).

### Acknowledgement:
 * `assemblathon_stats.pl` and `FAlite.pm` are from [ucdavis-bioinformatics/assemblathon2-analysis](https://github.com/ucdavis-bioinformatics/assemblathon2-analysis) GitHub Repo.
 * `asm2stats.minmaxgc.pl` is from [rjchallis/assembly-stats](https://github.com/rjchallis/assembly-stats) GitHub Repo, and is modified to also support `.gz` input fasta file.

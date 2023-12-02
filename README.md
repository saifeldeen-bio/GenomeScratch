# GenomeScratch
GenomeScratch is a user-friendly tool designed for effortlessly generating virtual reference genomes, accompanied by GFF and GTF files. 
Tailored for testing workflows and training purposes, it enables users to simulate genomic scenarios and optimize bioinformatics processes in a controlled, lightweight environment. 
This tool is especially valuable when high-performance computing resources are scarce, allowing researchers to refine their methodologies efficiently before transitioning to real data. Whether for educational use or practical testing, GenomeScratch provides a convenient solution for genomics and bioinformatics applications.

**Usage:**

```
genomescratch -h [manual] -l <nline> -d/-r <DNA/RNA> -n <fileName> -o <outDir> [optional: -t/-f <GTF/GFF> -ng <nGenes> -gl <geneLength>]
```

**Parameters:**
- `<nline>`: Choose the desired number of sequence lines, each line containing 60 nucleotides.
- `<DNA/RNA>`: Specify the sequence type (DNA or RNA).
- `<fileName>`: Provide a name for the output files.
- `<outDir>`: Specify the output directory for the virtual sequences.

**Optional Parameters:**
- `-t/--GTF -f/--GFF`: Choose either GTF or GFF format for the output (default: none).
- `-ng/--nGenes`: Specify the number of genes (mandatory if using the -t option).
- `-gl/--geneLength`: Specify the length of the genes (default: 500).

**Options:**
- `-l/--nline`: Specify the number of sequence lines (nucleotides) for each line.
- `-d/--DNA -r/--RNA`: Choose between DNA and RNA as the sequence type.
- `-n/--name`: Specify the name for the output files.
- `-o/--out`: Specify the output directory for the virtual sequences.

**Example Usage:**
```bash
genomescratch -l 100 -d -n myGenome -o output_directory -t -ng 50 -gl 800
```

**Authorship:**
© Saifeldeen M. Ibrahim 2023

This software provides a convenient solution for genomics and bioinformatics applications, offering a controlled and efficient environment for testing and training purposes. Researchers can utilize GenomeScratch to simulate various genomic scenarios and optimize their workflows before applying them to real data.

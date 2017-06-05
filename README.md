# Select-Markers-Examples-file
# Example files for pipeline used in "Targeted NGS for species level phylogenomics: “made to measure” or “one size fits all”? (Kadlec, M., Bellstedt, D. U., Le Maitre, N. C., and Pirie, M. D. (2017). Peer J Prepr. doi:10.7287/peerj.preprints.2763v1.)

# AllMarker.py

# Input Files : 
  # Transcriptomes files available in Input files branch (When running AllMarker.pu, all transcriptomes must be in the same directory named Transcriptome.
  # Genome : WGS.fasta (in Input files branch)

# Commandline used : ./AllMarkers.py -NbT 3 -np 3 -l 1000 Transcriptome WGS.fasta nucl

# BestMarkers.py (Used complete path with input files)

# Input Files :
   # Blast File : Transcriptome4_SelectedSeq.fastavsDBWGS.fasta.xml (Output file of AllMarkers.py that can be found in BlastWGS directory.)
   # Sequences Files : Transcriptome4 (Output file of AllMarkers.py than can be found in Final_AllSelectedSequences directory)
   
# Commandline used : ./BestMarkers.py -l 1200 -intron? Y -Blast_file Transcriptome4_SelectedSeq.fastavsDBWGS.fasta.xml -Length_intron 200 -Number_baits 6000 -Length_baits 120 Transcriptome4

# Biopython
DNA Sequence Analysis
import Bio
from Bio.Seq import Seq 


print(Bio.__version__)

dna = Seq("ATGCGT")
print(dna)

print(dna.complement())

rna = dna. transcribe()  #Transcription of DNA

print(rna)

protein = rna.translate()  # Translation of RNA
print (protein) 

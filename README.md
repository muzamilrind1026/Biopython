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

#SeqRecord

from Bio.Seq import Seq 
from Bio.SeqRecord import SeqRecord

dna = Seq("ATGCGT")

record = SeqRecord(

    dna,

    id = "12345",

    name = "MMS",

description = "This is a test record",

)
print(record.id)
print(record.name)
print(record.description)


protien_Seq = Seq("ATGCGT")
protien_record = SeqRecord(
protien_Seq,

id = "Prot1",

name = "Test Protien",

description = "Sample Protien",


)
print(protien_record.id)
print(protien_record.name)
print(protien_record.description)



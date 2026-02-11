# Running Exomiser with a Phenopacket

We created a phenopacket for Pfeiffer syndrome in the [Phenoboard module](../phenopackets/phenoboard.md). We will now use this to run Exomiser.


java -jar exomiser-cli-14.0.0.jar --sample path/to/phenopacket.json --vcf path/to/genome.vcf --assembly hg38

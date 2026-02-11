# ▶️ Running Exomiser with a Phenopacket

In the previous step, we created a phenopacket for **Pfeiffer syndrome** using the  
[Phenoboard module](../phenopackets/phenoboard.md).  
We will now use this phenopacket as input for an Exomiser analysis.

## 🚀 Execute Exomiser

Run the following command from your terminal:

```bash
java -jar exomiser-cli-14.1.0.jar \
  --sample path/to/phenopacket.json \
  --vcf path/to/genome.vcf \
  --assembly hg19
```


This should run for about 15 seconds and then produce an HTML output file. 



!!! note "Interpreting Exomiser output"

    We will discuss how to evaluate the results in detail during the workshop. 
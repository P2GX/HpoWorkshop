# ▶️ Running Exomiser with a Phenopacket

In the previous step, we created a phenopacket for **Pfeiffer syndrome** using the  
[Phenoboard module](../phenopackets/phenoboard.md).  
We will now use this phenopacket as input for an Exomiser analysis.

## 🚀 Execute Exomiser

Run the following command from your terminal:

```bash
java -jar exomiser-cli-14.1.0.jar \
  --sample phenopacket.json \
  --vcf  examples/Pfeiffer.vcf \
  --assembly hg19
```

In this command, 

- `phenopacket.json` is the phenopacket we made with Phenoboard (adjust the path/filename if needed)
- `examples/Pfeiffer.vcf` is an example Variant Call Format (VCF) file provided by the Exomiser distribution.

This should run for about 15 seconds and then produce an HTML output file. 



!!! note "Interpreting Exomiser output"

    We will discuss how to evaluate the results in detail during the workshop. 
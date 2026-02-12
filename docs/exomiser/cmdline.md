# 🧬 Running Exomiser from the Command Line

!!! abstract "Goal"
    In this section we will install and run **Exomiser CLI** using the  
    Phenopacket generated with **Phenoboard**.

---

## ⚙️ Installation

Download the latest Exomiser distribution from:

👉 https://data.monarchinitiative.org/exomiser/latest/

At the time of writing, the file is:

```
exomiser-cli-14.0.0-distribution.zip
```

### Required Data Files

You will also need:

- Phenotype data — e.g. `2406_phenotype.zip`
- Variant data — choose **hg19** or **hg38**

!!! tip "Workshop setup"
    For this workshop we will use the **HG37** dataset because our example VCF file was made with this assembly.

---

## ⬇️ Download with `wget`

Create a project directory and download the files:

```bash
wget https://data.monarchinitiative.org/exomiser/latest/exomiser-cli-14.0.0-distribution.zip

# Download datasets (⚠️ ~40 GB total — this may take a long time!)
wget https://data.monarchinitiative.org/exomiser/latest/2402_hg19.zip
wget https://data.monarchinitiative.org/exomiser/latest/2402_phenotype.zip
```

!!! warning "Large download"
    The variant dataset is very large (~80 GB).  
    Ensure you have sufficient disk space and a stable internet connection.

---

## 📦 Unpack the Files

Unzip the distribution and data archives:

```bash
unzip exomiser-cli-14.0.0-distribution.zip
unzip 2402_*.zip -d exomiser-cli-14.0.0/data
```

This creates a directory named:

```
exomiser-cli-14.0.0/
```

---

## 📁 Expected Directory Structure

After extraction, your directory should look similar to this:

```text
exomiser-cli-14.0.0/
├── CHANGELOG.md
├── LICENCE.txt
├── README.md
├── application.properties
├── examples
│   ├── Pfeiffer.vcf
│   ├── Pfeiffer.vcf.gz
│   ├── Pfeiffer.vcf.gz.tbi
│   ├── exome-analysis.yml
│   └── (...)
├── exomiser-cli-14.1.0.jar
├── lib
│   ├── HikariCP-5.0.1.jar
│   ├── (...)
│   └── xz-1.8.jar
├── pr2.json
└── results
    ├── bwa_mem2.gatk4_hc_gvcf.0037X64-N1-DNA1-WGS1-exomiser.html
    └── (...)
``` 


If everything has gone well, we can now run the softwre

```bash
java -Xmx4g -jar exomiser-cli-14.1.0.jar
usage: java -jar exomiser-cli-{build.version}.jar [...]
    --analysis <file>            Path to analysis script file. This should
                                 be in yaml format.
    (...)
```



**Next Module:** [Java](java.md){ .md-button .md-button--primary }
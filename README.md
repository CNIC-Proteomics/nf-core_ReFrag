# nf-SearchEngine


# Usage
In production (Docker):
```
cd /opt/PTM-compass

nextflow \
    -log "/var/log/nextflow/nextflow.log" \
    run main.nf   \
        -profile singularity \
        --params_msf "/mnt/tierra/PTM-compass/params/SHIFTS.ini" \
        --input_files "/mnt/tierra/PTM-compass/tests/test1/Recom/JM_HuMarfanPlasma_TMT[0-9].txt" \
        --outdir  "/mnt/tierra/PTM-compass/tests/test1" \
        -resume
```


Debugging using Ubuntu (WSL):
```
cd /home/jmrodriguezc/projects/nf-ReFrag

nextflow \
    -log "/var/log/nextflow/nextflow.log" \
    run main.nf   \
        -profile singularity \
        --params_msf "/home/jmrodriguezc/projects/nf-ReFrag/tests/test1/params/closed_fragger.params" \
        --input_files "/home/jmrodriguezc/projects/nf-ReFrag/tests/test1/raws/*.raw" \
        --outdir  "/home/jmrodriguezc/projects/nf-ReFrag/tests/test1" \
        -resume

```

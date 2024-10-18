The standard notation of teloscope is:
``` 
teloscope -f input.[fasta][.gz] -o [output/dir] -c [canonical] -p [pattern1,pattern2,pattern3] -w [window size] -s [step size] -k
```

Let's begin by looking at the options of teloscope:
```
teloscope -h
```

1. Let's evaluate the telomere contents of the fasta file:
```
time teloscope -f path/GCF_000002985.6_WBcel235_genomic.fna  -o path/ -j 4 -w 200 -s 100 -c TTAGGC -p TKWGGC -d 24 -l 36 -k

```

2. Now let's evaluate the telomere contents of the fasta file:
```
time teloscope -f path/GCF_000002985.6_WBcel235_genomic.fna  -o path/ -j 4 -w 200 -s 100 -c TTAGGC -p TKWGGC -d 24 -l 36 -k

```

3. Now let's evaluate the telomere contents of the fasta file:
```
time teloscope -f path/GCF_000002985.6_WBcel235_genomic.fna  -o path/ -j 4 -w 200 -s 100 -c TTAGGC -p TKWGGC -d 24 -l 36 -k

```

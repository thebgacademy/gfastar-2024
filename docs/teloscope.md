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
mkdir c.elegans/
teloscope -f GCF_000002985.6_WBcel235_genomic.fna  -o c.elegans/ -j 4 -w 200 -s 100 -c TTAGGC -p TKWGGC -d 24 -l 36 -k --verbose

```

2. Now let's evaluate the telomere contents of the fasta file:
```
mkdir gorilla/
teloscope -f mGorGor1.pat.cur.20231122.fasta.gz  -o gorilla/ -j 4 -w 1000 -s 500 -c TTAGGG -p TTAGGG,TCAGGG,TGAGGG,TTGGGG,CTAGGG,GTAGGG,TCCGGG,TTCGGG,TCGGGG -d 50 -l 1000 

```

3. Now let's evaluate the telomere contents of the fasta file:
```
mkdir bonobo/
teloscope -f mPanPan1.mat.cur.20231122.fasta.gz  -o bonobo/ -j 4 -w 1000 -s 500 -c TTAGGG -p TTAGGG,TCAGGG,TGAGGG,TTGGGG,CTAGGG,GTAGGG,TCCGGG,TTCGGG,TCGGGG -d 50 -l 1000 

```

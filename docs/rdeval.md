The standard notation of rdeval is:
``` 
rdeval input.[fasta|fastq|gfa][.gz] [expected genome size]
```

Let's begin by looking at the options of redeval:
```
rdeval -h
```

Now let's evaluate the contents of our fasta file:
```
rdeval random1.fasta
```

And filter sequences with a length greater than 10:
```
rdeval random1.fasta -f ">10"
```

Let's get an "ultralong" dataset. First check your input:
```
rdeval filtered.fastq
```

Then filter for >10000bp:
```
rdeval filtered.fastq -f ">10000" -o filtered_ul.fastq
```

We can also get the individual sizes for post-processing, e.g. as a histogram:
```
rdeval -r random1.fasta --out-size h
```

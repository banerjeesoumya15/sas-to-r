## To save a dataset
### SAS code
```SAS
/* define paths */
libname libout "/path/to/output/";
libname libin "/path/to/input/";

data libout.outdata;
  set libin.indata;   /* read input data */
 run;
 ```
 ### R code
 ```r
 # read input data
 load(file="/path/to/input/indata.RData")
 
 # write to output
 save(indata, file="/path/to/output/outdata.RData")
 ```

## Short patch example

In this example two files are compared with each other with the diff command.
The difference between those two files will be written into a Patch.

### File1
```sh
Andreas
Max
Jan
Hans
Klaus
```

### File1
```sh
Andreas
Max2
Jan
Hans2
Klaus
```


### Creating the patch
```sh

#difference between the files
$diff file1 file2    

# take a look at man diff for -Naur
$diff -Naur File1 File2 > patch.txt  
```


### Patching the file
It will allways patch the first file from the diff command

```sh
$patch < patch.txt
```

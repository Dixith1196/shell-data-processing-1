# shell-data-processing
 
 ## Powershell Commands:
```Powershell
 mkdir - Used to create a new directories.
 cd - Used to chnage the current woking directory.
 ni - Used to create a new item.
 ls- Used to list the files and directories within the file system.

```
## Curl data:

```Powershell
curl "yourlongurl" -O 
```
- This is the curl command I used to get my data.
```Powershell 
curl "http://shakespeare.mit.edu/romeo_juliet/full.html" -O "data.txt"

## Bash Commands:

- Transform each space ' ' into a return character '\12'
```Powershell
tr ' ' '\12' < returnedfile
```
- Pipe the output to sort
```Powershell
tr ' ' '\12' < returnedfile | sort
```
- Pipe the sorted output to uniq -c to count
```Powershell
tr ' ' '\12' < returnedfile | sort | uniq -c
```
- Pipe the reduced output to sort with -nr flag
```Powershell
tr ' ' '\12' < returnedfile | sort | uniq -c | sort -nr
```
- Redirect the output to result.txt
```Powershell
tr ' ' '\12' < returnedfile | sort | uniq -c | sort -nr > result.txt
```

- The bash up arrow will return the previous command.
- -n flag means --numeric-sort. Compares according to string numerical value.
- -r means --reverse. Reverses the result of comparisons.
- For a single letter flag we will use a single dash(-) and if it has more than one letter then we use (--).




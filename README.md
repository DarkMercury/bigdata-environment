# BigData environment

Stuff for labs and assignment for Big Data class at Poly. 

## Credentials

User: bigdata
Pass: bigdata

# Starting hadoop

Scripts are made to ease starting and stopping of nodes. Open terminal and run
the following commands

```
hstart
```

Starts the hadoop nodes

```
hstop
```

Stops hadoop nodes

# Wordcount

```
String[] otherArgs =new String[]{"input","output"};
```

The line in `wordcount.java` sample file. (line 53). Change `input` and
`output` into the files for input and output inside hadoop file system. To add
files,

```
hdfs dfs -put <file> <optional dir> 
```

Without `<optional dir>`, the file will be added on the root inside
`/user/bigdata/`

# Troubleshooting

## File exists error

In eclipse, check left side and open the folder in 'DFS Locations/MapRed
Location/user/bigdata` and delete
the file output i.e. `wr_output`

# Hadoop Map-Reduce Project

## Steps for executing the project:

### I. Conversion of Directed Graph into Undirected graph

1. Download the project zip file 'mapreduce_project.zip' and extract it using unzip command:- unzip mapreduce_project.zip
2. Navigate to the folder ‘conversion’ inside extracted folder using cd command:- cd conversion
3. Compile the java code using the command:- com.sun.tools.javac.Main adjList.java
4. Build jar file using the command:- jar cvf adjList.jar *.class
5. Run the jar file built in previous step using the command:- hadoop jar adjList.jar adjList <(INPUT) path to directed graph file> <(OUTPUT) path to store undirected graph file>
6. This will generate output file having converted directed graph into undirected graph.

### Sample output:

99999	77307
99999	86254
99999	68982
99999	68987
99999	86256
99999	77309
99999	77300


### II. Finding connectivity and maximum adjacency list for directed graph
1. Download the project zip file 'mapreduce_project.zip' and extract it using unzip command:- unzip mapreduce_project.zip
2. Navigate to the folder ‘directed’ inside extracted folder using cd command:- cd directed
3. Compile the java code using the command:- com.sun.tools.javac.Main adjList.java
4. Build jar file using the command:- jar cvf adjList.jar *.class
5. Run the jar file built in previous step using the command:- hadoop jar adjList.jar adjList <(INPUT) path to directed graph file> <(OUTPUT) path to store result file> 

### Sample output:
Node 611459 having Minimum Connectivity of 1
Node 292640 having Maximum Connectivity of 249
Node 292640 having longest adj list of 292832,292833,292844,292843,292842,292841,292840,292839,292838,292864,292865,292866,292867,292868,292869,292870,292871,292872,292718,292837,292836,292835,292846,292847,292848,292849,292845,272919,284306,292641,292642,292643,292644,292645,292646,292647,292648,292649,292650,292651,292652,292653,292654,292655,292656,292657,292658,292659,292660,292661,292662,
*skipped* 
,292830,292851,292852,292834,299039,292886,292885,292884,292883,292882,292881,292880,292879,292878,292877,292876,292875,292874,292873,292853,292854,292855,292856,292857,292858,292859,292860,292861,292862,292863,292831
Executed on: 2019-11-16 03:13:58.109326
*********************************************************


### III. Finding connectivity and maximum adjacency list for undirected graph
1. Download the project zip file 'mapreduce_project.zip' and extract it using unzip command:- unzip mapreduce_project.zip
2. Navigate to the folder ‘undirected’ inside extracted folder using cd command:- cd undirected
3. Compile the java code using the command:- com.sun.tools.javac.Main adjList.java
4. Build jar file using the command:- jar cvf adjList.jar *.class
5. Run the jar file built in previous step using the command:- hadoop jar adjList.jar adjList <(INPUT) path to directed graph file> <(OUTPUT) path to store result file> 

### Sample output:
Node 600416 having Minimum Connectivity of 1
Node 438238 having Maximum Connectivity of 84290
Node 438238 having longest adj list of 375217,6152,28196,320712,28188,341295,341149,28225,341208,320718,16535,28177,4823,341214,339598,339590,28186,448192,64689,320713,341204,28194,16532,28176,341329,320717,28179,339599,28223,339597,4821,341145,28214,339593,28193,28197,320719,28198,340790,28185,341138,28216,16534,341091,28217,320716,36128,28178,324547,28189,341039,339596,450678,341119,341255,28203,
*skipped*
359856,35504,44791,323984,32828,6107,350237,17303,44796,333501,346956,44784,6108,22007,21948,32825,22042,6166,333500,323194,22004,6109,17306,333499,346957,6157,22037,333498,359848,32824,323195,22040,323814,6148,333497,17310,36289,6113,36247,36271,333496,32823,35800,336927
Executed on: 2019-11-16 04:21:47.989640
*********************************************************

input files
-------------
1. graph file
2. prior file
3. train file

Steps
---------
S1: g++ metric.cpp -O3 -o metric

S2: g++ sybilscar.cpp -pthread -O3 -o sybilscar

S3: ./sybilscar -graphfile Undirected_Facebook/graph.txt -trainfile Undirected_Facebook/train.txt -postfile Undirected_Facebook/post_SybilSCAR.txt -mIter 6 -tp 0.9 -tn 0.1 -wg 0 -wei 0.6 -nt 1 

S4: ./metric -testfile Undirected_Facebook/test.txt -postfile Undirected_Facebook/post_SybilSCAR.txt


NOTE: Try removing -O3 and try the above steps.
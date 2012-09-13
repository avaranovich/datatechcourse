Ideas for slides:
- Nonrelational Database Systems, Not-Only SQL or NoSQL?

Riak
http://www.slideshare.net/dreverri/riak-mapreduce

Hadoop
Configuration guide
http://www.michael-noll.com/tutorials/running-hadoop-on-ubuntu-linux-single-node-cluster/

Format log
user@nosql:/usr/local/hadoop$ /usr/local/hadoop/bin/hadoop namenode
-format
12/09/11 13:58:25 INFO namenode.NameNode: STARTUP_MSG: 
/************************************************************
STARTUP_MSG: Starting NameNode
STARTUP_MSG:   host = nosql/127.0.1.1
STARTUP_MSG:   args = [-format]
STARTUP_MSG:   version = 1.0.3
STARTUP_MSG:   build =
https://svn.apache.org/repos/asf/hadoop/common/branches/branch-1.0 -r
1335192; compiled by 'hortonfo' on Tue May  8 20:31:25 UTC 2012
************************************************************/
12/09/11 13:58:25 INFO util.GSet: VM type       = 64-bit
12/09/11 13:58:25 INFO util.GSet: 2% max memory = 19.33375 MB
12/09/11 13:58:25 INFO util.GSet: capacity      = 2^21 = 2097152
entries
12/09/11 13:58:25 INFO util.GSet: recommended=2097152, actual=2097152
12/09/11 13:58:25 INFO namenode.FSNamesystem: fsOwner=user
12/09/11 13:58:25 INFO namenode.FSNamesystem: supergroup=supergroup
12/09/11 13:58:26 INFO namenode.FSNamesystem: isPermissionEnabled=true
12/09/11 13:58:26 INFO namenode.FSNamesystem:
dfs.block.invalidate.limit=100
12/09/11 13:58:26 INFO namenode.FSNamesystem:
isAccessTokenEnabled=false accessKeyUpdateInterval=0 min(s),
accessTokenLifetime=0 min(s)
12/09/11 13:58:26 INFO namenode.NameNode: Caching file names occuring
more than 10 times 
12/09/11 13:58:26 INFO common.Storage: Image file of size 110 saved in
0 seconds.
12/09/11 13:58:26 INFO common.Storage: Storage directory
/app/hadoop/tmp/dfs/name has been successfully formatted.
12/09/11 13:58:26 INFO namenode.NameNode: SHUTDOWN_MSG: 
/************************************************************
SHUTDOWN_MSG: Shutting down NameNode at nosql/127.0.1.1
************************************************************/

copy files to DFS
user@nosql:/usr/local/hadoop/bin$ hadoop dfs -copyFromLocal
/tmp/gutenberg /user/gutenberg

show files in DFS
user@nosql:/usr/local/hadoop/bin$ hadoop dfs -ls /user/gutenberg

Admin urls
http://nosql.101companies.org:50030/
http://nosql.101companies.org:5070/

simple-yarn-app
===============

Simple YARN application to run n copies of a unix command - deliberately kept simple (with minimal error handling etc.)

Usage:
======
1.将jar包存入hdfs
$ bin/hadoop fs -copyFromLocal simple-yarn-app-1.1.0.jar /apps/simple/simple-yarn-app-1.1.0.jar

2.运行yarn应用
$ bin/hadoop jar simple-yarn-app-1.1.0.jar com.hortonworks.simpleyarnapp.Client /bin/date 2 /apps/simple/simple-yarn-app-1.1.0.jar
  
    

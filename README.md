# Apache-Spark-

Apache Spart fo data science with Python session at Scaler by Amit Singh 

Problem Statments - 
What was most popular movie/dish/series/match/story/book/video/stocks of 2022 like all that?
Which Movie has given highest IMDB rating on netflix OTT platform?
Which best comedy movie of 2022?

We can solve above problem with below technologies 
  -  Python(pandas)(20m cvs, 100m) Huge data we need to process in less time
  -  RDBMC (Oracle, MySQL, Postgess) - Work well when data in TB, but what if data is in PB and HB, It will give you RTO(Request Timeout)
  -  NoSQL (It help you to store huge size of data, but we need to process that data(like finding the rating or reviews, popularity), Good storage but not good comput)
  -  Exel (100000) it gives error when xls has 1L rows even for opening

To solve this they come with distributed programming ie distributed processing 
Multiple processing working together for common goal (2500 servers)


Solution A
All servers are connected each others we call it cluster 
we call that server nodes and they connected high bandwidth network 
Each server has its dedicated RAM, HARD DISK, CPU - which process executes some jobs or task

Challages for above approach 
1.  Maintanance (Network failure, Disk failed, CPU motherboard issue, RAM issue, overheating)
2.  Who will distribution, who will assign the task to difference task, who will scheduling, who will balance the load across all servers
3.  Network bandwidth

Doog cutting (Father of Hadoop) - 
Created framework HADOOP
    Monitoring
    Distribution 
    Output

Test 
100 TB sorted in 22 min only by 1000 servers cluster

Hadoop has 18 plus components 

We are going to focus one compnents ie map reduce 
Map Reduce - Was very popular
           - Legacy technology 
           - Accepted by yahoo
           - it used till 2009 
           - matai zomb find limitation of map reduce 
          
      file -> read that file in to memory(Mapping) -> Temp location in disk -> Reduce read it and write to another file location 
      here we have to read 2 time and write 2 times 
      Batch Processing  => last working day => csv file => cron jobs => banks read the cvs file(working days, bonus etc) => bank account credit => message notification
     
  distribution system has main critical point is 
  network bandwidth 
  read/write disk operations 
  
  
 realtime processing was not possible with the map reduce technology 
 answer to that issue is spark 
 
 He is introduced to world is spark
 Spark is nearly 50times faster than the map reduce, also sometime its reaches to 100time faster.
 
 What is archtecture doing that benifits 
 
 Spark is 
      - distributed falt talerance engine 
      - in-memory procesisng engine(it happens in map reduce- but intermedit disk operation, here is on read and one write operation)
      - in-memory operation happens on the each cluster node
    
Spark Architecture
  - Apache Spark Core
  - Spark SQL (Structure processing)
  - Spark Streaming (real time processing (AI))
  - ML Lib ()
  - Graphic (Graph processing, linkedn in connection graph structure)
  
  Spark Nothing but Processing Engine only 
  File, DB, S3 
  
  
 Driver program 
  - smpart context 
  - Main program 
  - Master
  - who will govern
  - where to job to be send
  - how to do schedulling 
  - Entry point 
 
Worker node, it has executor, it has task/job, 
   - JVM process - where SC will send the program to run
   -  

Cluster Manager
   - Pool of resource 


Here in spark we keep data at the worker node in HDFC, S3, files

in cloud software managed by spark and hardware managed by aws 

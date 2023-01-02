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
     
     
  distribution system has main critical point is 
  network bandwidth 
  read/write disk operations 
  
  

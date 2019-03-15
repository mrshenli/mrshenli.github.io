---
permalink: /
title: "About Me"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a research scientist at Facebook NYC. I received my Ph.D. degree in Computer Science from the University of Illinois Urbana-Champaign. I am broadly interested in distributed systems and backend technologies. 

Experiences
======
* 2018/11 - Present Research Scientist, **Facebook AI Research**.
* 2016/06 - 2018/11 Research Staff Member, **IBM Research** T. J. Watson Lab
* 2010/10 - 2016/05 Research Assitant, **University of Illinois Urbana-Champaign**
* 2015/05 - 2015/08 Research Intern, **IBM Research** T. J. Watson Lab
* 2014/05 - 2014/08 Research Intern, **IBM Research** T. J. Watson Lab
* 2013/06 - 2013/08 Software Engineer Intern, **Facebook** Inc.
* 2012/05 - 2012/08 Software Engineer Intern, **Yahoo!** Inc.



Projects
======
* **IBM Streams Beam Runner**

	IBM Streams is a high-throughput low-latency analytic platform for streaming data applications. I work on multiple research issues in IBM Streams, including transform graph translation and optimization, out-of-order event arrival processing, large window aggregation, etc. Currently, I lead a small team of four people to adopt Apache Beam model into IBM Streams, which involves filling in the model gaps between Beam and Streams, indexing/garbage-collecting Beam transform states, and managing operator parallelism. Our work produces both research papers and a product (IBM Streams Beam runner toolkit) deployed in IBM Cloud which won 2018 IBM Outstanding Technical Achievement Award. [[VLDB'18](http://www.vldb.org/pvldb/vol11/p1742-li.pdf)]

* **Stark: Optimizing In-Memory Computing for Dynamic Dataset Collections**

	In this project, we explored the possibility of combining in-memory computation frameworks with the backend of online services to answer massive user queries in real-time. Success along this path would push online services beyond the existing store-index-retrieve design pattern, allowing the backend to afford relatively complex data analytic algorithms to serve every user query with highly optimized results. This project tackles this problem by optimizing Apache Spark for online queries. [[ICDCS'17](https://ieeexplore.ieee.org/document/7979959)]

* **Pyro: A Spatial-Temporal Big-Data Storage System**

	In this project, we designed a spatial-temporal big-data storage system tailored for high-resolution geometry queries and dynamic workload hotspots. With the rapid growth of mobile devices and applications, geo-tagged data has become a significant workload for big data storage systems. In dealing with spatial-temporal big-data workloads, existing systems either fall short in scalability or fail to deliver high efficiency. This project attacks this problem by optimizing the HBase/HDFS stack for spatial-temporal data. [[ATC'15](https://www.usenix.org/system/files/conference/atc15/atc15-paper-li-shen.pdf)]

* **Real-time Scheduling for Map-Reduce Systems**

	This project, in collaboration with Yahoo!, introduces the marriage between real-time scheduling and Map-Reduce systems. Map-Reduce ecosystems have become dominant big data analytic solutions. Nevertheless, schedulers in the state-of-the-art Map-Reduce systems remain relatively simple, which often fails to utilize resources in large clusters efficiently. Based on the advances in the real-time community, we develop both systems and theories to improve Map-Reduce workflow scheduling by enabling the utilization-based schedulability analysis. [[RTAS'15](https://ieeexplore.ieee.org/document/7108416)][[ICDCS'14](WOHA: Deadline-Aware Map-Reduce Workflow Scheduling Framework over Hadoop Cluster)]

* **Energy Efficient Data Centers**

	This project is sponsored by NSF, and in collaboration with VMWare. In this project, we built a 107-server cluster in a server room equipped with 40 UPS devices, 12 temperature sensors, a remotely controllable Computer Room Air Conditioning (CRAC) unit, and 6 smart PDUs. On this cluster, we design and evaluate energy-aware systems for data center workloads. More specifically, I am working on the following problems: (1) Thermal-aware workload placement, which assigns workloads to different servers leveraging the uneven thermal distribution in the cluster. (2) Power proportional memory cache cluster, that delivers elasticity and handles transition penalty. (3) Data center power capping using energy storage systems. [[ICDCS'13](https://ieeexplore.ieee.org/document/6681577)][[ICDCS'12](https://ieeexplore.ieee.org/document/6258012)][[IGCC'11](https://ieeexplore.ieee.org/document/6008602)]

* **Apollo: A Data Distillation Service for Social Sensing**

	This project is one of the very few "Golden Nuggets" projects of the Network Science Collaborative Technology Alliance (NS-CTA), a collaborative research alliance between the US Army Research Laboratory (ARL) and other research organizations such as UIUC, CMU, and IBM Research. In this project, we propose Apollo, a new service for social sensing applications, which aims at distilling large amounts of noisy social sensory data into smaller amounts of more trustable information. Particularly, I am working on improving the scalability of the system, and at the same time preserving the Quality of Information (QoI). [[IPSN'14](https://dl.acm.org/citation.cfm?id=2602339.2602344)]

* **SmartRoad: A Crowd-Sourced Road Sensing System**

	This project is sponsored by NSF, Siebel Foundation, and in collaboration with Microsoft Research. In this project, we design and develop a vehicular smartphone testbed, called SmartRoad, which can automatically collect, transport, and analyze participatory sensing data for decision making. SmartRoad is currently running on 35 external participatory vehicles, and will soon be extended to a larger-scale (100-200 vehicles) deployment with the UIUC Facilities and Services Department. SmartRoad facilitates various research applications such as (1) GreenGPS: a navigation service providing the most fuel-efficient routes for vehicles between an arbitrary pair of end-points. (2) Providing energy efficient navigation service that takes advantage of phone's low-power MEMS sensors in place of GPS. [[ICCPS'17](https://ieeexplore.ieee.org/document/7945012)]


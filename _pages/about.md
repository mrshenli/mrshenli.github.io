---
permalink: /
title: "About Me"
excerpt: "About me"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

I serve as the tech lead for [PyTorch](https://pytorch.org/) Distributed team and work on all major features in the [distributed package](https://pytorch.org/tutorials/beginner/dist_overview.html), including [FullyShardedDataParallel](https://pytorch.org/blog/introducing-pytorch-fully-sharded-data-parallel-api/), [DistributedDataParallel](https://pytorch.org/docs/master/generated/torch.nn.parallel.DistributedDataParallel.html), [collective communication](https://pytorch.org/docs/stable/distributed.html), and [RPC-based distributed training](https://pytorch.org/docs/master/rpc.html). I am broadly interested in ML systems and large scale ML applications.

Experiences
======
* 2023/06 - Present Principal Research Scientist, **Meta MRS**.
* 2018/11 - 2023/05 Senior Staff Research Scientist, **Meta AI**.
* 2016/06 - 2018/11 Research Staff Member, **IBM Research** T. J. Watson Lab
* 2010/10 - 2016/05 Research Assitant, **University of Illinois Urbana-Champaign**
* 2015/05 - 2015/08 Research Intern, **IBM Research** T. J. Watson Lab
* 2014/05 - 2014/08 Research Intern, **IBM Research** T. J. Watson Lab
* 2013/06 - 2013/08 Software Engineer Intern, **Facebook** Inc.
* 2012/05 - 2012/08 Software Engineer Intern, **Yahoo!** Inc.



Projects
========

* **Large Language Model Training**

    This project optimized training efficiency with PyTorch native features for GPT models ranging from 162M to 1T parameters. We summarized the guidelines on using cloud resources and PyTorch features including DistributedDataParallel, Pipeline Parallel, FullyShardedDataParallel, Activation Checkpionting/Offloading, etc.

    * PyTorch Data Parallel Best Practices on Google Cloud [Joint [Post](https://medium.com/pytorch/pytorch-data-parallel-best-practices-on-google-cloud-6c8da2be180d) and [Talk](https://www.nvidia.com/en-us/on-demand/session/gtcspring22-s42584/) with GCP]
    * Training and Profiling Large Scale Models with PyTorch [[GTC'22 Talk](https://www.nvidia.com/en-us/on-demand/session/gtcspring22-s41986/)]
    * Training a 1 Trillion Parameter Model With PyTorch Fully Sharded Data Parallel on AWS [Joint [Post](https://medium.com/pytorch/training-a-1-trillion-parameter-model-with-pytorch-fully-sharded-data-parallel-on-aws-3ac13aa96cff) and [Talk](https://www.nvidia.com/en-us/on-demand/session/gtcspring22-s42556/) with AWS]

* **PyTorch FullyShardedDataParallel**

    This is the first native feature in PyTorch that can support models with up to trillions of parameters. FullyShardedDataParallel (FSDP) decomposes the model into smaller units. For every unit, FSDP shards Tensor storage across data-parallel processes to reduce memory footprint, `allgather`s full parameters before computation, and discards gathered parameter shards afterward. FSDP offers multiple performance optimizations out-of-box, including computation and communication overlap, parameter prefetching, parameter CPU offloading, and mixed-precision support in both computation and communication. [[VLDB'23](https://arxiv.org/pdf/2304.11277.pdf)][[Post](https://pytorch.org/blog/introducing-pytorch-fully-sharded-data-parallel-api/)][[Doc](https://pytorch.org/docs/stable/fsdp.html)][[Tutorial](https://pytorch.org/docs/stable/fsdp.html)]

* **Pipelined Data Parallel**

    We developed a pipelined data parallel training paradigm called PipeTransformer which leverages automated elastic pipelining for efficient distributed training of Transformer models. PipeTransformer can adaptively freeze model layers, shrink pipelines based on the number of active layers to free resources, and dynamically allocate those resources to increase data parallel width. [[ICML'21](https://arxiv.org/pdf/2102.03161.pdf)][[Post](https://pytorch.org/blog/pipetransformer-automated-elastic-pipelining/)]

* **PyTorch RPC**

    PyTorch RPC provides a flexible and high-performance set of low-level APIs for distributed deep learning. PyTorch RPC natively provides essential features for implementing training applications in a distributed environment, including optimized tensor communications, remote memory management, and distributed autograd. It allows users to easily implement different training paradigms (e.g., parameter servers, pipeline parallel, etc.) on top. [[GTC'21](https://www.nvidia.com/en-us/on-demand/session/gtcspring21-s31630/)][[DevDay'20](https://www.youtube.com/watch?v=bWqpf8ISk_c)][[Doc](https://pytorch.org/docs/stable/rpc.html)][[Tutorial](https://pytorch.org/tutorials/intermediate/rpc_tutorial.html)]

* **PyTorch DistributedDataParallel**

    DistributedDataParallel (DDP) helps to scale model training to large datasets and large clusters. It can be enabled on top of local training scripts with 1-line code change and will automatically overlap backward computation with gradient communication. This feature is widely adopted both internally at Meta and externally across the industry. [[VLDB'18](http://www.vldb.org/pvldb/vol13/p3005-li.pdf)][[Talk1](https://www.youtube.com/watch?v=3XUG7cjte2U)][[Talk2](https://www.bilibili.com/video/BV1MA411n7ef?p=134)][[Doc](https://pytorch.org/docs/stable/generated/torch.nn.parallel.DistributedDataParallel.html)][[Tutorial](https://pytorch.org/tutorials/intermediate/ddp_tutorial.html)]


* **IBM Streams Beam Runner**

	IBM Streams is a high-throughput low-latency analytic platform for streaming data applications. I work on multiple research issues in IBM Streams, including transform graph translation and optimization, out-of-order event arrival processing, large window aggregation, etc. Currently, I lead a small team of four people to adopt Apache Beam model into IBM Streams, which involves filling in the model gaps between Beam and Streams, indexing/garbage-collecting Beam transform states, and managing operator parallelism. Our work produces both research papers and a product (IBM Streams Beam runner toolkit) deployed in IBM Cloud which won 2018 IBM Outstanding Technical Achievement Award. [[VLDB'18](http://www.vldb.org/pvldb/vol11/p1742-li.pdf)]

* **Pyro: A Spatial-Temporal Big-Data Storage System**

	In this project, we designed a spatial-temporal big-data storage system tailored for high-resolution geometry queries and dynamic workload hotspots. With the rapid growth of mobile devices and applications, geo-tagged data has become a significant workload for big data storage systems. In dealing with spatial-temporal big-data workloads, existing systems either fall short in scalability or fail to deliver high efficiency. This project attacks this problem by optimizing the HBase/HDFS stack for spatial-temporal data. [[ATC'15](https://www.usenix.org/system/files/conference/atc15/atc15-paper-li-shen.pdf)]

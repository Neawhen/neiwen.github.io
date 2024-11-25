---
layout: page
title: Smart City
description: "Soar: Design and Deployment of A Smart Roadside Infrastructure System for Autonomous Driving <br> CoEdge: A Cooperative Edge System for Distributed Real-Time Deep Learning Tasks"
img: assets/img/lamppost.jpg
importance: 2
category: work
---

**Soar: Design and Deployment of A Smart Roadside Infrastructure System for Autonomous Driving**

MobiCom 24 <a href="https://neawhen.github.io/neiwen.github.io/assets/pdf/soar_mobicom24.pdf" target="_blank" rel="noopener noreferrer"> Paper </a> 

Recently, smart roadside infrastructure (SRI) has demonstrated the potential of achieving fully autonomous driving systems. To explore the potential of infrastructure-assisted autonomous driving, this paper presents the design and deployment of Soar, the first end-to-end SRI system specifically designed to support autonomous driving systems. Soar consists of both software and hardware components carefully designed to overcome various system and physical challenges. Soar can leverage the existing operational infrastructure like street lampposts for a lower barrier of adoption. Soar adopts a new communication architecture that comprises a bi-directional multi-hop I2I network and a downlink I2V broadcast service, which are designed based on off-the-shelf 802.11ac interfaces in an integrated manner. Soar also features a hierarchical DL task management framework to achieve desirable load balancing among nodes and enable them to collaborate efficiently to run multiple data-intensive autonomous driving applications. We deployed a total of 18 Soar nodes on existing lampposts on campus, which have been operational for over two years. Our real-world evaluation shows that Soar can support a diverse set of autonomous driving applications and achieve desirable real-time performance and high communication reliability. Our findings and experiences in this work offer key insights into the development and deployment of next-generation smart roadside infrastructure and autonomous driving systems.


**CoEdge: A Cooperative Edge System for Distributed Real-Time Deep Learning Tasks**

IPSN 23 <a href="https://neawhen.github.io/neiwen.github.io/assets/pdf/coedge_ipsn23.pdf" target="_blank" rel="noopener noreferrer"> Paper </a> 

Recent years have witnessed the emergence of a new class of cooperative edge systems in which a large number of edge nodes can collaborate through local peer-to-peer connectivity. In this paper, we propose CoEdge, a novel cooperative edge system that can support concurrent data/compute-intensive deep learning (DL) models for distributed real-time applications such as city-scale traffic monitoring and autonomous driving. First, CoEdge includes a hierarchical DL task scheduling framework that dispatches DL tasks to edge nodes based on their computational profiles, communication overhead, and real-time requirements. Second, CoEdge can dramatically increase the execution efficiency of DL models by batching sensor data and aggregating the inferences of the same model. Finally, we propose a new edge containerization approach that enables an edge node to execute concurrent DL tasks by partitioning the CPU and GPU workloads into different containers. We extensively evaluate CoEdge on a self-deployed smart lamppost testbed on a university campus. Our results show that CoEdge can achieve up to 82.32% reduction on deadline missing rate compared to baselines.
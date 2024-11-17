---
layout: page
title: Time-sensitive DL on Edge Device
description: "BlastNet: Exploiting Duo-Blocks for Cross-Processor Real-Time DNN Inference <br> RT-mDL: Supporting Real-Time Mixed Deep Learning Tasks on Edge Platforms"
img: assets/img/car.jpg
importance: 1
category: work
redirect: false
---

**BlastNet: Exploiting Duo-Blocks for Cross-Processor Real-Time DNN Inference**

SenSys 22 <a href="https://neawhen.github.io/neiwen.github.io/assets/pdf/blastnet_sensys2022.pdf" target="_blank" rel="noopener noreferrer"> Paper </a> 

In recent years, Deep Neural Network (DNN) has been increasingly adopted by a wide range of time-critical applications running on edge platforms with heterogeneous multiprocessors. To meet the stringent timing requirements of these applications, heterogeneous CPU and GPU resources must be efficiently utilized for the inference of multiple DNN models. Such a cross-processor real-time DNN inference paradigm poses major challenges due to the inherent performance imbalance among different processors and the lack of real-time support for cross-processor inference from existing deep learning frameworks. In this work, we propose a new system named BlastNet that exploits duo-block - a new model inference abstraction to support highly efficient cross-processor real-time DNN inference. Each duo-block has a dual model structure, enabling efficient fine-grained inference alternatively across different processors. BlastNet employs a novel block-level Neural Architecture Search (NAS) technique to generate duo-blocks, which accounts for computing characteristics and communication overhead. The duoblocks are optimized at design time and then dynamically scheduled to achieve high resource utilization of heterogeneous CPU and GPU at runtime. BlastNet is implemented on an indoor autonomous driving platform and three popular edge platforms. Extensive results show that BlastNet achieves 35.07 % less deadline missing rate with a mere 1.63% of model accuracy loss.


**RT-mDL: Supporting Real-Time Mixed Deep Learning Tasks on Edge Platforms**

SenSys 21 <a href="https://neawhen.github.io/neiwen.github.io/assets/pdf/RT-mDL_SenSys2021.pdf" target="_blank" rel="noopener noreferrer"> Paper </a> 

Recent years have witnessed an emerging class of real-time applications, e.g., autonomous driving, in which resource-constrained edge platforms need to execute a set of real-time mixed Deep Learning (DL) tasks concurrently. Such an application paradigm poses major challenges due to the huge compute workload of deep neural network models, diverse performance requirements of different tasks, and the lack of real-time support from existing DL frameworks. In this paper, we present RT-mDL, a novel framework to support mixed real-time DL tasks on edge platform with heterogeneous CPU and GPU resource. RT-mDL aims to optimize the mixed DL task execution to meet their diverse real-time/accuracy requirements by exploiting unique compute characteristics of DL tasks. RT-mDL employs a novel storage-bounded model scaling method to generate a series of model variants, and systematically optimizes the DL task execution by joint model variants selection and task priority assignment. To improve the CPU/GPU utilization of mixed DL tasks, RT-mDL also includes a new priority-based scheduler which employs a GPU packing mechanism and executes the CPU/GPU tasks independently. Our implementation on an F1/10 autonomous driving testbed shows that, RT-mDL can enable multiple concurrent DL tasks to achieve satisfactory real-time performance in traffic light detection and sign recognition. Moreover, compared to state-of-the-art baselines, RT-mDL can reduce deadline missing rate by 40.12% while only sacrificing 1.7% model accuracy.
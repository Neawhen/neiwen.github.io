---
layout: page
title: Time-sensitive LLM in Physical AI
description: "TimelyLLM: Segmented LLM Serving System for Time-sensitive Robotic Applications <br> TypeFly: Flying Drones with Large Language Model"
img: assets/img/robot.jpg
importance: 3
category: work
redirect: false
---

**TimelyLLM: Segmented LLM Serving System for Time-sensitive Robotic Applications**

<a href="https://neawhen.github.io/neiwen.github.io/assets/pdf/timelyllm.pdf" target="_blank" rel="noopener noreferrer"> Paper </a> 

Large Language Models (LLMs) such as GPT-4 and Llama3 can already comprehend complex commands and process diverse tasks. This advancement facilitates their application in controlling drones and robots for various tasks. However, existing LLM serving systems typically employ a first-come, first-served (FCFS) batching mechanism, which fails to address the time-sensitive requirements of robotic applications. To address it, this paper proposes a new system named TimelyLLM serving multiple robotic agents with time-sensitive requests. TimelyLLM introduces novel mechanisms of segmented generation and scheduling that optimally leverage redundancy between robot plan generation and execution phases. We report an implementation of TimelyLLM on a widely-used LLM serving framework and evaluate it on a range of robotic applications. Our evaluation shows that TimelyLLM improves the time utility up to 1.97x, and reduces the overall waiting time by 84%.


**TypeFly: Flying Drones with Large Language Model**

<a href="https://neawhen.github.io/neiwen.github.io/assets/pdf/typefly.pdf" target="_blank" rel="noopener noreferrer"> Paper </a> 

Recent advancements in robot control using large language models (LLMs) have demonstrated significant potential, primarily due to LLMs’ capabilities to understand natural language commands and generate executable plans in various languages. However, in real-time and interactive applications involving mobile robots, particularly drones, the sequential token generation process inherent to LLMs introduces substantial latency, i.e. response time, in control plan generation. In this paper, we present a system called TypeFly that tackles this problem using a combination of a novel programming language called MiniSpec and its runtime to reduce the plan generation time and drone response time. That is, instead of asking an LLM to write a program (robotic plan) in the popular but verbose Python, TypeFly gets it to do it in MiniSpec specially designed for token efficiency and stream interpretation. Using a set of challenging drone tasks, we show that design choices made by TypeFly can reduce up to 62% response time and provide a more consistent user experience, enabling responsive and intelligent LLM-based drone control with efficient completion.



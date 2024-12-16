---
title: Challenge resources
menu_title: Resources
menu_icon: journal-code
---

### Reporting and quantifying

**Code Carbon** - [Python package](https://github.com/mlco2/codecarbon) \
A python package estimating the hardware energy consumption (CPU + GPU + RAM) of your program. 

**Power Hungry Processing: Watts Driving the Cost of AI Deployment?** – [Luccioni et al., 2023](https://arxiv.org/abs/2311.16863) \
A broad study of AI models’ power consumption at inference stage. Experiments are run with Code Carbon and applied to both Natural Language Processing and Computer Vision tasks.

**The Price of Prompting: Profiling Energy Use in Large Language Models Inference** - [Huson et al., 2024](https://arxiv.org/abs/2407.16893) \
A study focusing on LLM inference energy needs. Provides an open-source tool for energy monitoring and additional insights into energy profiles during LLM inference.

**Trends in AI inference energy consumption: Beyond the performance-vs-parameter laws of deep learning** – [Desislavov et al., 2023](https://www.sciencedirect.com/science/article/pii/S2210537923000124) \
The authors gather data on hardware performance and models computing needs during inference. They focus on both vision and NLP tasks, concluding on how energy consumption varies with performance increase.

### A wider perspective on the (negative) environmental impacts of AI

**The great challenges of generative AI (French only)** - [Data For Good, 2023](https://dataforgood.fr/iagenerative/). \
Pages 80 to 107 are dedicated to the environmental impacts of generative AI.

**Awesome Green AI** - [Samuel Rincé](https://github.com/samuelrince/awesome-green-ai) \
A curated collection of Green AI resources including tools, scientific papers and reports. It covers training, inference and model deployment.

### Reducing and optimizing

**Efficient Deep Learning: A Survey on Making Deep Learning Models Smaller, Faster, and Better** – [Gaurav Menghani, 2023](https://arxiv.org/pdf/2106.08962) \
A broad technical survey on making deep learning models more efficient at inference stage. It includes compression (pruning, quantization, clustering…) and training methods, efficient architectures and frameworks as well as automation processes designed to increase energy efficiency. 

**Towards Greener LLMs: Bringing Energy-Efficiency to the Forefront of LLM Inference** – [Stojkovic et al., 2024](https://arxiv.org/abs/2403.20306) \
The authors estimate the influence of three optimization methods for LLM inference, namely workload type, batching and model parallelism. They conclude on their influence with respect to throughput, power and energy consumption.

**Quantization and other optimization modules** \
[Model optimization in Tensorflow](https://www.tensorflow.org/model_optimization/guide) \
[Quantization in Pytorch](https://pytorch.org/docs/stable/quantization.html) \
[vLLM](https://docs.vllm.ai/en/v0.6.3.post1/index.html) 

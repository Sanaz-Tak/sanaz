---
title: "ViT-LCA (AICAS 2025)"
collection: portfolio
---
![](../images/ViTLCA.png)
This work introduces a novel model that combines Vision Transformers with the Locally Competitive Algorithm (LCA) to facilitate their energy-efficient deployment on low-power systems.  

This work introduces ViT-LCA, a novel model that integrates Vision Transformers (ViT) with the Locally Competitive Algorithm (LCA) to enable energy-efficient deployment on neuromorphic platforms. By leveraging ViT's self-attention mechanisms to extract contextual embeddings and combining them with LCA's sparse coding within a single-layer Spiking Neural Network (SNN), ViT-LCA achieves high classification accuracy on datasets such as CIFAR-10, CIFAR-100, and ImageNet-1K. The model extracts self-attention representations once and stores them in non-volatile memory, facilitating in-memory computation and significantly reducing energy consumption compared to other spiking vision transformer models. The approach eliminates the need for dictionary training, as required in traditional LCA, and demonstrates compatibility with memristor crossbar arrays for efficient neuromorphic implementation. ViT-LCA's performance highlights its potential for low-power, high-efficiency AI systems, paving the way for further exploration of transformer-based architectures in neuromorphic computing.

This work introduces ViT-LCA, a novel model that integrates Vision Transformers (ViT) with the Locally Competitive Algorithm (LCA) to enable energy-efficient deployment on neuromorphic platforms. By combining ViT's self-attention mechanisms with LCA's sparse coding in a single-layer Spiking Neural Network (SNN), ViT-LCA achieves high classification accuracy on CIFAR-10, CIFAR-100, and ImageNet-1K datasets. The model extracts self-attention representations once, storing them in non-volatile memory for in-memory computation, significantly reducing energy consumption compared to other spiking vision transformer models. ViT-LCA eliminates the need for dictionary training and supports efficient mapping to memristor crossbar arrays, demonstrating substantial potential for low-power, high-efficiency AI systems in neuromorphic computing.

[📄 Read the full paper (PDF)](../files/ViT_LCA.pdf)

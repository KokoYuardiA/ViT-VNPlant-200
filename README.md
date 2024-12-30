# Vision Transformer for Fine-Grained Plant Species Classification 🌿
This repository contains the implementation and experimental results of our research on utilizing Vision Transformer (ViT) models for fine-grained classification of plant species. The research focuses on evaluating the performance of ViT-B/16 and ViT-L/16 models with different configurations of learning rates, hidden layer neurons, and activation functions.
## 🔍 Research Overview
Accurate classification of plant species plays a crucial role in biodiversity conservation and urban green space management. This research explores the effectiveness of ViT models, leveraging the VNPlant-200 dataset, which consists of 200 classes of plant species with visually similar characteristics. Fine-grained classification is particularly challenging due to the subtle differences between species, and Vision Transformers (ViTs) provide a promising solution by capturing global relationships within images.
## Key Contributions:
1. Learning Rate Optimization:
   - Evaluated learning rates (10^-3, 10^-4, 10^-5, 10^-6) and found that a learning rate of 10^-4 yielded the best results for both ViT-B/16 and ViT-L/16.
   - Achieved accuracy of 0.9597 and F1-Score of 0.9580 for ViT-B/16, and 0.9811 accuracy and 0.9810 F1-Score for ViT-L/16.
2. Hidden Layer Neurons:
   - Investigated neuron configurations (64, 128, 256, 512, 1024).
   - ViT-B/16 performed optimally with 1024 neurons, while ViT-L/16 achieved the best results with 256 neurons.
3. Activation Function Impact:
   - Tested 13 activation functions (e.g., ReLU, Tanh, Hard Tanh).
   - Tanh was the best for ViT-B/16, and Hard Tanh was optimal for ViT-L/16
4. Performance Comparison:
   - ViT-L/16 outperformed ViT-B/16 but required 3.1x more computation time on GPU and CPU.

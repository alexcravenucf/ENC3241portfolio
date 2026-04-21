---
layout: default
title: Proposal
---

# Proposal

AgAI

Name: Alexander Craven				Department: Computer Science

Background 
Florida’s agriculture sector, particularly the citrus industry, faces troubling problems with diseases such as Citrus Greening (HLB) and various fungal pathogens. The problem is so severe that it has resulted in 90% losses in citrus production (USDA, 2025). Standard diagnostic methods to find and resolve this disease require manual inspections by experts; a process that is expensive, time-consuming, and typically only detects the disease after it’s spread. Basically, putting the efforts in vain. However, recent progress in Convolutional Neural Networks (CNNs) has shown success in plant pathology; downsides include the cost of pricey hardware and the need for a fast internet connection (Pal, 2025). With this being so expensive, it makes obtaining this critical piece of technology significantly more difficult for small-scale farms. This project focuses on what I’m calling AgAI, where the goal is to create low-optimized models on low-cost, solar-powered hardware to deliver real-time alerts of potential diseases for a fraction of the cost. 

Methodology 
Data acquisition:
My plan is to create a dataset of over 1,000+ images focusing on common Florida diseases and fungal pathogens. The majority of the data will be sourced from the UCF Arboretum and local farms in the surrounding area. I also intend to use the open-source PlantVillage dataset, which has numerous images of infected plants. Next, I’ll implement data agumentation by rotating, scaling, and changing the brightness on the photos to ensure the model can handle different scenarios with different lighting in real environments.
Model optimizaton:
I’ll start by implementing a Convolutional Neural Network (CNNs) using the Tensorflow Framework. Due to the limited processing power of the Raspberry Pi 5, I plan to utilize transfer learning with a lightweight architecture model, specifically MobileNetV2 (Sandler, 2018). Once the model has been trained to the point that it reaches the 90% accuracy consistently, I will apply Post-Training Quantization, converting it into a TensorFlow Lite format. This will reduce the size of the model and inference latency, allowing for the processing of images without the need of a GPU or internet. 
Device Deployment and Testing:
Once the model is optimized I’ll deploy it onto a Raspberry Pi 5 equipped with a high-resolution camera. This device will be housed in an IP67-rated enclosure. Testing will take place just over 4 weeks at the UCF Arboretum and local gardens, where I’ll be measuring the time it takes to notice a disease and identify it, how the device handles the Florida environment, and how fast it sends alerts. I intend to trial this device in 9 local gardens and will come prepared with gift cards as incentives for volunteering their garden.

Anticipated Outcomes 
The major result of this will be a functional prototype of a “smart field camera” that can identify at least 3 common Florida crop diseases with over 90% accuracy, differentiate between helpful and harmful pests, and provide farmers with live updates. I also expect to produce countless datasets of localized plant imagery that could potentially be used by UCF researchers. After testing is completed, I will make graphs to compare multiple high end CNNs to my budget friendly version comparing three major metrics: cost, accuracy, durability.

Significance 
This project’s goal is to lower the current barrier to entry for smart farming. By providing a $150 device without a cloud connection, it becomes possible to give small-scale farmers the same diagnostic power as industrial-scale farms.
It’s intended to reach small farmers around the Central Florida area, along with local community gardens and the UCF Arboretum staff.
This project will provide new insights into how smaller devices can manage the heat and visual challenges of a Florida farm environment. It also offers a low-cost solution to a statewide issue, resulting in greater crop production/yield. I also hope it could lead to a reduction in the need for such harmful pesticides currently in use.

References
Pal, Chiranjit. “A lightweight and Explainable CNN Model for Empowering Plant Disease Diagnosis.” Scientific Reports, vol 15, no. 1, 2025, pp 1-18, https://www.nature.com/articles/s41598-025-94083-1 

Sandler, Mark. “MobileNetv2: Inverted Residuals and Linear Bottlenecks.” Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition (CVPR), 2018, pp. 4510-4520, https://arxiv.org/abs/1801.04381 

United States Department of Agriculture. “Orange You Glad That Researchers Made A Sweet Discovery For The Citrus Industry?” Agricultural Research Service, 12 Feb. 2025, https://www.ars.usda.gov/news-events/news/research-news/2025/orange-you-glad-that-researchers-made-a-sweet-discovery-for-the-citrus-industry 

Timeline 


Budget 





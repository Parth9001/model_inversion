# Knowledge-Enriched Distributional Model Inversion Attack

This repository contains the implementation of the **Knowledge-Enriched Distributional Model Inversion Attack** using the CIFAR-10 dataset as public data. This project is based on the paper:

> **Chen, X., Wu, L., & Zhang, Z. (2021). Knowledge-Enriched Distributional Model Inversion Attacks.**  
> Proceedings of the IEEE/CVF International Conference on Computer Vision (ICCV).

This implementation uses a custom GAN architecture that leverages knowledge distillation from a target model to reconstruct synthetic images resembling private training data. The attack is evaluated using **Attack Accuracy**, **K-Nearest Neighbor Distance (KNN Dist)**, and **Fréchet Inception Distance (FID)**.

---

## **Project Overview**

Model Inversion (MI) attacks aim to reconstruct private training data from model parameters, posing significant privacy risks. This project implements a knowledge-enriched approach that:

- Distills knowledge from public data using soft labels from the target model.
- Models a distribution of private training examples using a Gaussian distribution in the latent space of the GAN.
- Evaluates attack effectiveness using three metrics: **Attack Accuracy**, **KNN Dist**, and **FID Score**.

---

## **Requirements**

The implementation is built using **PyTorch** and other Python libraries. Install the required dependencies using:

```bash
pip install torch torchvision numpy matplotlib scikit-learn scipy
```

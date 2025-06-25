# Face Recognition with Triplet Loss 🧠📸

This repository contains my implementation of the **Face Recognition** programming assignment from **Course 4: Convolutional Neural Networks** in the **DeepLearning.AI Deep Learning Specialization**.

The project builds a face verification and recognition system using a pre-trained model based on the **FaceNet** architecture and demonstrates the principles of one-shot learning using triplet loss.

## 📘 Project Overview

The system performs:

1. **Face Verification (1:1 Matching):**  
   Determines whether a given image matches a claimed identity — e.g., unlocking a phone with your face.

2. **Face Recognition (1:K Matching):**  
   Identifies a person from a database of known individuals — e.g., security systems in smart offices.

The model maps facial images to a 128-dimensional embedding space, where facial similarity corresponds to Euclidean distance.

## 🧠 Key Concepts & Technical Details

- **FaceNet & Pre-trained Model:**  
  Utilizes a pre-trained deep CNN based on the Inception architecture to produce 128-D face embeddings.

- **Triplet Loss:**  
  Trained using triplets — Anchor, Positive, Negative — to enforce that:
  - Distance(A, P) < Distance(A, N) + margin α  
  While this project demonstrates the implementation of `triplet_loss`, model training is skipped as the pretrained model is used directly.

- **One-Shot Learning:**  
  The system can recognize a person using just one image — a powerful application of embedding-based models.

- **Functions Implemented:**  
  - `triplet_loss` — Demonstrates understanding of the key loss function.  
  - `verify(image, identity)` — Performs 1:1 face verification.  
  - `who_is_it(image)` — Performs 1:K face recognition.

## 🎓 Source & Acknowledgements

This project is from the **"Face Recognition" assignment** in  
[Course 4: Convolutional Neural Networks](https://www.coursera.org/learn/convolutional-neural-networks)  
of the [DeepLearning.AI Deep Learning Specialization](https://www.coursera.org/specializations/deep-learning) by Andrew Ng.

All credit for the dataset, problem formulation, and pretrained model goes to **DeepLearning.AI** and the course instructors:  
**Andrew Ng**, **Kian Katanforoosh**, and **Younes Bensouda Mourri**.

---

> ✨ A hands-on application of face recognition that bridges deep learning theory with real-world use cases like biometric verification and access control systems.

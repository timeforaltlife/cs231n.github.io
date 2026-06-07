
Notes and assignments for Stanford CS class [CS231n: Convolutional Neural Networks for Visual Recognition](http://vision.stanford.edu/teaching/cs231n/)

--- My copy of Schedule page, to know what sequence to read these markdown files etc in ---

# CS231n: Deep Learning for Computer Vision - Study Map

This repository contains my personal study notes and progress tracking for Stanford's CS231n course. The sequence follows the structural roadmap of the official course schedule, linking directly to the Markdown notes within this repository alongside local lecture slides, external primary papers, blogs, and review sessions.

---

## 📘 Phase 1: Deep Learning Basics

### Topic 1: Course Introduction
*   **Concepts**: Computer vision overview, historical context.
*   **Lecture Slides**: [Slides 1](./slides/lecture1_1.pdf) | [Slides 2](./slides/lecture1_2.pdf)

### Topic 2: Image Classification & Linear Classifiers
*   **Concepts**: The data-driven approach, K-nearest neighbor, Algebraic/Visual/Geometric viewpoints, Softmax loss.
*   **Repository Source Notes**: 
    *   [`classification.md`](./classification.md) (Image Classification Problem)
    *   [`linear-classify.md`](./linear-classify.md) (Linear Classification)
*   **Review & Tools**: [Python / Numpy Review Session Colab](https://colab.google.com/github/cs231n/cs231n.github.io/blob/master/python-colab.ipynb) | [Numpy Tutorial Notebook](./python-tutorial.md)
*   **Lecture Slides**: [Slides](./slides/lecture2.pdf)

### Topic 3: Regularization and Optimization
*   **Concepts**: Regularization, Stochastic Gradient Descent (SGD), Momentum, AdaGrad, Adam, Learning rate schedules.
*   **Repository Source Notes**: 
    *   [`optimization-1.md`](./optimization-1.md) (Optimization)
*   **Lecture Slides**: [Slides](./slides/lecture3.pdf)

### Topic 4: Neural Networks and Backpropagation
*   **Concepts**: Multi-layer Perceptron, Backpropagation.
*   **Repository Source Notes**: 
    *   [`optimization-2.md`](./optimization-2.md) (Backpropagation)
    *   [`linear-backprop.md`](./linear-backprop.md) (Linear Backpropagation Example)
*   **Suggested Readings**: 
    *   [Why Momentum Really Works](https://distill.pub/2017/momentum/)
    *   [Derivatives Notes (PDF)](https://cs231n.stanford.edu/handouts/derivatives.pdf)
    *   [Efficient Backprop (LeCun et al.)](http://yann.lecun.com/exdb/publis/pdf/lecun-98b.pdf)
    *   More Backprop References: [[1]](http://neuralnetworksanddeeplearning.com/chap2.html) | [[2]](https://www.youtube.com/watch?v=Ilg3gGewQ5U) | [[3]](https://ctbujp.github.io/posts/2018-04-13-backprop)
*   **Review & Tools**: [Backprop Review Session Colab](https://colab.research.google.com/drive/19S78bZ8TxbCRgZ7S_qg2vO6Z6U_3n6Bf) | [Review Slides](./slides/backprop_review.pdf)
*   **Lecture Slides**: [Slides](./slides/lecture4.pdf)

---

## 👁️ Phase 2: Perceiving and Understanding the Visual World

### Topic 5: Image Classification with CNNs
*   **Concepts**: History of ConvNets, Higher-level representations, Image features, Convolution and pooling.
*   **Repository Source Notes**: 
    *   [`convolutional-networks.md`](./convolutional-networks.md) (Convolutional Networks)
*   **Lecture Slides**: [Slides](./slides/lecture5.pdf)

### Topic 6: CNN Architectures
*   **Concepts**: Batch Normalization, Transfer learning, Classic architectures (AlexNet, VGG, ResNet).
*   **Repository Source Notes**:
    *   [`transfer-learning.md`](./transfer-learning.md) (Transfer Learning Guide)
*   **Architectures Reference**: [AlexNet, VGGNet, GoogLeNet, ResNet Summary](./assets/architectures.md)
*   **Project Context**: [Final Project Overview Guidelines](./slides/project_guidelines.pdf)
*   **Lecture Slides**: [Slides](./slides/lecture6.pdf)

### Topic 7: Recurrent Neural Networks
*   **Concepts**: RNN, LSTM, GRU, Language modeling, Image captioning, Sequence-to-sequence.
*   **Suggested Readings**: 
    *   [Deep Learning Book: RNN Chapter](https://www.deeplearningbook.org/contents/rnn.html)
    *   [Understanding LSTM Networks (Chris Olah Blog)](https://colah.github.io/posts/2015-08-Understanding-LSTMs/)
*   **Lecture Slides**: [Slides](./slides/lecture7.pdf)

### Topic 8: Attention and Transformers
*   **Concepts**: Self-Attention mechanisms, Transformers in Vision.
*   **Suggested Readings & Papers**:
    *   [Attention is All You Need (Original Paper)](https://arxiv.org/abs/1706.03762)
    *   [Attention? Attention! (Lilian Weng Blog)](https://lilianweng.github.io/posts/2018-06-24-attention/)
    *   [The Illustrated Transformer (Jay Alammar Blog)](https://jalammar.github.io/illustrated-transformer/)
    *   ViT: Transformers for Image Recognition: [Paper](https://arxiv.org/abs/2010.11929) | [Google Blog](https://ai.googleblog.com/2020/12/transformers-for-image-recognition-at.html) | [Video](https://www.youtube.com/watch?v=TrdevFK_am4)
*   **Review & Tools**: [PyTorch Walkthrough Review Session Colab](https://colab.research.google.com/drive/1d9UeY4tS8epE8606idZ133v6yYat8-y6)
*   **Lecture Slides**: [Slides](./slides/lecture8.pdf)

### Topic 9: Object Detection, Image Segmentation, Visualizing and Understanding
*   **Concepts**: Single-stage/Two-stage detectors, Semantic/Instance/Panoptic segmentation, Feature visualization/inversion, Adversarial examples, DeepDream and Style Transfer.
*   **Models Covered**: FCN, R-CNN, Fast R-CNN, Faster R-CNN, YOLO.
*   **Suggested Readings**:
    *   DETR: End-to-End Object Detection with Transformers: [Paper](https://arxiv.org/abs/2005.12872) | [GitHub Blog](https://github.com/facebookresearch/detr) | [Video Walkthrough](https://www.youtube.com/watch?v=TCHUMe1N7U0)
*   **Lecture Slides**: [Slides](./slides/lecture9.pdf)

### Topic 10: Video Understanding
*   **Concepts**: Video classification, 3D CNNs, Two-stream networks, Multimodal video parsing.
*   **Review Session**: [RNNs & Transformers Review Slides](./slides/discussion_rnn_transformer.pdf)
*   **Lecture Slides**: [Slides](./slides/lecture10.pdf)

### Topic 11: Large Scale Distributed Training
*   **Concepts**: Hardware utilization, Data/Model Parallelism, Activation Checkpointing.
*   **Lecture Slides**: [Slides](./slides/lecture11.pdf)

---

## 🎨 Phase 3: Generative and Interactive Visual Intelligence

### Topic 12: Self-supervised Learning
*   **Concepts**: Pretext tasks, Contrastive learning, Multisensory supervision.
*   **Suggested Readings**:
    *   [Self-Supervised Learning (Lilian Weng Blog Post)](https://lilianweng.github.io/posts/2019-11-10-self-supervised/)
    *   DINO: Emerging Properties in Self-Supervised Vision Transformers: [Paper](https://arxiv.org/abs/2104.14294) | [Meta Blog](https://ai.facebook.com/blog/dino-v2-the-first-open-source-self-supervised-vision-model-to-outperform-weakly-supervised-models/) | [Video](https://www.youtube.com/watch?v=h3ij3Fn3vjA)
*   **Lecture Slides**: [Slides](./slides/lecture12.pdf)

### Topic 13: Generative Models I
*   **Concepts**: Variational Autoencoders (VAEs), Generative Adversarial Networks (GANs), Autoregressive Models.
*   **Suggested Readings**:
    *   [ELBO — What & Why (Blog)](https://deep-generative-models.github.io/notes/vae/)
*   **Lecture Slides**: [Slides](./slides/lecture13.pdf)

### Topic 14: Generative Models II
*   **Concepts**: Diffusion Models, Score-based Generative Networks.
*   **Lecture Slides**: [Slides](./slides/lecture14.pdf)

### Topic 15: 3D Vision
*   **Concepts**: 3D Shape representations, Shape reconstruction, Neural Implicit Representations (NeRFs, etc.).
*   **Lecture Slides**: [Slides](./slides/lecture15.pdf)

### Topic 16: Vision and Language
*   **Concepts**: Multimodal embedding frameworks, CLIP, Vision-Language Foundation Models.
*   **Lecture Slides**: [Slides](./slides/lecture16.pdf)

### Topic 17: World Modeling
*   **Concepts**: Guest Lecture under Prof. Gordon Wetzstein exploring generative structures for simulated physical realities.
*   **Lecture Slides**: [Slides](./slides/lecture17.pdf)

### Topic 18: Human-Centered AI
*   **Concepts**: Ethical boundaries, biases in vision networks, and fairness metrics.
*   **Lecture Slides**: *(Awaiting slide upload)*

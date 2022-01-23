# Exploring-early-exits
Experiment to explore the techniques of effectively splitting deep neural networks to reduce their training and inference time.
This has been implemented on state-of-the-art neural networks like ResNet50, DenseNet169, MobileNet, VGG16 and EfficientNetB0.

4 experiments were conducted on each of the neural networks:
  1) Experiment 1: Using the original model, training it and measuring performance (base case)
  2) Experiment 2: Adding various early exits, training the whole new model and measuring performance
  3) Experiment 3: Using weights from experiment 2 in the original model, training the rest of the model and measuring performance
  4) Experiment 4: In the early-exit models from experiment 2, using weights of original model from experiment 1, training only exit part of the model and measuring performance

Along with this, the training time taken on Google Colab (GPU - NVIDIA Tesla T4) and personal machine (GPU - NVIDIA GeForce GTX 1660 Ti) was also noted for each of the experiments and networks.

---
title: "Things I Wish I Knew Before Learning Machine Learning"
author: Muthiah
category: story
layout: post
---

<center>
  <img src="https://live.staticflickr.com/65535/54675040957_27c9a3452c_n.jpg" alt="ML Journey" style="border-radius: 8px; margin-bottom: 1em;">
</center>


> *"I thought machine learning was about a literal machine that learns. Turns out... it's not."*


When I first heard the term *Machine Learning*, I imagined a physical machine like a CPU that "learns" on its own, maybe a robot that trains itself to walk. But that’s not it. Machine Learning is actually a **computational system** a method that enables computers to **learn patterns from data and make predictions** without being explicitly programmed.

And honestly, it’s a lot more complex than I initially thought. There are countless algorithms, each with different goals, use cases, and structures.


#### 📚 The Beginning: CNN and My Final Project

During my final year of college, I took a bold step and chose to build a Machine Learning project for my thesis , more specifically, using **Convolutional Neural Networks (CNNs)**. I wanted to create a system that could classify images, and CNN was a powerful algorithm known for its high accuracy in image-based tasks.

Coming from an IT background gave me a slight edge with programming logic, but finding a novel research idea was tough , it felt like “everything had already been done.”

Still, as I dove deeper into CNNs, I was amazed. Just imagine: how can we, as humans, design a system that mimics how our brains process visuals? While we have **natural neurons** that instinctively recognize shapes, colors, and patterns, a computer has to learn it all from scratch.


#### 🔍 How Does a CNN Process an Image?

Every image is just a matrix of **pixels** to a computer, that’s a collection of numbers. Even a 100x100 image means processing 10,000 values. A CNN processes this in several key steps:

1. **Input Layer** – Converts the image into a numerical array.
2. **Convolution Layer** – Applies filters to detect features like edges or textures.
3. **Activation Layer (ReLU)** – Eliminates negative values to improve efficiency.
4. **Pooling Layer** – Reduces dimensionality while preserving important features.
5. **Fully Connected Layer** – Aggregates all learned features to start prediction.
6. **Output Layer** – Produces classification probabilities.

And this process runs over and over each iteration called an *epoch*. That’s just for one algorithm: CNN.


#### 💻 Tools That Saved Me

Initially, I tried running everything **locally on my laptop**. But CNN models are heavy, and my laptop only had 12GB of RAM. A single training session could take **over 7 hours**!

Then I discovered **Google Colab** and it truly saved me. Colab lets you run Python code in the cloud, with access to **free GPUs and TPUs** (with time limits, of course). Benefits include:
- Faster training
- Cloud-based storage
- Easy sharing with teammates or advisors

Other frameworks also made life as an ML beginner much easier:
- **TensorFlow** and **Keras** (now merged)
- **PyTorch**
- **Scikit-learn** (for classical algorithms)
- **OpenCV** (for image processing tasks)

Without these tools, we’d have to manually calculate matrix operations and that’s not fun 😅


#### 💬 Is Python a Must?

Not really.

Python is simply the most popular option because:
- It has easy-to-read syntax
- A huge ecosystem of ML libraries
- A supportive community

But you can also build ML systems using:
- **R** (especially for statistics and visualization)
- **Java** (used in enterprise environments)
- **Julia** (for fast numerical computing)
- **MATLAB** (commonly used in academic research)
- **C++** (for speed-critical applications)

Still, for me, Python remains the most intuitive and productive.


#### 💭 Final Thoughts: In Awe of the Brain and the Algorithm

After learning CNNs and exploring other algorithms, I found myself deeply impressed by two things:
1. **The Human Brain** which processes visual data instantly and subconsciously
2. **Algorithms** which try to replicate that process with lines of code and mathematics

Learning Machine Learning isn’t easy, but it’s incredibly rewarding. And I believe, you don’t need to be an expert to begin you just need to be **curious and willing to learn**.


> If you're just getting started with ML, or have struggled with CNNs and other algorithms like I did , hang in there. You’re not alone. 😊

#### 🚀 Explore My Project

*If you're curious to see what I've been working on, feel free to explore the following project:*
- 🧠 **Image Classification with Deep Learning** : Explore my image classification project using CNNs and transfer learning:  
  👉 [Image Classification Repo](https://github.com/MuthiahAinun/image_classification)



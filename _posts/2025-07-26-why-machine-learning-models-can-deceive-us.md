---
title: "Why Machine Learning Models Can Deceive Us?"
author: Muthiah
category: technology
layout: post
---

<center>
  <img src="https://live.staticflickr.com/65535/54676197335_aea1dd4f63_n.jpg" alt="ML Journey" style="border-radius: 8px; margin-bottom: 1em;">
</center>

A red and green apple, round in shape, that’s what we call a **data point**: specific data about an apple.

Now, if we add more data about other fruits : say, bananas that are green and yellow with a long-curved shape, and so on , this becomes a **fruit dataset**. In other words, a **dataset** is a collection of similar data with the same structure or category.

If we combine a fruit dataset with a vegetable dataset, we end up with two or more datasets. This collection is known as a **data collection**, **multi-dataset**, or **combined dataset**.

#### 🧠 The Core of Learning: Data

In the world of technology, **data is everything**. Just like humans need letters to learn how to read, machines need data to learn anything. Those letters are the *raw material* or *input* , our version of data.

If the data is **accurate and clean**, then the understanding (or prediction) will also be accurate and meaningful.

So yup, **Machine Learning (ML)** learns from data to understand things, just like humans or what I jokingly call  **"Mammal Learning"**. If a child wants to learn English, they need to first understand the **Latin alphabet** (A-Z). But imagine in the middle of learning, they suddenly get exposed to Japanese scripts or Russian Cyrillic letters.

They’ll be confused. And when they try to write “I’m hungry” in English, it might come out as:
"Я’м はんгрý."

A strange mix of Russian and Japanese letters! 😵

That’s exactly why **consistent and context-appropriate data** is critical for humans and machines alike.


#### 🔧 Why Garbage In = Garbage Out

If a model is trained with inconsistent, mixed, or messy data, the output will also be flawed or invalid. That’s why **preprocessing** and **data cleaning** are so crucial.

When you're dealing with thousands or millions of data points, it's impossible to manually check each one for typos or missing values, that’s why automation is needed to clean and validate the data.


#### ❓ So... How Can a Machine Learning Model Mislead Us?

Actually, it’s not the model that tricks us. **We teach it wrong.**

Imagine a child learning English and right before mastering the alphabet, their parent suddenly introduces Japanese scripts. Of course the child gets confused. Should we blame the child?

Nope.  
Just like that child, machines are innocent. They only learn what we give them.


#### 🐋 Real-Life Example: Mislabeling Destroys Meaning

Suppose you're building a model to classify **land vs sea animals**. But in your training data, some marine animals like dolphins and seals are mistakenly labeled as **land animals**.

When the model sees a whale, it might classify it as a land animal. Funny, but tragic.

Why?  
Because the model saw dolphins labeled as land animals, and it learned a **false pattern**.

#### 🔍 Ways Machine Learning Can Mislead Us

#### 1. ⚖️ Biased or Incomplete Data
Imagine building a face recognition model, but your training data only contains images of white-skinned individuals. Then when the model sees a black-skinned face, it misidentifies it.

Why? Because the model never *really* learned to recognize a wide range of faces.

#### 2. 💔 False Correlations
Kind of like a relationship that looks strong but lacks meaning, Upss.

For example: a pneumonia detection model is trained on X-ray images. But it ends up learning from the word **"pneumonia"** written on some X-rays, not the image itself. Result? The model classifies healthy lungs as sick if it sees that word.

Yikes. The model learned **from the label, not the lungs**.

#### 3. 🧠 *Overfitting* (Too Much Memorization)
A good ML model should **learn patterns**, not memorize data.

If it memorizes the training data too well, it performs great during training but fails on real-world data.

This happens when the model is too complex or trained too long.  
High training accuracy, but low test accuracy.  
It knows the answers, but doesn’t understand the questions.


#### 4. 🎯 Misleading Metrics
We often rely only on **accuracy or F1-score**, but those don’t tell the whole story.

Just because a model scores **90% accuracy** , doesn’t mean it's good. Accuracy ≠ *fairness, robustness, or trustworthiness.*


#### 📌 What Makes a Good Model?

Beyond metrics, a truly good model must be:

- ✅ Fair Across Groups

Check performance (like F1-score) **for each subgroup**: men vs women, urban vs rural, etc.  
*If the model performs well for one group but poorly for another, it’s not fair.*


- ✅ Robust to Changes

Test the model on slightly altered data:
  - Blurry images
  - Cut-off objects
  - Noisy input

*If performance drops significantly, it’s not robust.*

- ✅ Matches Real-World Distribution

The model should reflect **real-world data**.  
*If it only sees one scenario (e.g., only old data, or data from one city), it won't generalize well.*


- ✅ Explainable & Trustworthy

Let humans evaluate:
  - Are the predictions reasonable?
  - Can the model's decisions be explained?

Especially important in healthcare, finance, and law.

- ✅ Handles Data *Drift*

The world changes. A model trained before COVID might fail after it.

Try **Cross-Domain or Cross-Time Testing**:  
  - Use 2022 education data to test a model in 2024.
  - If it performs poorly, it’s *overfitting* to the past.


- ✅ Transparent and Interpretable

Many modern models (like deep learning) are **black-boxes**:  
We know the input and output, but not **why** it made a decision.

For example:
  - The model correctly predicts a cat 🐱
  - But maybe it learned to recognize the **grass** behind the cat, not the cat itself.

Or worse: A heart disease model learns from **patient names**, not medical data.

That’s why we must understand what **features** the model relies on what it *thinks* is important.


#### 🧪 So What’s the Solution?

Use **interpretability tools** like:
- 🟢 SHAP (SHapley Additive explanations)
- 🟡 LIME (Local Interpretable Model-agnostic Explanations)
- 🔵 Attention Visualization (especially in NLP)

These tools help us answer:
> *"Why did the model make this prediction?"*


#### 🙌 Final Thought

> Machine Learning doesn't lie.  
> But if we teach it the wrong lessons, it will confidently make the wrong decisions.

So let’s not just aim for high accuracy. 
 
Let’s build models that are:
- Fair
- Reliable
- Transparent
- Truly intelligent

✨ Because understanding how a model thinks is just as important as what it predicts.

#### 🚀 Explore My Project

*If you're curious to see what I've been working on, feel free to explore the following project:*
- 📰 **Machine Learning with MLflow – Indonesian Fact & Hoax News Detection** : A complete ML pipeline with MLflow for predicting fake vs factual political news in Indonesia:  
  👉 [Fact & Hoax News Prediction](https://github.com/MuthiahAinun/Proyek_MSML_Indonesian-Fact-and-Hoax-Political-News)

---
title: "Why Your AI Patent Application Will Get Rejected (And How to Fix It Before Filing)"
date: 2024-11-22
author: Robert Matijasec
categories: [Patent Law, Artificial Intelligence, USPTO Practice]
tags: [AI patents, patent prosecution, USPTO examination, machine learning patents, blockchain patents]
excerpt: "I spent three years as a USPTO patent examiner in Art Units 2498 and 2496, examining AI, machine learning, and blockchain applications. Here's what I learned about why most AI patent applications fail—and how to draft claims that actually survive examination."
---

# Why Your AI Patent Application Will Get Rejected (And How to Fix It Before Filing)

I spent three years as a USPTO patent examiner in Art Units 2498 and 2496—the art units that handle AI, machine learning, cryptography, and cybersecurity applications. I examined hundreds of AI patent applications. Most of them got rejected.

Not because the technology wasn't innovative. Not because the inventors weren't brilliant. But because the patent applications themselves were drafted without understanding what examiners actually look for.

Now that I run my own practice ([QED IP](https://qedip.com)), I use that insider knowledge to help AI and blockchain startups draft patent applications that survive examination. Here's what you need to know.

## A Real Rejection From My Examining Days

Let me show you an actual rejection I issued. I've anonymized it, but this is exactly what happened:

**The Application:** A company filed for a patent on what they claimed was a "revolutionary AI system for automatically adjusting data access policies."

**The Claims:** Here's the independent claim (simplified):

> A computer-implemented method comprising:
> - generating, from a first model parameter, an autoencoder network;
> - measuring a reconstruction error for the autoencoder network;
> - aggregating the reconstruction error and a confidence score corresponding to a complexity level of the autoencoder network;
> - and generating, from the level of difficulty score and an initial data access policy level, a derived data access policy level...

**What I Found (in about 30 minutes of searching):**

1. **Ali et al., "Automatic Modulation Classification Using Deep Learning Based on Sparse Autoencoders With Nonnegativity Constraints"** (Nov 2017)
   - Disclosed using autoencoders with reconstruction error minimization
   - Disclosed complexity scoring via KL divergence
   - Disclosed the exact cost function structure they claimed

2. **Rajarathinam, US 2020/0202179 A1** 
   - Disclosed hyperparameter optimization for neural networks
   - Disclosed varying model architecture (number of layers, neurons per layer)
   - Disclosed using these parameters to control network behavior

3. **Saxena, US 11,178,182 B2**
   - Disclosed using machine learning to dynamically adjust access control policies
   - Disclosed transforming policy data into vector representations
   - Disclosed using autoencoders to learn policy patterns

**My Rejection:**

> "Ali, Rajarathinam, and Saxena are in the similar field of endeavor and related to the technology of secure access via dynamic policies. It would have been obvious to a person of ordinary skill in the art before the effective filing date of the claimed invention to incorporate the features described by using policy data and user data of Saxena as an input to the autoencoder of Ali and the updated policy as the output much as in Saxena. Using the *KSR v. Teleflex* rationale, such a combination uses known methods (using the autoencoder) to produce predictable results (getting an encoder and decoder that yields the most important features of a policy as a derived policy)."

**Result:** All 20 claims rejected.

**The Problem:** The claims were so broad they essentially described "use an autoencoder to adjust policies"—which is just combining two well-known concepts. There was no specific technical innovation. No unexpected results. No solution to a technical problem that others had failed to solve.

## Why AI Patent Applications Are Different

If you're drafting an AI patent application the same way you'd draft a mechanical or chemical patent, you're setting yourself up for failure. Here's why:

### 1. The Prior Art Base Is Massive and Recent

In mechanical engineering, relevant prior art might go back decades. In AI, everything relevant has been published in the last 5-7 years, and most of it is freely available online.

When I was examining, I had access to:
- IEEE Xplore (every AI conference paper)
- arXiv (preprints of cutting-edge research)
- Google Scholar
- Massive databases of existing patents

I could find relevant prior art in minutes. Your "novel" approach to training neural networks? There's probably a paper from NeurIPS 2019 that disclosed it.

### 2. Examiners in These Art Units Are Technical

Art Units 2498 and 2496 don't get random examiners. They get examiners with computer science backgrounds who understand:
- How neural networks actually work
- The difference between supervised, unsupervised, and reinforcement learning  
- What KL divergence measures
- Why certain architectural choices matter

You can't paper over lack of innovation with vague language. We see through it.

### 3. The Abstract Idea Rejection Is Waiting

Under *Alice Corp. v. CLS Bank International*, if your claims are directed to an abstract idea, they're not patent-eligible unless they provide "significantly more" than the abstract idea itself.

For AI patents, this is the killer. If your claims basically say "use machine learning to do X," that's an abstract idea. You need to show:
- A specific technical implementation
- An improvement to computer functionality
- A solution to a technical problem in the field

Generic language like "a trained neural network" or "machine learning algorithm" invites an *Alice* rejection.

## What Examiners Actually Look For

When I examined an AI patent application, here's my workflow:

### Step 1: Read the Independent Claims
I'm looking for:
- **Specific technical details** (not "a neural network" but "a convolutional neural network with specified architecture")
- **Concrete functional language** (not "processes data" but "extracts features using X technique to solve Y problem")
- **Technical improvements** (not "faster" but "reduces computational complexity from O(n²) to O(n log n) by...")

### Step 2: Identify the Alleged Innovation  
What is *actually* new here? Strip away:
- Generic computer components ("processor," "memory")
- Well-known AI techniques ("training a model," "using backpropagation")  
- Obvious combinations ("apply technique A to problem B")

What's left? If the answer is "not much," the application is in trouble.

### Step 3: Search the Prior Art
I'd typically search:
- Keywords from the claims
- The specific AI technique + application domain
- Recent conference papers (NeurIPS, ICML, CVPR, etc.)
- Existing patents in the same space

Finding three references that together teach all the claim elements? That's a rejection under § 103 (obviousness).

### Step 4: Apply *Alice*  
If the claims survive obviousness, I'd check patent eligibility:
- **Step 1:** Are the claims directed to an abstract idea?
- **Step 2:** Do the claims provide significantly more?

For AI patents, Step 1 is almost always "yes." The question is whether you can survive Step 2.

## How to Draft AI Patent Claims That Survive

Here's what works, based on examining hundreds of these applications:

### 1. Focus on the Specific Technical Problem You Solved

**Bad Claim:**
> A method for classifying images using a neural network...

**Better Claim:**  
> A method for classifying medical images with limited training data, comprising: implementing a few-shot learning architecture with a Siamese network structure; using a triplet loss function that enforces a minimum margin between...

See the difference? The second claim identifies:
- The specific problem (limited training data in medical imaging)
- The specific solution (few-shot learning with Siamese networks)
- Technical details that show this isn't just "apply AI to medical images"

### 2. Describe Your Architecture in Detail

**Bad Claim:**
> storing a trained machine learning model...

**Better Claim:**
> storing a trained convolutional neural network comprising: an encoder portion with four convolutional layers using 3×3 kernels, each followed by batch normalization and ReLU activation; a bottleneck layer that compresses the representation to a 128-dimensional latent space; and a decoder portion that reconstructs...

The details matter. They show you're not just using "a neural network" generically—you made specific architectural choices for specific technical reasons.

### 3. Highlight Technical Improvements

**Bad Claim:**
> The method improves accuracy...

**Better Claim:**  
> The method reduces the number of training samples required to achieve 95% accuracy from 10,000 to 500 by implementing a novel data augmentation approach that generates synthetic training examples by interpolating in the latent space of a pre-trained variational autoencoder...

Examiners want to see:
- Measurable improvements
- The technical reason for the improvement  
- Why it's not obvious to just combine existing techniques

### 4. Don't Just Describe the Algorithm—Describe How It Integrates

**Bad Claim:**
> receiving data; processing the data with a neural network; outputting a result

**Better Claim:**
> receiving encrypted transaction data from a blockchain node; preprocessing the encrypted data by applying homomorphic encryption operations that preserve privacy while enabling computation; feeding the preprocessed data to a federated learning model that trains locally on the node without exposing raw transaction data; aggregating model updates using secure multi-party computation...

The integration of multiple technical elements to solve a specific problem is much harder to reject than a generic "use AI to process data" claim.

### 5. Survive *Alice* By Showing Improved Computer Functionality

You can't patent "use AI to predict stock prices" (that's an abstract idea applied to a business method). 

But you *can* patent "a specific neural network architecture that reduces latency in real-time trading systems by processing streaming data with a memory-efficient recurrent structure that maintains accuracy while using 50% less GPU memory."

The difference: you're claiming an improvement to how computers function, not just using a computer to implement an abstract idea.

## Common Mistakes That Guarantee Rejection

### Mistake #1: Claims That Are Really Just Flowcharts

If I can read your claims and they're just describing a process flow ("do A, then B, then C"), without any technical details about *how* A, B, or C are accomplished, that's a rejection waiting to happen.

### Mistake #2: Claiming the Training Data or Dataset

"A method comprising: obtaining a dataset of labeled images; training a neural network on the dataset..."

Data isn't patentable. The process of collecting it usually isn't either. Don't waste claim space on it.

### Mistake #3: Over-Broad Functional Language

"A system for optimizing any machine learning model using any optimization technique..."

This is too broad. You haven't invented all possible optimization techniques for all possible models. Claim what you actually invented.

### Mistake #4: Ignoring the Specification

Your claims can't be broader than what you disclosed. If your spec only describes using convolutional neural networks for image classification, don't claim "any machine learning model for any classification task."

### Mistake #5: No Working Example

The specification should include enough detail that someone skilled in the art could implement your invention. For AI patents, that means:
- Network architecture details
- Training procedures  
- Hyperparameters (or ranges)
- Example results

If your spec is vague ("we use a neural network to achieve improved results"), expect a rejection under § 112 for lack of enablement.

## The QED IP Advantage: I Know What Examiners Are Looking For

When I draft AI patent applications now, I write them thinking about what I would have looked for as an examiner:

✅ Specific technical details that show real innovation  
✅ Claim language that distinguishes from obvious prior art  
✅ Integration of multiple technical elements to solve a concrete problem  
✅ Technical improvements that are measurable and non-obvious  
✅ Specification that enables the invention without being so detailed it limits claim scope  

I also know the prior art landscape in AI/ML because I spent three years searching it daily. I know what papers from NeurIPS 2019 are going to sink your claims. I know which patents in the space are actually relevant and which are just noise.

Most importantly, I know how to position your innovation to survive examination—because I know exactly what would have convinced me to allow an application when I was on the other side of the desk.

## Your AI Innovation Deserves Protection That Actually Works

You've built something innovative. You've solved hard technical problems. You've created value.

Don't let a poorly drafted patent application waste your time and money. Don't file something that's going to get rejected because it was drafted without understanding how AI patents are actually examined.

If you're working on AI, machine learning, blockchain, or cryptography innovations, I can help you protect them the right way.

**Contact QED IP:**  
📧 [robert@qedip.com](mailto:robert@qedip.com)  
🌐 [qedip.com](https://qedip.com)  
📍 Serving AI and blockchain startups nationwide

---

**About the Author:**  
Robert Matijasec is a patent attorney and founder of QED IP (Bukva LLC). He spent three years as a USPTO patent examiner in Art Units 2498 and 2496, examining AI, machine learning, cryptography, and cybersecurity applications. He leverages his insider knowledge of USPTO examination procedures to help startups draft patent applications that actually survive examination. He's admitted to practice before the USPTO and focuses on AI, blockchain, and software innovations.

*This post is for informational purposes only and does not constitute legal advice. For specific guidance on your patent application, please schedule a consultation.*

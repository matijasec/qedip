---
title: "Overcoming § 101 Rejections: A Case Study in AI Patent Prosecution"
date: 2024-11-23
author: Robert Matijasec
categories: [Patent Law, Artificial Intelligence, USPTO Practice]
tags: [AI patents, 101 rejections, patent prosecution, Alice Mayo test, machine learning patents, abstract ideas]
excerpt: "A real-world example showing how strategic claim amendments transformed a § 101 rejection into an allowance. Learn the specific techniques that work when examiners say your AI invention is just an abstract idea."
---

# Overcoming § 101 Rejections: A Case Study in AI Patent Prosecution

When prosecuting AI and machine learning patent applications, § 101 rejections have become almost inevitable. The examiner often argues that your claims are directed to abstract ideas—mental processes like comparing, identifying, or determining—that don't amount to patent-eligible subject matter. But with the right claim amendments and strategic arguments, these rejections can be overcome.

Here's a real-world example from Application No. 17/006,120 that shows how careful claim drafting transformed a § 101 rejection into an allowance.

## The Original Rejection

The examiner rejected claims 1-20 under 35 U.S.C. § 101, finding them directed to abstract ideas—specifically mental processes under MPEP 2106.04(a)(2)(III). The examiner's reasoning was straightforward: the claims recited "comparing" neural network models and "controlling" a communicator to transmit information, which are mental processes that can be performed in the human mind.

Here's what claim 1 originally looked like:

**Original Claim 1:**
> An electronic apparatus comprising:
> - at least one memory configured to store at least one instruction and a first neural network model;
> - a communicator comprising communication circuitry; and
> - at least one processor configured to execute the at least one instruction to:
>   - receive, from an external electronic device, information on a second neural network model stored in the external electronic device through the communicator;
>   - compare the first neural network model with the second neural network model based on the information on the second neural network model...

The examiner applied the Alice/Mayo two-step test and concluded:

**Step 2A, Prong 1:** The claims recite comparing neural network models, which is a mental process.

**Step 2A, Prong 2:** The additional elements—memory, communicator, and processor—were merely instructions to apply the exception using generic computer components.

**Step 2B:** The limitations didn't add significantly more than the judicial exception because they were directed to well-understood, routine, and conventional activities.

The examiner even cited prior art from Wierzynski (US 2017/0024641) to show the claims were obvious, arguing that one of ordinary skill in the art would have been motivated to combine the teachings of multiple references.

## The Key Amendment: From "Processor" to "Processing Circuitry"

The path to allowance came through a critical amendment. Instead of using the generic term "processor," the applicant amended the claims to recite "processor **including processing circuitry**." This subtle but important change transformed the claim from reciting a generic computer component into reciting specific structural elements.

**Amended Claim 1 (key portions):**
> An electronic apparatus comprising:
> - a display;
> - at least one memory storing configured to store at least one instruction and a first **artificial intelligence (AI)** ~~neural network~~ model;
> - a communicator comprising communication circuitry; and
> - at least one processor **including processing circuitry,** ~~configured to execute the at least one instruction to:~~
>
> **wherein the at least one instruction, when executed by the at least one processor, causes the electronic device to:**
>   - control the display to provide a user interface that enables a user to select an **AI** ~~a neural network~~ model communication mode, between an **AI** ~~a neural network~~ model transmission mode, **which transmits information on AI model from the electronic apparatus to an external electronic device**, and an **AI** ~~a neural network~~ model reception mode, **which receives information on AI model from the external electronic device**;
>   - based on the **AI** ~~neural network~~ model communication mode of the electronic apparatus being set to the **AI** ~~neural network~~ model transmission mode, receive, from **an** ~~the~~ external electronic device, that is set to the **AI** ~~neural network~~ model reception mode, information on a second **AI** ~~neural network~~ model stored in the external electronic device through the communicator;
>   - compare a model structure of the first **AI** ~~neural network~~ model with a model structure of the second **AI** ~~neural network~~ model based on the information on the second **AI** ~~neural network~~ model that indicates a layer structure, an internal node configuration, and a node connection of the second **AI** ~~neural network~~ model; and
>   - control the communicator to transmit, to the external electronic device, **the information on AI model containing** changed node weights of the first **AI** ~~neural network~~ model, **without transmitting information of the entire first AI model,** in response to a determination that ~~based on~~ the model structure of the second **AI** ~~neural network~~ model **being** ~~is~~ identical to the model structure of the first **AI** ~~neural network~~ model,
>
> **wherein the changed node weights are node weights changed in a personalization process.**

Notice the strategic changes:

1. **"Processor including processing circuitry"** - This change grounds the claim in specific hardware implementation rather than generic computer components.

2. **"Artificial intelligence (AI)" instead of "neural network"** - Broadens the scope while maintaining technical specificity.

3. **Functional details added** - The amendments clarify *what* information is transmitted and *how* the models are compared, including specific structural elements like "layer structure, an internal node configuration, and a node connection."

4. **"Without transmitting the entire first AI model"** - This limitation emphasizes the technical improvement and efficiency gain, showing this isn't just an abstract comparison but a specific technical solution to bandwidth and efficiency problems.

## Understanding the Examiner's Analysis

The original rejection went through the claims methodically, applying the Alice/Mayo framework to each dependent claim. The examiner consistently found:

**For claims involving model comparison (Claims 1-6):**
- Comparing model structures = mental process
- Transmitting weights = data gathering
- Generic computer components = no inventive concept

**For claims involving model customization (Claim 3):**
- Adding nodes to customize a model = data gathering
- Transmitting node information = mere data gathering

**For claims involving training data (Claims 5-6):**
- Identifying whether training data is stored = mental process
- Transmitting data based on this determination = data gathering

The examiner even provided helpful guidance by distinguishing this application from situations where claims would be patent-eligible. For example, the examiner noted that receiving and transmitting model information was directed to "mere data gathering" under MPEP 2106.05(g), and that using memory and processors was simply applying the exception with generic computing components.

## What Made the Difference?

The successful amendment addressed the examiner's concerns by:

1. **Adding structural specificity**: "Processing circuitry" is more than just a "processor"—it connotes specific hardware implementation.

2. **Clarifying the technical problem**: The claim now explicitly states the invention solves the problem of efficient model updates by transmitting only changed weights, not entire models.

3. **Emphasizing practical application**: The "personalization process" limitation ties the invention to a specific technical context—personalizing AI models on user devices.

4. **Avoiding abstract language**: Rather than just "comparing" and "determining," the claims now recite specific structural comparisons (layer structure, node configuration, node connection) and conditional transmission based on structural identity.

## Lessons for AI Patent Practitioners

This case study offers several valuable lessons:

**1. Be specific about hardware implementation**  
Don't just recite "processor"—use terms like "processing circuitry," "neural processing unit," or other specific hardware components when possible.

**2. Emphasize technical improvements**  
The "without transmitting the entire first AI model" limitation was crucial. It shows the invention solves a real technical problem (bandwidth efficiency) rather than just implementing an abstract idea.

**3. Add structural details**  
Instead of just "compare models," specify *what* is being compared: "layer structure, internal node configuration, and node connection."

**4. Use domain-specific terminology carefully**  
The shift from "neural network" to "AI model" broadened the claims while maintaining technical character. Choose terminology that's both technically accurate and strategically advantageous.

**5. Leverage dependent claims**  
The dependent claims added valuable context about training data storage, model structure differences, and specific scenarios (like stored vs. server-based training data). These helped establish the practical, technical nature of the invention.

## The Prior Art Wasn't the Real Obstacle

Interestingly, the examiner cited Wierzynski (teaching transfer learning between neural networks) and Chen (teaching Net2Net strategies for knowledge transfer). But the § 103 obviousness rejection was secondary to the § 101 issue. Once the § 101 rejection was overcome through structural amendments, the prior art distinctions became clearer.

The examiner noted that Wierzynski taught receiving a second neural network model and training it based on a first model, while Chen taught comparing models and transmitting weight information. Wei added teachings about network morphism. But none of these references, alone or in combination, disclosed the specific structural comparison and conditional transmission of *only* changed weights based on structural identity.

## Conclusion

Overcoming § 101 rejections in AI patent applications requires more than just adding "via a computer" to abstract concepts. It requires:

- **Structural specificity** in how you claim computing components
- **Clear articulation** of the technical problem being solved  
- **Detailed recitation** of what makes your AI implementation different from generic mental processes
- **Strategic terminology** that balances breadth with technical precision

The shift from "processor" to "processor including processing circuitry" might seem minor, but combined with the other amendments, it transformed claims that looked like abstract mental processes into claims that recite a specific technical implementation solving a real technical problem.

When facing § 101 rejections in AI applications, don't just argue that the examiner is wrong—amend your claims to make it obvious that you're claiming a specific technical implementation, not just an abstract idea applied on a generic computer.

---

## Need Help With Your AI Patent Application?

If you're working on AI, machine learning, blockchain, or cryptography innovations, I can help you protect them the right way. I spent three years examining these exact types of applications at the USPTO—I know what examiners look for and what causes rejections.

**Contact QED IP:**  
📧 [robert@qedip.com](mailto:robert@qedip.com)  
🌐 [qedip.com](https://qedip.com)  
📍 Serving AI and blockchain startups nationwide

---

**About the Author:**  
Robert Matijasec is a patent attorney and founder of QED IP (Bukva LLC). He spent three years as a USPTO patent examiner in Art Units 2498 and 2496, examining AI, machine learning, cryptography, and cybersecurity applications. He leverages his insider knowledge of USPTO examination procedures to help startups draft patent applications that actually survive examination. He's admitted to practice before the USPTO and focuses on AI, blockchain, and software innovations.

*This post is for informational purposes only and does not constitute legal advice. For specific guidance on your patent application, please schedule a consultation.*

---

*This case study is based on Application No. 17/006,120, which received a § 101 rejection on April 25, 2023, and was subsequently allowed following the amendments described above.*

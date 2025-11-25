---
title: "Inside the USPTO: How Computer-Implemented Inventions Are Actually Examined"
date: 2024-11-23
author: Robert Matijasec
categories: [Patent Law, USPTO Practice, Computer-Implemented Inventions]
tags: [USPTO examination, patent prosecution, software patents, AI patents, blockchain patents, patent examiner perspective]
excerpt: "I spent three years examining computer-implemented inventions in Art Units 2498 and 2496 at the USPTO. Here's what actually happens behind the scenes when an examiner opens your patent application—and how understanding this process can dramatically improve your chances of getting a patent."
---

# Inside the USPTO: How Computer-Implemented Inventions Are Actually Examined

Most patent attorneys have never examined a patent application. They've argued with examiners, negotiated claim amendments, and written countless responses to Office Actions—but they've never sat on the other side of the desk.

I have. For three years, I examined AI, machine learning, cryptography, and cybersecurity applications in Art Units 2498 and 2496. I know exactly what happens when an examiner opens your application for the first time. I know what makes them write a § 101 rejection in the first 15 minutes, and what makes them spend three hours searching for prior art because they think you might actually have something patentable.

Understanding this process isn't just interesting—it's the difference between an application that gets allowed and one that gets rejected over and over until you give up.

## The First 15 Minutes: Life or Death for Your Application

When an examiner receives a new application, they don't read it cover to cover. They scan for specific things in a specific order, and if they don't find what they're looking for, your application is probably going to get a § 101 rejection before they even look at the prior art.

Here's what actually happens:

### Step 1: The Examiner Reads the Independent Claims

Not the specification. Not the abstract. The claims.

Specifically, the independent claims. If you have 20 claims, the examiner is probably reading claims 1, 8, and 15 (assuming they're independent). They're looking for two things:

1. **Is this claiming an abstract idea?** If the claim reads like a business method or a mathematical formula with "computer" sprinkled in, the examiner is already drafting the § 101 rejection in their head.

2. **Is there a technical solution here?** The examiner is looking for claim language that describes how the invention actually works—not just what it accomplishes.

**What this means for you:** Your independent claims need to immediately convey that you're solving a technical problem with a technical solution. If your claim reads like "A method for improving customer engagement comprising: collecting data, analyzing data, and presenting results," you're going to get rejected even if you have brilliant implementation details buried in the specification.

### Step 2: Quick Specification Scan for Technical Details

If the claims pass the initial smell test, the examiner will skim the specification looking for:

- **System architecture diagrams** that show actual components and data flows
- **Technical explanations** of how things work (not just what they do)
- **Implementation details** that demonstrate you're not just claiming a generic computer

They're not reading every word. They're looking for signs that there's real technical substance behind the claims.

**What this means for you:** Your specification needs to have clear, detailed technical explanations that are easy to find. Burying your implementation details in paragraph 0087 on page 23 means the examiner probably won't see them during the initial review.

### Step 3: The Alice/Mayo Decision Point

Now the examiner makes the critical decision: Is this a § 101 rejection or does it warrant a prior art search?

If the claims and specification have shown sufficient technical character—specific algorithms, novel data structures, unconventional computer operations, measurable technical improvements—the examiner moves on to searching.

If not, you get a § 101 rejection, often with a Form Paragraph that barely mentions your specific invention.

**What this means for you:** This decision often happens in the first 10-15 minutes. Everything about how your application is drafted should be optimized for passing this initial filter.

## If You Pass § 101: The Prior Art Search

Once an examiner decides your invention isn't abstract, they move to searching for prior art. This is where the examination gets interesting—and where understanding examiner behavior really pays off.

### How Examiners Actually Search

Despite what you might think, examiners don't start with Google or general patent databases. They start with:

1. **Classification codes** (CPCs and USPCs) that correspond to your technology area
2. **The "pool"** - applications from the same classification that other examiners in their art unit have cited
3. **Known key references** - certain patents that come up repeatedly in their art unit

Only after exhausting these do they branch out to broader searches.

**What this means for you:** If you cite relevant prior art in your Information Disclosure Statement (IDS), especially recent patents from your classification, you're actually helping the examiner. They'll use your citations as a starting point and may not dig as deeply if they feel you've already addressed the closest prior art.

### The Two-Hour Search Rule

Here's something most people don't know: Examiners have production quotas. A typical "full examination" is given about 8-20 hours depending on the complexity, and that includes:

- Reading the application
- Searching for prior art
- Writing the Office Action
- Interviewing the attorney if requested
- Reviewing the response
- Doing additional searches if needed

For the initial search, examiners typically spend 1-3 hours. If they haven't found a strong rejection after 2-3 hours of searching, they often start thinking about allowing the application or issuing a weak rejection that will be easy to overcome.

**What this means for you:** If your invention is legitimately novel, being clear about exactly what's new helps the examiner search efficiently. If they waste time searching for the wrong things because your claims are unclear, they might accidentally find unrelated prior art that creates problems.

### The Combination Rejection Strategy

When examiners can't find a single reference that discloses everything, they combine multiple references. Here's how they decide which references to combine:

1. **One reference must be "analogous art"** - similar enough field that combining is obvious
2. **There must be a "reason to combine"** - motivation to put them together
3. **The combination must be technically feasible** - no "hindsight bias"

Examiners know that combinations are easier to argue against, so they prefer single-reference rejections when possible. But if your claims are narrow and specific, they may have no choice but to combine 2-3 references, which actually puts you in a stronger position for negotiation.

**What this means for you:** Narrow claims aren't always bad. Sometimes it's better to have a combination rejection you can argue against than a single reference that discloses everything.

## What Examiners Look For in Different Technology Areas

Having examined in Art Units 2498 and 2496, here's what examiners focus on for different types of computer-implemented inventions:

### Machine Learning and AI Applications

Examiners look for:
- **Training data preparation specifics** - not just "collect data" but how you structure, filter, or augment it
- **Novel network architectures** - specific layer configurations that aren't standard
- **Loss function innovations** - custom objectives that solve technical problems
- **Inference optimization** - specific techniques for improving speed or accuracy in deployment

**Common rejection pattern:** Claims that just recite "train a neural network" with no architectural or algorithmic specificity. Every ML patent application does this. You need to claim what's different about your approach.

### Cryptography and Blockchain

Examiners look for:
- **Specific protocol modifications** - exact changes to consensus mechanisms or cryptographic schemes
- **Performance improvements with metrics** - quantifiable gains in speed, security, or resource usage
- **Novel data structures** - new ways of organizing blockchain data or cryptographic keys
- **Interoperability solutions** - technical approaches to connecting different systems

**Common rejection pattern:** Business method rejections for applications that claim "using blockchain to do X" without explaining what's technically new about the blockchain implementation itself.

### Cybersecurity Applications

Examiners look for:
- **Detection algorithms with specifics** - exactly how you identify threats, not just that you do
- **Response automation details** - the specific logic for automated threat response
- **Novel indicators or signatures** - new ways to characterize malicious activity
- **Performance optimizations** - how you maintain security without degrading system performance

**Common rejection pattern:** Claims that describe what security goal is achieved without explaining the technical mechanism for achieving it.

## The Interview: Your Secret Weapon

Here's something most applicants don't fully utilize: the examiner interview.

After you get an Office Action, you can request an interview with the examiner. These typically happen by phone and last 15-30 minutes. Based on my experience on both sides of these calls, here's what makes them effective:

### What Examiners Want From Interviews

1. **Clarity on what you're actually claiming** - If there's confusion about the invention, explain it clearly
2. **Focused discussion of specific claim amendments** - Don't argue about the rejection, propose solutions
3. **Understanding of the technical problem** - Help them see why your solution is non-obvious
4. **Reasonable scope** - Show you're willing to narrow if needed to distinguish prior art

### What Makes Interviews Ineffective

1. **Arguing about whether a reference is prior art** - The examiner has already made that determination
2. **Reading claim language verbatim** - They can read, explain it in plain English
3. **Asking for hints about what would be allowable** - Examiners can't draft claims for you
4. **Being unprepared with specific proposals** - Don't use the interview to brainstorm

**What this means for you:** Come to the interview with 2-3 specific claim amendments ready to propose. Explain the technical distinction clearly. Be ready to narrow scope if your current claims are too broad. Most examiners want to allow applications if they can find a reasonable scope.

## The Final Office Action: Not Actually Final

If you get a Final Office Action, many applicants think they're out of options. Not true.

Examiners issue Final Office Actions when:
1. They've already made their position clear in a previous Office Action
2. No new issues are being raised
3. It's time to force a decision point

But "Final" doesn't mean final. You can:
- **File an After Final amendment** if it clearly overcomes the rejection
- **Request continued examination (RCE)** and keep prosecuting
- **Appeal** if you think the examiner is wrong
- **File a continuation** and try different claim scope

**What this means for you:** A Final Office Action is a negotiation tactic, not a death sentence. If you have a strong invention, keep pushing. Examiners expect this.

## The Real Difference Between Allowed and Rejected Applications

After examining hundreds of applications, here's what separates the ones that get allowed from the ones that don't:

### Allowed Applications Have:

1. **Specific technical details in the claims themselves** - not just in the specification
2. **Clear explanation of the technical problem being solved** - not just the business benefit
3. **Implementation specifics that aren't generic** - particular algorithms, data structures, or system configurations
4. **Measurable improvements** when possible - specific performance gains or efficiency improvements
5. **Claim scope that's appropriately narrow** - covering the actual invention, not every possible variation

### Rejected Applications Have:

1. **Claims that read like user stories or business requirements** - "do X to achieve Y" with no technical how
2. **Generic computer components** - "processor," "memory," "network" with no specific configuration
3. **Specification that describes results but not methods** - what the system accomplishes, not how it works
4. **Overly broad claim scope** - trying to cover every possible implementation approach
5. **Disconnect between claims and specification** - claims that aren't supported by the technical disclosure

## How to Draft Claims That Examiners Understand

Based on what actually works during examination:

### Do This:

```
A method comprising:
  receiving, by a neural network comprising a convolutional layer 
  with kernel size K×K, an input image;
  
  extracting, by applying the convolutional layer with a stride 
  of S pixels, a plurality of feature maps;
  
  generating, based on the plurality of feature maps and using 
  a custom loss function that weights edge detection errors by 
  a factor F, a trained model; and
  
  applying the trained model to classify images with at least 
  X% accuracy improvement over standard architectures.
```

### Not This:

```
A method comprising:
  receiving, by a computer system, an input;
  
  processing the input using machine learning;
  
  generating a trained model; and
  
  applying the trained model to produce outputs.
```

The first claim tells the examiner exactly what's novel. The second claim could describe any machine learning system ever created.

## What Happens After Allowance

Once an examiner decides to allow your application, they:

1. **Write a Notice of Allowance** explaining which claims are allowed and why
2. **Calculate the issue fee** based on your entity size
3. **Forward the case to the Issue Notification Mailing team**
4. **Move on to the next application in their queue**

The application typically issues as a patent about 2-3 months after allowance, assuming you pay the issue fee promptly.

**What this means for you:** Once you get a Notice of Allowance, the examination is over. You can't make claim amendments anymore (except for very limited corrections). Make sure your claims are exactly what you want before the examiner allows them.

## Why This Matters for Your Patent Strategy

Understanding how examination actually works changes how you should approach patent applications:

1. **Draft for the examiner, not for yourself** - They're your first audience, and they're reading quickly
2. **Front-load technical details** - Don't make them hunt for what makes your invention patentable
3. **Be specific in claims** - Generic language triggers generic rejections
4. **Use interviews strategically** - They're free and can save months of written prosecution
5. **Think like an examiner during prosecution** - What would make this easy to allow?

The USPTO examination process isn't arbitrary. Examiners have specific procedures they follow, specific time constraints they work under, and specific things they're looking for. When you understand this system, you can draft applications that move through it much more smoothly.

---

## Need Help With Your Patent Application?

If you're working on AI, machine learning, blockchain, or cryptography innovations, I can help you draft applications that examiners will understand—because I've been on both sides of the process.

**Contact QED IP:**  
📧 [robert@qedip.com](mailto:robert@qedip.com)  
🌐 [qedip.com](https://qedip.com)  
📍 Serving AI and blockchain startups nationwide

---

**About the Author:**  
Robert Matijasec is a patent attorney and founder of QED IP. He spent three years as a USPTO patent examiner in Art Units 2498 and 2496, examining AI, machine learning, cryptography, and cybersecurity applications. He leverages his insider knowledge of USPTO examination procedures to help startups draft patent applications that actually survive examination. He's admitted to practice before the USPTO and focuses on AI, blockchain, and software innovations.

*This post is for informational purposes only and does not constitute legal advice. For specific guidance on your patent application, please schedule a consultation.*

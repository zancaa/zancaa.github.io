---
permalink: /teaching-with-gen-AI/
title: "Teaching with Generative Artifical Intelligence (GenAI)"
author_profile: true
---

Content developed via conversations with Copilot to teach introduce first-year science students to the concepts behind GenAI. (Copilot generated the basic structure and themes, I have tweaked structure in some places and modified examples. In-class activities draw on my expertise in tertiary education.) This page contains:
- The intended learning objectives for the content. The teaching activities designed to reach the intended learning objectives are described below.
- Two-hours of lecture content. Desgined to be delivered synchronously, but can be adjusted to be asynchronous (polls can be run asynchronously, for example).
- Two-hours of applied class content. Including some python coding.

For advanced students, more theory would be introduced (e.g. mathematical formulae). For statistics students, the focus would focus more heavily on data and training. 

Intended learning objectives
======
- Explain what artificial intelligence is
- Describe the relationships and differences between artificial intelligence, machine learning, and GenAI
- Explain how a machine learning algorithm works
- Understand the limitations, biases, ethical and environmental concerns regarding GenAI use

Two-hour lecture content
======
## Opening activity (7-ish minutes) 
- Poll asking students whether they have heard of GenAI, then ever used GenAI. (Show of hands. Anticipating almost everyone to have heard of and used GenAI tools, even if they have not realised it. This activity is more to guage the engagement of the live audience, if it exists.)
- Anonymous online poll asking students how they *think* GenAI works. (Not too sure what to expect from this one! For an introductory class, this could vary. More for me to learn the knowledge base of those in the room.)
- Anonymous online poll asking students what prompt they would provide GenAI to tell them how GenAI works. (To start conversations around prompt engineering.)
- Use one of the student responses (if they exist) to ask Copilot how GenAI works. Spend some time here unpacking the answer, guaging student's thoughts on the answer, e.g. using a 'hands up' poll asking students whether they *think* they understand how GenAI works after engaging with Copilot's answer. 

## Introducing terms (4-ish minutes)
Don't want to overload students with terms here. An applied class activity will be to explore more specific terms in more detail. Introduce some of the most common. 

Will refer to the following diagram throughout the lecture: 
![Venn diagram of artificial intelligence (AI) terms. Large language models (LLMs) is a subset of generative AI (GenAI), which is a subset of neural networks, which are a subset of machine learning, which is a subset of artificial intelligence.](../images/ai_venn_diagram.png)
We will start by introducing Gen AI:

- GenAI: 'A category of artificial intelligence that can create new content such as text, images, videos and music.' (Source: [Organisation for Economic Co-operation and Development](https://www.oecd.org/en/topics/sub-issues/generative-ai.html), a definition also used by the [Australian Government](https://architecture.digital.gov.au/capability/generative-artificial-intelligence). Question for the class: how do different sources define GenAI? Why may the wording be different?) 

So what is the definition of artificial intelligence? (AI)
- AI: 'An AI system is a machine-based system that, for explicit or implicit objectives, infers, from the input it receives, how to generate outputs such as predictions, content, recommendations, or decisions that can influence physical or virtual environments.' (Source: [Organisation for Economic Co-operation and Development](https://oecd.ai/en/wonk/definition). Question for the class: do we 'like' this definition? What do and do we not like about it?)

## A short history of AI (8-ish minutes)
Okay, so how do these 'machine-based systems' work? Where have they come from?
- These ideas pre-date ChatGPT and even the internet! People have been interested in using machines to automate tasks that humans can do for a long time.
- A first example of AI (using methods we will not cover today) is the 'Logic Theorist' computer program developed by Allen Newell, Herbert Simon, and Cliff Shaw to use symbolic logic to prove mathematical theorems.

## Machine learning introduction (3-ish minutes)
As we have seen above, AI is a broad term that can cover a range of ideas. A subset of AI is machine learning:
- Machine learning: Machine learning (ML) is a field within artificial intelligence (AI) and computer science dedicated to using *data* and *algorithms* to help AI mimic human learning, thereby enhancing its precision over time. (Source: [Australian Government Architecture](https://architecture.digital.gov.au/capability/machine-learning))

The type of data and algorithms used depends on the problem we are trying to solve! Let's start with an example:

## Revision and terminology activity: linear regression as an example of machine learning (10-ish minutes)
Opening activity: ask students who has heard of linear regression (I suspect all of them, but again this provides an opportunity for me to guage engagement later in the lecture). Ask students who could explain linear regression to a high school student (to check their memory/confidence, which will guide how quickly I move through the revision activity). 

A lot of terms used in machine learning are similar to terms students will have met before, place these in context. Machine learning uses *data* to learn. There are certain terms that you may have met previously (e.g. when learning linear regression - will be treated with more thoroughly in a statistics setting) that have different names in the machine learning world. Opportunity to draw on other examples and content in the course that students connect with (e.g. examples from climate change, population dynamics, pharmacokinetics (the Lineweaver-Burk plot is a classic here), or epidemics).
- Recall linear regression that you may have met before. Let \\(Y\\) be a random variable representing the outcome we are interested in (for the Lineweaver-Burk plot, this would be \\(1/V\\), where \\(V\\) is rate of change of product of a chemical reaction). The random variable \\(Y\\) is sometimes referred to as the 'dependent', 'response', 'outcome' or 'target' variable. We wish to determine the relationship between our response variable and a 'predictor' variable \\(x\\). The predictor variable is sometimes referred to as the 'independent', 'explanatory' variable or 'covariate'.  \\(y = m x + c\\) (or \\(y = a x + b\\)).   In machine learning land, we have:

| Symbols | Math words | Machine learning words |
| --- | --- | --- |
| \\(x\\) | Independent variable | Feature |
| \\(y\\) | Dependent variable | Label |

The *data* our machine learning algorithm *trains* on is an input, typically rows and columns. Each row of the dataset is referred to as an *example* and the columns are features and/or labels. In machine learning land, we are trying to identify relationships between features and labels.

The *parameters* in our 'old school' linear regression model are \\(m\\), the slope of our regression line, and \\(c\\), the intercept. These also have corresponding names in maching learning land:

| Symbols | Math words | Machine learning words |
| --- | --- | --- |
| \\(m\\) | Slope | Weight |
| \\(c\\) | Intercept | Bias |


## Logistic regression as an example of machine learning (25-ish minutes)
Ask students for examples of yes/no questions. If there is a good example from the class use it, otherwise have a back up option of image recognition (e.g. using a blurred photo of Taylor Swift, or someone else from popular culture [does such a thing still exist?] - the `good' thing about this example is that facial recognition is a technology that is being used, and this example allows students to reflect on the potential flaws and issues with the technology). 


## Brain break (5 minutes)
For activities longer than one hour, I always allow a few minutes for breath for students (and myself!)



Closing image for the introducing terms section: 
![Venn diagram of artificial intelligence terms. Deep learning is a subset of neural networks, which are a subset of machine learning, which is a subset of artificial intelligence.](../images/ai_venn_diagram.png)
We only covered artificial intelligence and machine learning in this lecture. The other terms, neural networks, deep learning, and large language models (LLMs) are options for you to explore in the activity class.



## Limitations, biases, ethics and cost

<!-- Making a start on
Two-hour applied class content
======
Drawing on the content from the lecture, we wish to expand students' understanding of terms by giving them the tools to explore concrete examples. 

## Activity 1
In lectures, the terms generative artificial itnelligence, artificial intelligence and machine learning were introduced. The first activity for this activity class is to explore an artificial intelligence topic in more detail. Choose one of the terms below, or another term of your choice, to explore during the class:
- Neural networks
- Deep learning
- LLMs
-->
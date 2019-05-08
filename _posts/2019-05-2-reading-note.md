---
title:  "Paper Reading Notes on AI, HCI, decision-making, and explaination"
date:   2019-05-02 10:00:00
comments: true
excerpt: "My recent paper reading notes, loosely organized chronologically (mainly pasted from Mendeley)"
tags:
  - paper reading
---


## May8 Mixed-initiative interaction, HCI + AI mix


- Horvitz, E. Principles of Mixed-Initiative User Interfaces.

- Allen, J. E., Guinn, C. I. & Horvtz, E. Mixed-initiative interaction. IEEE Intell. Syst. 14, 14–23 (1999).

    > Mixed-initiative interaction is a flexible interaction strategy in which each agent (human or computer) contributes what it is best suited at the most appropriate time.

    - Form the interaction within a diaglogue framework, the AI agent need to have a good timing for inferring the state of other, underst the grounding, listening and interrupting.

    - Eric Horvitz refers to the expected utility, which coincide with my yesterday's readings on decision-making. After reading [his interview](https://www.microsoft.com/en-us/research/blog/ai-and-our-future-with-machines-eric-horvitz/) and [bio](http://erichorvitz.com/), I came to know he is also fascinated by intellilgence, and got a MD and PhD in AI. He is also the PI in the following CHI 2019 paper:

- Amershi, S. et al. Guidelines for Human-AI Interaction.

### Riedl, M. O. Human-Centered Artificial Intelligence and Machine Learning. (2019).

- AI and ML systems need a theory of mind about humans.

- XAI allow non-ML-expert to seek remedy in critical situations.


- Ehsan et al. (2019) show that human-like rationales.


- It mentioned one approach of current XAI is post-hoc explanation: "
translate the internal state of an autonomous agent into the natural language
explanations in the corpus". While I'm reading this and its context, I am thinking: maybe
the brain using a similar system for human-human explanation? i.e. although we don't know exactly what's going on inside the neuron activities, the brain develops a good mechanism to generate rationales from those neuron activities at a macro level (motivation, emotional reaction, thoughts).


Additional readings:

[Eric Horvitz's interview on AI, decision-making, and human-AI collaboration
](https://www.microsoft.com/en-us/research/blog/ai-and-our-future-with-machines-eric-horvitz/)

[AI autumn by Jeffrey Bigham](http://jeffreybigham.com/blog/2019/the-coming-ai-autumnn.html) on a mix of HCI and AI for human-AI collaboration

---

## Simon, H. A. (Herbert A. Reason in human affairs. (Stanford University Press, 1983).

- May6

I read over the 1st chapter and scan through ch 2 and 3. In chapter one, it proposed 3 visions of human rationality:

1. SEU (subjective expected utility) model: it is similar to game theory (and the one used in robots and AI), that a decision maker choose among the alternative actions the one that will **maximize the expected value** in terms of its utility function, by foreseeing and assign a consistent joint probability distribution to all future sets of events. Although elegant, SEU has never been employed in reality, because "human beings have neither the facts nor the consistent structure of values, nor the reasoning power at their disposal that would be required".

2. The behavioural model, or bounded rationality. It admits the fact that human rationality is very limited, very much bounded by the situation and by human computational powers. Compared with SEU, bounded rationality is more valid on how human makes decisions. This theory illustrated how human process limited computational abilities, make adaptive choices, and sometimes survive in a complex, but mostly empty, world.

3. The intuitive model. This one, to me, is very similar to Daniel Kahneman's fast thinking system (in contrast, the bounded rationality is to the slow thinking system). Simon also regards it as a component of the behavioural model.

In ch2, Simon sees an evolutional model of rationality does not do global **optimization** (everything is evolving to some stationary optimal state). Instead, there is lots of local **adaptation** to the current environment and its continually moving .

I also scan through Simon's another two papers on bounded rationality.

- Simon, H. A. A Behavioral Model of Rational Choice. (1955).

> Broadly stated, the task is to replace the global rationality of economic man with a kind of rational behaviour that is compatible with the access to information and the computationalmarcinski that are actually possessed by organisms, including man, in the kinds of environments in which Such organisms exist.

The model of the actual decision process is similar to but a simplified version of a minimax game based on game theory. It substitutes the actual alternatives with decision maker's "considered" alternatives, and regards the pay-off (utility) as satisfactory outcome (not a global optimization process). The decision maker behaves rationally w.r.t the simplified model.


- Simon, H. A. Rational choice and the structure of the environment. (1956).

It states that evidently, organisms adapt well enough to "satisfice" (using very simple perceptual and choice mechanisms); they do not, in general, "optimize."

I was hoping to find unified theory on human decision making, and it seems such an attempt will be quite invalid since decision-making is quite a big topic umbrella. I guess in medical decision making, this will be the same.

I am also thinking, maybe XAI can fit within the bounded rationality, by extending decision-maker's simplified rational model and adding more knowledge with explanations from AI's big data processing and knowledge inferencing abilities. By explaining the reasonings from AI, human can be equipped with better capability to process big data and go deeper into the future to acquire the utility function and joint probability, which human cannot process without the assistance of AI.

Other References:
- https://plato.stanford.edu/entries/bounded-rationality/
- https://en.wikiquote.org/wiki/Bounded_rationality
- https://multi-act.com/bounded-rationality-unbounded-confidence/

---

## Pearl, J. & Mackenzie, D. The book of why : the new science of cause and effect.

- Apr26 - May5

I know this book from another book "possible minds" where Pearl talked about the limitations of opaque learning machines. I was fascinated by the examples Pearl gives about the transparent-vs-opacity contrast of Greek and Babylonian astronomers. Although Babylonian astronomers were masters of black-box predictions and had better accuracy to their Greek rivals. Greek astronomers, in contrast, use wild modelling strategy with metaphorical imagery. Such a model- rather than a function-based approach incubates the modern astronomy. Similar cases also occur repetitively in history, such as why the science is not born in China, instead of in the west, although the ancient Chinese has advanced the knowledge in nature. But such knowledge is only for application purpose, not for scientific discovery which requires generalization and abstraction of such knowledge.

The above examples are good motivations for explanation requirements in model ML models. Although Pearl did not provide an explicit explainable AI approach in "the book of why", it tells a complete story about the elements and development of causal inference. Current big data and DL approaches are at the level of correlation inference. In statistics, we always remind ourselves that "correlation does not imply causation". We need such frequent reminder because our brain is wired to process causality. Thus, it seems like talking about causality is a taboo in statistics. In the first half of the book, Pearl tells the story of how the Causality Revolution happened under such environment. The causal diagram, which is similar to the author's invention, Bayesian diagram, is a good tool to be coupled with the data to do causal inference. So instead of avoiding doing causal inference (throw the baby out with the bathwater), causal inference suggests that after carefully controlling for the confounders (like the RCT), the correlation in observational data IS causality. They have different ways to deal with confounders (back and front door adjustment, instrumental variables), so that with only the observational data and the causal diagram, we can make causal inference without having to conduct a randomized controlled trial (RCT)! Such tools can even enable us to do counterfactual reasonings.

---

## Darwiche, A. Human-Level Intelligence or Animal-Like Abilities? (2017).

- May2

This is a high-level commentary work from the conversation of the authors with many other people in and outside AI communities, on the current trends in AI. I get to know this work from Pearl's "the book of why". It sees the current deep learning trend as the curve fitting for the cognition functions (vision, language, speech recognition). It negates the recent progress in DL and contributes them to merely the improvement of computational power and data (which is true. It points out that NN is invented long ago).

It also emphasizes on the explainability challenge in AI. A model-based approach can allow AI users to ask more questions (what if, counterfactual) that are beyond the ability of the function-based approach (rely on data-collection, input-output mapping). In this part, he quotes Judea Pearl in the book of why ch1:


> There is only one way a thinking entity (computer or human) can work out what would happen in multiple scenarios, including some that it has never experienced before. It must possess, consult, and manipulate a mental
causal model of that reality.

It points out that "the vocabulary of (existing) explanations is restricted to the function inputs" (feature attribution). These limited vocabulary face challenges when encountering novel situations. According to Pearl, "model-based explanations are also important because they give us a sense of “understanding” or “being in control” of a phenomenon".

In the end, it points out the future challenge of AI should be combining the model and function based approaches(mapping them to slow and fast human thinking, which is interesting).
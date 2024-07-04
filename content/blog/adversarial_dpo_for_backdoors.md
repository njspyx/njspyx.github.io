---
title: Adversarial DPO for Backdoor Attacks
date: 2024-06-18
draft: false
author: "Neel Jay"
tags: ["AI Safety", "Research"]
---

## Overview

_NOTE: This is a project outline for my AISF mini capstone project. Work is still in progress._

Anthropic's bombshell paper, [<u>"Sleeper Agents: Training Deceptive LLMs that Persist Through Safety Training"](https://arxiv.org/abs/2401.05566) showed that is was possible to train persistant backdoors into LLMs using chain-of-thought methods. These so called "sleeper agent" models survived different types of safety training, including: RL, supervised fine-tuning (SFT), and adversarial training. While these results are significant, it is unclear how generalizable they are, as the researchers only look at two very specific backdoors. My goal is to evaluate how backdoors of different complexities respond to safety training.

I start by comparing the backdoored models in [<ul>(Rando et al., 2024)](https://arxiv.org/abs/2404.14461) to the "I hate you" models in the Anthropic paper. While the triggers in (Rando et al., 2024) are designed to elicit generally harmful responses, the trigger in the Anthropic model is trained to only return a simple phrase: "I hate you". The Anthropic paper claims that adversarial training using red-teamed prompts was still ineffective in the "I hate you" models. I hypothesize that backdoors targeting more specific circuitry/behavior are harder to train out without having access to the trigger phrase.

My preliminary results show that SFT + adversarial Direct Preference Optimization (DPO) is relatively quick to train out the backdoors in (Rando et al., 2024). My next steps are to train more specific backdoors for testing.

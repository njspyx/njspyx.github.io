---
title: "Apart Research Deception Hackathon Recap"
date: 2024-07-02
draft: false
author: "Neel Jay"
tags: ["AI Safety", "Hackathon", "Research"]
---

## Overview

Over the weekend, I completed my first "research hackathon" with [<u>Apart Research](https://www.apartresearch.com/), a decentralized organization that hosts sprints and funds research teams working on important problems in AI safety. This sprint was focused on AI deception. As AI systems become more capable, the idea that they might lie or spread misinformation for their own reward signal becomes a realistic concern. Example scenarios include:

- An AI agent lying to stock investors to make money for its company.
- A model deceptively masking its harmful intentions by appearing aligned during safety training/eval.

For the hackathon, I met my team online only a few hours before the start time. We essentially brainstormed, tested, and wrote-up our project in <48 hours! Since the event was completely virtual and all of us lived in different time zones, collaboration was chaotic at times.

Despite this, I'm proud that we were able to put together a solid result. By the end, I had more appreciation for the ability to formulate experiments and tell coherent stories in research. It's not always about now technical your codebase is. I will definitely come to the next one with a better understanding of what a 2 day research project should look like.

Our final write-up can be found here: https://www.apartresearch.com/project/evaluating-steering-methods-for-deceptive-behavior-control-in-llms.

Our github repo (forked version by me) can be found here: https://github.com/njspyx/apart_hack_steering_vectors_deception

## Future Directions

While the hackathon is over, I intend to continue exploring the ideas in our paper. Some ideas I wish to explore are:

- Building an interactive UI to see steering vector projection values while talking to a Llama 7B model.
- Elaborating on the idea of using activations to guide models for deception dataset creation (inspired by [<u>this post](https://www.alignmentforum.org/posts/iHmsJdxgMEWmAfNne/red-teaming-language-models-via-activation-engineering)). Creating more diverse examples of deception by combining "dishonesty" vectors with other steering vectors may give us a more robust and generalizable dataset to work with.


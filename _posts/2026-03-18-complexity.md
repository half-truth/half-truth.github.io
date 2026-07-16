---
layout: post
title: Complexity
date: 2026-03-18 19:55:00 +0800
---
> "Fred Brooks explained this in 1975 in his The Mythical Man-Month."  
> "He draws a simple diagram with four quadrants. In the top-left corner sits the Program... you can transform your program into a Product... you can get to a Programming System... in the bottom-right corner sits the Programming Systems Product..."  
> "With a multiplication of the effort (he approximates it at 3x)... you can transform your program into a Product... Through another multiplication of the effort you can get to a Programming System...
The distance between the two corners is not incremental. It is a multiplier. “Three” times the effort to turn your script into something anyone can use. “Three” times again to make it coexist with everything else."
>
> \- [No you can't build it in a day](https://blog.alaindichiappari.dev/p/no-you-cant-build-it-in-a-day)  

> "Deep modules provide substantial benefits with minimal costs, as their interfaces hide internal complexities."  
> "Designing deep classes and dividing your module interface from its implementation hides complexity, allowing users to interact with a simplified abstraction..."  
>
> \- [Must classes be small? Wrong question.](https://blog.alaindichiappari.dev/p/must-classes-be-small-wrong-question)  

> "The complexity being pulled down is closely related to the class’ existing functionality (e.g. retry-timeout loops in a client hiding API calls)."  
> "Will your users (or any upper-level module) be able to determine a better value than we can determine here?"  
>
> \- [Death by configuration parameters - Where to place complexity?](https://blog.alaindichiappari.dev/p/death-by-configuration-parameters)  


> I often hear this argument from people who have just started building AI agents: “Given the right context, the possibilities are endless.”  
>
> This is a deeply flawed assumption.  
>
> There are two fundamental problems.  
>
> 1\. Correct context does not guarantee correct behavior Even with the right context, an LLM can still choose a sub-optimal path. This is not a theoretical concern — it is observable in practice. If context alone were sufficient, basic evaluation benchmarks would consistently reach 100% test success. They don’t. Models reason probabilistically, not deterministically, and therefore correctness cannot be reduced to context quality alone.  
>
> 2\. “Right context” is itself an unsolved problem The real difficulty is shifted upstream: what does having the right context actually mean?  
>
> Determining relevant context is extremely hard. Modern agent architectures largely exist to solve this exact issue. To identify useful information, you must search through vast amounts of possible context — but relevance cannot be known without already understanding the task. This creates a recursive problem:  
>
> +   You need context to decide relevance.  
>
> +   You need relevance to choose context.  
>
> Agents attempt to bridge this gap by searching sources, retrieving information, and maintaining memory. But in practice, sources are often incomplete, outdated, or incorrect. As a result, the model frequently operates on imperfect inputs and produces imperfect outcomes.  
>
> The implication As a founder building an AI company its important for me to state the fact ie. - Today LLMs work reliably only within relatively narrow instruction spaces and controlled environments. Supplying more context does not unlock unlimited capability; it mostly shifts complexity into retrieval, validation, and orchestration layers (aka the harness).  
>
> “Just give it the right context” is not a solution — it is where the real engineering problem begins.  
>
> \- [LLMs and Context @tusharmath]()


---
title: "Why should you draw Software Architectures?"
seoDescription: "Optimize Architecture Drawing: Enhance understanding, evaluate change, maintain stability, and improve communication with effective diagrams and pract..."
datePublished: Thu Apr 20 2023 13:31:42 GMT+0000 (Coordinated Universal Time)
cuid: clgp5vv3q00000al3h20s8u5c
slug: why-should-you-draw-software-architectures
canonical: https://www.cafeio.xyz/why-should-you-draw-software-architectures/
cover: https://cdn.hashnode.com/res/hashnode/image/stock/unsplash/pvMVecxVoW0/upload/d49ae453dae1d39dde6ebe522d9c585c.jpeg
tags: software-architecture

---

> Thoughts & Experiences for Drawing Software Architecture

Most Architects represent their thoughts in the form of diagrams. These are of varied types and formats.

\- Some like to represent in the form of mixed formats representing Data flow, Applications, Infrastructure all in a single view while others are often selective about what is captured - Some will focus on direction of arrows, strength(thickness) of lines, colour of lines while others might doodle away - Choosing the amount of detail presented is a choice that is individual too unless stronger standards exists

All of them are Correct and there’s always more that a single diagram can communicate. But why are diagrams so effective in describing architectures ? The answers lies in a definition or more so understanding of the Term.

While there are many I love the definition by Mr. Martin Fowler, “**the shared understanding that the expert developers have of the system design**” ..! In a complex system with multiple services and varied tech stack this defination helps intutively understand why there is a need to draw.

Softwares evolve and are constantly under change. With this there is a natural need to understand the impact of a change on the overall system. This is critical to maintaining stability and continuity of the system. How many times has it happened that we find ourselves changing a piece scared to death about it causing a cascading impact in production, or blowing off a downstream system due to lack of awareness of the overall picture. This awareness is what Architecture diagram brings in.

So next time if you have a change ensure that the first activity within your sprint is to assess the architecture impact. *Even if there is none it is important to capture a simple* ***ADR (Architecture decision record)*** *describing the requirement and capturing the conversation.*

## Best Practises out of the personal experience

* Use colors to represent changing states
    
* Ensure that arrows follow a single convention (Data flow, Call Flow etc)
    
* Group multiple interfaces and move them to a different diagram basis the interoperability method (All external REST APIs are grouped under a single group)
    
* Different environments can have different diagrams with a graduation process guiding them
    
* Limit the details (Focus on requirements and eliminate the noise)
    

In the next post, I will try to a take a sample app draw it as I think might be good. Stay tuned.
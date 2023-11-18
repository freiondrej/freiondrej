---
title: "Tactical vs strategic todo improve, also filename"
date: 2023-11-19
---

Quite early in my career, a colleague of mine had a very different approach to programming than me. He was always able to solve a problem very quickly, seemingly no matter how difficult. From my perspective, the code was rather ugly - it was inconsistent, did not follow many "best practices" (whatever that meant to me at the time), was not maintainable or very readable. **But for the job it was created to do, it worked.** I saw myself as a counterbalance to this - I wanted to write code that would follow best practices, could be considered high-quality and could be something that I was proud of. But it always took me way, way longer to create such code. I was frustrated by this fact and made it my habit that I'd be always late with delivering (redempted by the quality - I wasn't capable of imagining I could create quality code fast).

**Now, years later, armed with more insight into what was happening at the heart of this difference, I think there were several aspects at play.**

One: as I considered it my duty to bring quality into the team, I thought it is totally warranted to invest any time into the quality, technical discussions, contemplating high-level ideas and refactoring "bad" code. Why this helped me immensely to build a solid knowledge foundation, pick up an eye for quality and start a lifelong passion for writing code following best practices, **it was not healthy for the business**. Had I a mentor in that time, I think I could have learnt way earlier about timeboxing, the power of good tradeoffs and fast iterations - without one, I simply cost the company more than I brought to the table.

Two: after reading John Ousterhout's _A Philosophy of Software Design_, I understood that my colleague could be labeled as a "tactical tornado", delivering very fast but without a strategy **todo definition from the book**. I, on the other hand, intuitively strived for a strategic approach, which however was much more costly, because it was always very hard for me to come up with all the abstractions up front. This took me all the longer because of how my brain works - while some people can start with coding pretty much at the same time as they learn about the very first aspect of the domain problem, I first always need to build an understanding of the whole problem, which gives me much better strategic position but also a fundamental delay.

As insightful as these realizations were for me to understand my past, there is also a specific learning for my future: On the topic of building an understanding of the problem and thus picking the right abstractions (as much as an abstraction can ever be considered "right"), I recently found a very simple approach which I pity I didn't come up with myself much earlier. It's called building a _spike_ = writing some exploratory code in a very tactical fashion to grasp enough understanding of the domain problem to be able to then build quality code in a second iteration. I don't have enough experience with spikes yet to decide whether spike should already be production-ready - intuitively, I think not, but maybe under a feature flag it could already bring some very early validation. Building the spike can be done in a collaboration with a product manager, especially in a situation when the domain problem is not fully understood even from a product side. A very important part of leveraging a spike successfully is an agreement of the whole team upon what a spike is and that the subsequent iteration of rewriting the code to a quality one is not something optional. I find this very important - if the engineer does not feel sure that they will really get an opportunity to rewrite the code into a good shape, they will try to account for the possibility of the spike being the final code by actually trying to write it strategically, which denies the purpose of the spike in the first place.
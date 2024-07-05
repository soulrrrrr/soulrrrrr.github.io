---
title: Debug message is important
summary: I spent 3 weeks to find a bug.
date: 2024-07-05
authors:
  - admin
tags:
  - Blog
---

Back in January, I started MIT's 6.5840 Distributed Systems course while I was serving the military. Since I couldn't use electronics in the camp, my weekends were all about catching up on lecture videos and programming homework, and I spend my weekdays in the camp reading papers.

The lectures covered a lot about distributed systems, but the real challenge was the labs, which were all about the Raft concensus algorithm and the key-value service built on it. I knew it was going to be tough, but it totally blew my mind. It was REALLY HARD. If it weren't for some online references (although the lab instruction said you shoudn't post your answer online, you still can find some), I don't think I could've finished the labs on my own.

For most labs, I gave myself about two weeks to think and try things out. The excitement of finishing a lab all by myself was huge. If I got stuck, I'd search for ideas online, and then implement them without looking at the source code directly.

But the last lab was a nightmare. There was this bug thatonly happened 3 times out of 500 tests, and it caused one character missed in the result. After struggling with it for weeks, I almost gave up. This morning, I noticed that I still had the VSCode tab open, so I decided to give it a try. I added debug messages to Raft and finally found the bug! It turned out that two snapshot messages were too close together, and the latter one wasn't received by shardkv. Fixing the Raft code solved the issue.

I spend two months modifying shardkv, even trying to make my structure almost identical to the online solution, but the bug persisted. This whole experience taught me the importance of having debug messages in the right place and remembering to turn them on.
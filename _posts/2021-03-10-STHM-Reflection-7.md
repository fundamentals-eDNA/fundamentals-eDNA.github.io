---
title: "EES 590 Reflections: Metabarcoding & Primer Design"
description: Week 7 Reflections
author: Samuel Tan
---

As an aside, while I am roughly familiar with the mechanisms behind how Illumina works, it never fails to awe me as to the level of technological wizardry needed to come up with things like bridge amplification, especially when you watch videos of the process (it isn't the easiest thing to visualize in your head). 

Interesting points of discussion this week included how primer choice is often a consequence of occupancy effects, first-come-first-served! This in turn affects what sort of taxa are represented in existing databases, with consequences for future studies using these established primers and the design of future primers as well. 

Personally, when it comes to general primers, I've had varying degrees of success with a few CO1 primer sets, ITS1, 28S, Histone 3 and 16S when barcoding my mollusc specimens before I joined Maine-eDNA. It was a little frustrating to have varying degrees of success within different genera. True, molluscs are full of PCR inhibitors, and collected specimens and museum specimens may differ in terms of the quality of extractable DNA, but my PCR success rates were not as consistent as they ought to be.

Andy brought up many interesting points which I was less familiar with (or altogether unfamiliar with), such as doing the first few rounds of amplification with general primers, ligating an adapter to the amplicon, then using a primer matching the adapter for the rest of the amplification cycles. 
qSeq was also a nifty idea: ligating random tags to the 5' end for the first cycle, in order to estimate how many DNA molecules there originally were in the sample. 

To me, the most interesting learning points this week were Andy's previous work on amplification bias, especially the observation that copy number variation is more important than cycle number when it comes to amplification bias, and this has major implications for eDNA, given the degree of stochasticity we have to deal with in our samples. It was also pointed out that many statistical estimates(e.g. Chao1 for diversity) do badly under conditions where the vast majority of species are rare, which may often be the case with eDNA. How to deal with these biases is another issue altogether, but at the very least, this must be something I should always keep in mind. 

Once again, the importance of mock communities was brought up, with the potential to be used for calibrating relative read abundance, and for used in occupancy-based modelling. Of course, as my course-mates have said, making a good mock community is a lot harder in practice than it sounds! I've never actually made one myself, after all. 

It was also interesting, as to how one might be able to estimate abundance indirectly from sequence diversity, with effective population size as an intermediary; while diversity can be estimated via occupancy-based models. Even more interesting was the observation that linking genetic data to traits and abundance leads to much higher accuracy when it comes to classifying processes to data. As someone with no experience in ecological modelling, these approaches are little beyond me, but this is something I hope to learn more about in the years to come, even if it may not necessarily be too relevant to my project ideas at the moment.


Finally, it's been a long time since I was part of leading a discussion of this scale, and while I was rather tongue-tied at some moments, and might not have been too coherent part of the time, I am appreciative of the fact that the Maine-eDNA community is full of nice folk who are more than happy to chip in with their own experiences and get the discussion going organically. I also have to pay more attention to the fact that background knowledge does vary widely among those in the program (e.g. when talking about multiple-sequence alignments and primer design), but it's great that people generally speak up when they are uncertain about concepts, in any case.
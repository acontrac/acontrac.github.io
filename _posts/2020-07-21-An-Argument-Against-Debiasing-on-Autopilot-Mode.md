---
layout: post
title: "An Argument Against Debiasing on Autopilot Mode"
date: 2020-07-21
---

The example I'll use throughout this post is an applicant screening algorithm used by a financial firm to which a diverse pool of candidates applies. For example, Citigroup uses the Alpha system to assess the qualifications of the many candidates who applied in 2020. Alpha was trained by engineers using the profiles of perhaps 10,000 Citigroup candidate profiles in the last 10 years. Citigroup finds that the 90% of the candidates in 2020 who Alpha deems are capable are Asian males. 

This would be concerning to several people, most obviously those females and non-Asian males which Alpha is not representing well enough for Citigroup to claim on its website that it hires a diverse group of people on the floor. We might hear the claim, "Alpha is biased!" And Alpha is biased. Biased algorithms are as ubiquitous as are algorithms. That's the point of discussing challenges on the road to algorithmic fairness! 

Bias in algorithms comes from many contextual variables that I chose not to enumerate here (I don't know them). But one very common source is bias which exists in training data. For example, it might be the case that Citigroup has been applying high standards on candidate literacy in mathematics and statistics, and it may be that Asian males seeking employment in metropolitan areas are likely to be extremely fluent in these subjects, which would explain the tendency towards this group. There are simpler examples. If you have an algorithm that classifies apples as tasty or not depending on the apple's shape, color, and shine, and you pass it training data which overwhelmingly labels green apples as repugnant, the algorithm will be biased against green apples. 

Recently, there have been efforts to debias algorithms by attacking biases in training data. This is promising, because if datasets can be "cleaned" to train algorithms that ultimately more strongly satisfy fairness definitions, there is hope that some semblance of equal protection under the law and equality of opportunity are not threatened as in the case of Citigroup's Alpha (which is fictitious). I will again choose to not enumerate the procedures of debiasing. Here is a <a href="https://arxiv.org/pdf/1908.10763.pdf">paper</a> if you are interested. 

The thought is that if automated decision systems are trained on debiased data, then selling them to companies that seek to use them for whatever they were going to use them for - job screening, for example - is reassuring. I argue to the contrary.

What's the alternative scenario if the buyer of a job-screening algorithm really wanted an algorithm? Hiring engineers in house is likely, in which case past records would have to be supplied by the company (because engineers can't produce training data from thin air). 


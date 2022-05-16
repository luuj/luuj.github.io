---
layout: single
title: "Projects I've Worked On"
permalink: /projects/
classes: wide
---


## Novel Bayesian Model for Nursing Home Data
<img align="left" width="300" style="padding-right:10px;" src="/assets/images/nursing.webp"> Nursing homes were hit hard during the COVID19 pandemic, and many news outlets reported rising interest in the quality of care of these nursing homes. I am developing more efficient models to analyze cost and healthcare utilization data from nursing homes. Furthermore, I am creating new joint metrics that can be used to better compare the quality of nursing homes.

This project is the center of my current dissertation with Sebastien Haneuse. We are looking into a Bayesian model that can tackle the statistical challenges of clustered semi-continuous data. We are also incorporating the competing risk of death into our models, due to the high mortality rate in nursing homes. To see my current progress, check out my <a href="https://github.com/luuj/Semi-continuous-Bayesian-Modeling">simulation and model code</a> on GitHub.

## COVID19 Duration of Viral Shedding
<img align="left" width="300" style="padding-right:10px;" src="/assets/images/covid.webp"> Isolation and distancing practices are fundamental elements of COVID-19 epidemic control. However, the CDC currently recommends only 5 days of quarantine after a positive test. We were interested in whether this recommendation should be re-extended.

For this study, we collected longitudinal viral load, viral culture samples, and CT values from Massachusetts General Hospital employees who tested positive for SARS-CoV-2. For our analysis, we adjusted for covariates including variants of the virus (original, delta, omicron) and vaccine status. We determined that the previous CDC recommendation of 10 days was needed. Check out our <a href="https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8855795/">paper</a> and <a href="https://github.com/luuj/SARS-CoV-2-Infection-Time">analysis code</a>.

## Phase I RCTs and the 3+3 Design
<img align="left" width="300" style="padding-right:10px;" src="/assets/images/ct.webp"> Before a drug can be introduced to market, it needs to undergo extensive testing. The first stage of this testing procedure is the phase I clinical trial, where drugs are tested for toxicity and the correct dosage. Currently, the most common design for phase I clinical trials is the 3+3.

Supervised by Susan Groshen of USC Norris Cancer Center, I wanted to compare the 3+3 to more modern methods at evaluating dose limiting toxicity and maximum tolerated dose. We found that despite the lack of statistical theory backing the 3+3, it performed very well when compared to the continual reassessment method, several Bayesian methods, and the rolling 6. Check out <a href="https://github.com/luuj/3-3-Simulation">my paper and code here</a>.

## Improving the SEIR model for Analyzing COVID19 Spread
<img align="left" width="300" style="padding-right:10px;" src="/assets/images/seir.webp"> 
The SEIR (susceptible, exposed, infectious, recovered) model is commonly used to model infectious disease spread. In a recent paper by <a href="https://www.nature.com/articles/s41586-020-2554-8">Hao et al</a>, they propose expanding this model by appending 3 transition states: presymptomatic infectious (P), unascertained infectious (A), and isolation in hospital (H). 

Although the model was effective in predicting how COVID19 would spread through Wuhan, China, we wanted to improve on their Bayesian methodology. Within their Metropolis-Hastings step, we implemented a relatively new algorithm called DRAM (Delayed Rejection Adaptive Metropolis), allowing for more flexibility and adaptability of the algorithm. This allowed us to increase simulation speed significantly (from 1103 to 593 seconds) while not affecting statistical performance. See our implementation, proposal, and presentation <a href="https://github.com/luuj/Bayesian-Methodology/tree/main/SAPHIRE-master">here</a>.

## Blinded Sample Size Re-estimation
<img align="left" width="300" style="padding-right:10px;" src="/assets/images/ss.webp"> 
Sample size and power calculations are critical when designing a clinical trial. In the past, clinical trials only performed these calculations at the start of the trial; however, researchers have begun implementing more adaptive procedures recently. For example, trials are often stopped to monitor if the treatment being evaluated is efficacious enough, or if the trial should be stopped for futility. During this stage, a common method of adaptation is performing sample size re-estimation to ensure that the trial has enough power to detect a difference between treatments.

For this project, I was tasked to perform sample size re-estimation for the <a href="https://www.thelancet.com/journals/landia/article/PIIS2213-8587(19)30346-8/fulltext">Long-term Odanacatib Fracture Trial (LOFT)</a>. Furthermore, I wanted to test through simulation how the type I error would be affected from changes to the sample size, power, accrual rate, and how many years patients would be followed up for. Check out my analysis and simulation code <a href="https://github.com/luuj/Recurring-endpoints---SS-reestimation">here</a>.

## Comparing Naive vs. Robust Methods for Cluster Randomized Trials
<img align="left" width="300" style="padding-right:10px;" src="/assets/images/cluster.webp"> 
Clustered randomized clinical trials are trials where patients are recruited in "clusters". These clusters are typically locations where individuals are likely to be correlated with one another, such as a school, nursing home, or village. These types of trials are becoming increasingly popular; however, methodology is still being developed.

When performing survival analysis on clinical trials, the proportional hazards Cox regression model is often used. The goal of this project was to determine if performing a naive analysis using the standard Cox model would be sufficient. I compared results from the naive model with the robust sandwich variant and randomization-based variant in 27 different scenarios. We discovered that despite not adjusting for the correlation inherent in these clusters, the naive Cox model still performed just as well as the other two models. Check out the code and presentation for my project <a href="https://github.com/luuj/Clustered-RCT-simulations">here</a>.

## Comparing Home-based vs. Hospital-based Palliative Care
<img align="left" width="300" style="padding-right:10px;" src="/assets/images/palliative.webp"> 
Palliative care focuses on providing relief from the symptoms and stress of an illness. The goal is to improve quality of life for both the patient and the family. However, some patients and families prefer receiving treatment in the comfort of their own home compared to at the hospital. We were interested in whether or not home-based palliative care was as effective as hospital-based palliative care.

This was a 5-year clinical trial enrolling 1155 participants. My main tasks involved managing confidential patient files sent from Blue Shield, creating surveys and scripts in the REDCap database, and recording/monitoring new inpatient referrals. I also created scripts to automatically create summaries of demographic information, ineligibility criteria, and patient concerns so that we could present them to the DSMB and funding agencies. Check out the <a href="https://pubmed.ncbi.nlm.nih.gov/31486727/">study</a> and my <a href="https://github.com/luuj/Palliative-care-clinical-trial">code here</a>.


## Eribulin Phase II Clinical Trial for Bladder Cancer
<img align="left" width="300" style="padding-right:10px;" src="/assets/images/bladder.webp"> 
Eribulin is a potential new treatment for bladder cancer. This was a combined phase I/II clinical trial aimed at determining whether or not Eribulin could move on to a phase III trial. At USC's Norris Cancer Center, I worked with Susan Groshen on the statistical analysis of this trial data.

First, we looked at the frequency of adverse events to generate toxicity tables for the DSMC report. Second, I coded up scripts to generate table I statistics, response tables, and Kaplan-Meier curves for progression-free and overall survival. Lastly, I ran a multivariate Cox regression model for progression-free survival. Check out the <a href="https://pubmed.ncbi.nlm.nih.gov/22198425/">paper</a> and <a href="https://github.com/luuj/Urothelial-carcinoma-study">my code here</a>.

## Inferno Tick Counter for Bluelite/Steroid OSRS Client
<img align="left" width="300" style="padding-right:10px;" src="/assets/images/inferno.webp"> 
Old school runescape is a classic MMORPG that released back in 2001. Despite its age, the game still has around 80,000 active players and is growing. In the game, one of the hardest challenges a player can overcome is completing the Inferno, a 69 wave gauntlet of increasingly difficult combat puzzles. 

A large number of players choose to use 3rd party clients to run the game, allowing for a plethora of plugins that improve quality of life. I wrote a customizeable plugin that tracks enemies and overlays a counter over them, indicating when they will next attack. This allows players to anticipate and defend against incoming attacks easily. You can download my plugin with accompanying instructions <a href="https://github.com/luuj/BlueLite-Inferno-Plugin">here</a>.

## Pokemon Battle Simulator
<img align="left" width="300" style="padding-right:10px;" src="/assets/images/pokemon.webp"> 
Pokemon is a popular franchise where players set out to capture and battle creatures they encounter. I, along with 4 other friends, created this simulator which attempts to recreate the battling component of the Pokemon video games. 

We implemented animated sprites, attributes from the player-run <a href="https://bulbapedia.bulbagarden.net/wiki/Pok%C3%A9mon_Wiki">wiki</a>, and the various battle formulas present in a typical Pokemon battle. Players are able to choose teams of 6 from the original 151 generation I Pokemon. Battle either locally or over WiFi with chat and emojis. Check out our implementation <a href="https://github.com/luuj/Battle-Simulator">here</a>.

## Destructo-Block Mobile Game
<img align="left" width="300" style="padding-right:10px;" src="/assets/images/destructo.webp"> 
Neopets was a popular website that allowed users to raise a cartoon pet, explore an interactive point-and-click world, and play hundreds of flash games to earn neopoints. One addicting game from Neopets was Destruct-o-match, a puzzle game with a goal of destroying as many blocks as possible by clicking on bundles of adjacently colored blocks. 

To learn the workflow of developing an Android mobile game, I recreated this flash game using assets from the original. I coded up the algorithm that enforces the game's rules, set up a point scoring system based on how many blocks were destroyed, and included a timer that limits how much time players had to complete each level. Levels were randomly generated and made to get increasingly harder. Check out the <a href="https://github.com/luuj/Destructo-Block">game here</a>.

## Polar Deep Web Crawler
<img align="left" width="300" style="padding-right:10px;" src="/assets/images/deepweb.webp"> 
The deep web is often associated with criminal activity. Furthermore, it is difficult to access the deep web unless you are explicitly looking. However, the deep web also holds a plethora of research information that cannot be easily accessed. 

Our goal with this project was to create a search engine that researchers can easily use to scour the deep web for polar-related information. Furthermore, we developed many visualization tools using D3 that are integrated within the search engine to simplify the results. Check out the <a href="http://irds.usc.edu/polar.usc.edu/">website</a> and the <a href="https://github.com/USCDataScience/polar.usc.edu">codebase here</a>.

## Google Web Crawler
<img align="left" width="300" style="padding-right:10px;" src="/assets/images/google.webp"> 
Google is the most used search engine in the world. I wanted to better understand how the search engine crawled through websites, which motivated this project.

The project was a mainly a test of understanding various algorithms and data structures such as DFS, graph theory, crawling policies, and filtering. Check out my implementation <a href="https://github.com/luuj/Web-Parser">here</a>.

## GIF Making
<img align="left" width="300" style="padding-right:10px;" src="/assets/images/hamtaro.webp"> 
Last but not least, a fun side project of mine is making gifs. Whether it be of a cute cartoon or of my friends doing silly things, I find having personalized gifs is a great way to express yourself and get some laughs out of your friends. My GIPHY account has accumulated over 30,000 views so it is also rewarding seeing that other people are using something you <a href="https://tenor.com/users/hamtarofan">created</a>!




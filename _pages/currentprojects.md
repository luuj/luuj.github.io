---
title: Projects
subtitle: What I've been working on lately.
description: Projects I am working on
featured_image: /images/portraits/projects.webp
---



#### Correlation between surrogate endpoints and overall survival in cancer trials
In cancer research, overall survival (OS) is the primary measure used to assess how well new treatments work. But OS can be tough to measure due to longer survival times, challenges with follow-up, treatment crossover, and additional therapies. This makes surrogate endpoints—alternative markers used in place of OS to evaluate effectiveness—an attractive option for researchers. Surrogates can shorten trial timelines, require fewer patients, and even enable single-arm study designs. Two common examples are progression-free survival (PFS) and objective response rate (ORR).

The challenge is knowing whether PFS and ORR are valid stand-ins for OS, which varies based on the type of cancer and treatment. To address this, we examine the link between these three endpoints using Prentice’s criteria. We also evaluate several correlation measures—Pearson’s, Spearman’s Rho, Kendall’s Tau, and Harrell’s C-index—and apply different models to analyze how PFS and ORR relate to OS across various cancer types.

#### Hierarchical models for longitudinal clustered semi-continuous data subject to mortality
During the COVID-19 pandemic, nursing homes were at the forefront due to the vulnerability of their residents. Costs and healthcare utilization emerged as key markers of quality care in these settings. However, data on these markers often exhibit a semi-continuous distribution with a mass of zero values and a long right tail, posing challenges for model fitting and interpretation. Additionally, the high mortality risk among nursing home residents acts as a competing risk.

We developed a novel Bayesian hierarchical discrete-time model to analyze clustered and longitudinal semi-continuous data truncated by death. This model separately addresses the probability mass at zero and the skewed cost distribution, integrating them within a discrete-time framework for semi-competing risks.

We demonstrated the model's applicability through simulations and by examining factors longitudinally associated with cost and healthcare utilization in and across nursing homes, using nationally collected CMS data.

#### Measuring performance for costs in nursing homes 
Building on our hierarchical discrete-time model, we aimed to develop a quantifiable performance measure for clustered longitudinal semi-continuous data affected by mortality. Understanding and comparing nursing home costs is critical for families, policymakers, and healthcare providers, as these costs are a key factor in financial planning for older adults. The growing demand for long-term care due to an aging population adds significant strain on public and private healthcare systems. However, analyzing these data presents challenges, including their semi-continuous nature and the semi-competing risk of death. This project proposed several metrics for profiling nursing homes. We validated these metrics through simulation and applied them to assess nursing homes based on 90-day costs and mortality using nationally collected CMS data for facilities in Massachusetts and California.

#### Comparing methods for multiple-period cluster-randomized crossover trials
Cluster randomized trials (CRTs) are increasingly used to evaluate health interventions, but they are often designed with fewer than 10 clusters. It's unclear which statistical methods work best in these cases, as standard approaches typically assume more than 40 clusters. More complex designs, like multiple-period cluster randomized crossover trials (MPCRCTs), can address issues related to a small number of clusters, but there is limited research on their effectiveness in this context. This project evaluates the performance of generalized linear mixed models (GLMM) and generalized estimating equations (GEE), along with small sample variance corrections, in MPCRCTs with fewer than 10 clusters. The findings from this simulation trial will guide MI-VACUNA, an ongoing MPCRCT studying the impact of motivational interviewing on vaccine hesitancy at two Boston community health centers.

#### Motivational interviewing for vaccine uptake in Latinx adults
Before the COVID-19 pandemic, the World Health Organization identified vaccine hesitancy—delaying or refusing vaccines despite availability—as one of the top 10 global health threats. Despite significant global efforts, it remained a major issue.

This project aimed to address vaccine hesitancy by integrating evidence-based motivational interviewing (MI) into behavioral health (BH) services, supported by electronic reminders and vaccination access at the point of care. In collaboration with Boston College, Harvard University, and the East Boston Neighborhood Community Health Center, we conducted a cluster-randomized crossover trial within four EBNHC programs. The study assessed the impact of MI and BH interventions on COVID-19 vaccine uptake among Latinx adults and examined the influence of vaccine hesitancy factors in the relationship between the intervention and vaccination rates.

#### Duration of viral shedding and culture positivity with post-vaccination breakthrough delta variant infections
Isolation and distancing are key to controlling COVID-19, yet the CDC advises just 5 days of quarantine after a positive test. We wanted to assess whether the 10-day quarantine recommendation should be reinstated.

For this study, we collected longitudinal viral load, culture samples, and CT values from employees at Massachusetts General Hospital who tested positive for SARS-CoV-2. Our analysis accounted for factors like virus variants (original, delta, omicron) and vaccination status. We found that the CDC’s earlier 10-day recommendation was still necessary. Check out our paper <a href="https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8855795/">here</a>.

#### Prevalence, incidence, and reversal pattern of childhood stunting from birth to age 2 years in Ethiopia
Despite a reduction in stunting (low height/length for age), malnutrition rates in Ethiopia remain high. Understanding child growth patterns and stunting estimates is essential for identifying vulnerabilities and potential for recovery. We collected longitudinal data to assess the prevalence, incidence, and reversal of stunting among children aged 0-24 months. The findings indicate a chronically malnourished population, with much of the burden driven by growth faltering during the neonatal period and after 6 months of age. Addressing growth faltering in populations like young children in Amhara, Ethiopia, is critical to eliminating all forms of malnutrition. Check out the HaSET project <a href="https://www.hsph.harvard.edu/haset/">here</a> and our <a href="https://jamanetwork.com/journals/jamanetworkopen/article-abstract/2814235">paper</a>.

#### Determinants of social risk screening and response equity in community health centers
Social determinants of health (SDH), including factors like age, race/ethnicity, sex, language, comorbidities, cultural background, and stress, play a critical role in health inequities. In collaboration with Caring Health Center and the Implementation Science Center for Cancer Control Equity, we aim to analyze how these SDH contribute to disparities in health outcomes.

The data, collected from electronic health records (EHR), presents challenges due to incomplete or missing information. Our goal is to develop methods that account for the complexity and diversity of this incomplete EHR data, with a focus on accurately addressing SDH factors.

#### A simulation evaluation of the effectiveness and usability of the 3+3 design for phase I clinical trials
Before a drug can be introduced to market, it needs to undergo extensive testing. The first stage of this testing procedure is the phase I clinical trial, where drugs are tested for toxicity and the correct dosage. Currently, the most common design for phase I clinical trials is the 3+3.

Supervised by Susan Groshen of USC Norris Cancer Center, I wanted to compare the 3+3 to more modern methods at evaluating dose limiting toxicity and maximum tolerated dose. We found that despite the lack of statistical theory backing the 3+3, it performed very well when compared to the continual reassessment method, several Bayesian methods, and the rolling 6. Additionally, its simplistic implementation was more desirable for researchers. Check out my paper <a href="https://www.proquest.com/openview/88a141f4bfd493b69231606fc30a02cb/1?pq-origsite=gscholar&cbl=18750&diss=y">here</a>.

#### Improving the SEIR model for analyzing COVID19 spread
The SEIR (susceptible, exposed, infectious, recovered) model is commonly used to model infectious disease spread. In a recent paper by <a href="https://www.nature.com/articles/s41586-020-2554-8">Hao et al</a>, they propose expanding this model by appending 3 transition states: presymptomatic infectious, unascertained infectious, and isolation in hospital. 

Although the model was effective in predicting how COVID19 would spread through Wuhan, China, we wanted to improve on their implementation. Within their Metropolis-Hastings step, we introduced a relatively new algorithm called DRAM (Delayed Rejection Adaptive Metropolis), allowing for more flexibility and adaptability of the algorithm. This allowed us to increase simulation speed significantly (from 1103 to 593 seconds) while not affecting statistical performance. See our implementation, proposal, and presentation <a href="https://github.com/luuj/Bayesian-Methodology/tree/main/SAPHIRE-master">here</a>.

#### Blinded sample size re-estimation
Sample size and power calculations are essential for designing clinical trials. Traditionally, these calculations were done only at the trial's outset, but recent practices have introduced more adaptive approaches. For example, trials are now often paused to evaluate if the treatment is sufficiently effective or if they should be halted for futility. At this stage, sample size re-estimation is commonly used to ensure the trial maintains adequate power to detect treatment differences.

For this project, I conducted sample size re-estimation for the <a href="https://www.thelancet.com/journals/landia/article/PIIS2213-8587(19)30346-8/fulltext">Long-term Odanacatib Fracture Trial (LOFT)</a>. Additionally, I simulated how changes in sample size, power, accrual rate, and follow-up duration would impact type I error rates. Check out my analysis and simulation code <a href="https://github.com/luuj/Recurring-endpoints---SS-reestimation">here</a>.

#### Comparing naive vs. robust methods for cluster randomized trials
Cluster randomized clinical trials involve recruiting patients in “clusters” like schools, nursing homes, or villages, where individuals within each cluster are likely to be correlated. While these trials are gaining popularity, the methodology is still evolving.

In survival analysis for these trials, the proportional hazards Cox regression model is commonly used. This project aimed to evaluate whether a standard Cox model, used naively, would be adequate. I compared the results of this naive Cox model with those from robust sandwich and randomization-based variants across 27 different scenarios. We found that, despite not accounting for cluster correlation, the naive Cox model performed comparably to the other models. Check out the code and presentation for my project <a href="https://github.com/luuj/Clustered-RCT-simulations">here</a>.

#### Expanding access to home-based palliative care: A randomized controlled trial
Palliative care aims to alleviate symptoms and stress related to illness, enhancing the quality of life for both patients and their families. Some patients and families prefer receiving care at home rather than in a hospital setting. We sought to evaluate whether home-based palliative care is as effective as hospital-based care.

In this 5-year clinical trial, I managed confidential patient files received from Blue Shield, developed surveys and scripts using the REDCap database, and tracked new inpatient referrals. Additionally, I created automated scripts to generate summaries of demographic information, ineligibility criteria, and patient concerns for presentation to the DSMB and funding agencies. Check out the <a href="https://pubmed.ncbi.nlm.nih.gov/31486727/">study</a> and my <a href="https://github.com/luuj/Palliative-care-clinical-trial">code here</a>.

#### A phase I/II study of E7389 Halichondrin B analog in metastatic urothelial tract cancer and renal insufficiency
Eribulin is a potential new treatment for bladder cancer. This was a combined phase I/II clinical trial aimed at determining whether or not Eribulin could move on to a phase III trial. At USC's Norris Cancer Center, I worked with Susan Groshen on the statistical analysis of this trial data.

First, we looked at the frequency of adverse events to generate toxicity tables for the DSMC report. Second, I coded up scripts to generate table I statistics, response tables, and Kaplan-Meier curves for progression-free and overall survival. Lastly, I ran a multivariate Cox regression model for progression-free survival. Check out the <a href="https://pubmed.ncbi.nlm.nih.gov/22198425/">paper</a> and <a href="https://github.com/luuj/Urothelial-carcinoma-study">my code here</a>.

#### OSRS plugins for RuneLite client
Old school runescape is a classic MMORPG that released back in 2001. Despite its age, the game still has around 140,000 active concurrent players and is growing. Although OSRS offers its own vanilla client, a majority of players choose to use a third-party client called RuneLite due to its open-source nature, quality-of-life improvements, and large developer presence.

By using RuneLite, it allows for a plethora of plugins that improve quality of life that make the game significantly easier to play. Using IntelliJ and the RuneLite API, I wrote several customizeable plugins that do a variety of things including tracking enemies and overlaying a counter over them, tracking projectiles, ground objects, and helpers for various fights. Check out my various plugins <a href="https://github.com/luuj">here</a> and learn how to install them using the official RuneLite wiki. 

#### Pokemon battle simulator
Pokemon is a popular franchise where players set out to capture and battle creatures they encounter. I, along with 4 other friends, created this simulator which attempts to recreate the battling component of the Pokemon video games. 

We implemented animated sprites, attributes from the player-run <a href="https://bulbapedia.bulbagarden.net/wiki/Pok%C3%A9mon_Wiki">wiki</a>, and the various battle formulas present in a typical Pokemon battle. Players are able to choose teams of 6 from the original 151 generation I Pokemon. Battle either locally or over WiFi with chat and emojis. Check out our implementation <a href="https://github.com/luuj/Battle-Simulator">here</a>.

#### Destruct-o-Block mobile game
Neopets was a popular website that allowed users to raise a cartoon pet, explore an interactive point-and-click world, and play hundreds of flash games to earn neopoints. One addicting game from Neopets was Destruct-o-match, a puzzle game with a goal of destroying as many blocks as possible by clicking on bundles of adjacently colored blocks. 

To learn the workflow of developing an Android mobile game, I recreated this flash game using assets from the original. I coded up the algorithm that enforces the game's rules, set up a point scoring system based on how many blocks were destroyed, and included a timer that limits how much time players had to complete each level. Levels were randomly generated and made to get increasingly harder. Check out the <a href="https://github.com/luuj/Destructo-Block">game here</a>.

#### Polar deep web crawler
The deep web is often associated with criminal activity and is difficult to access unless you are explicitly searching. However, the deep web holds a plethora of information that can be used for research.

Our goal with this project was to create a search engine that researchers can easily use to scour the deep web for polar-related information. We also developed many visualization tools using D3 that are integrated within the search engine to simplify the results. Check out the <a href="http://irds.usc.edu/polar.usc.edu/">website</a> and the <a href="https://github.com/USCDataScience/polar.usc.edu">codebase here</a>.

#### Google web crawler
Google is the most used search engine in the world. I wanted to better understand how the search engine crawled through websites, which motivated this project.

The project was a mainly a test of understanding various algorithms and data structures such as DFS, graph theory, crawling policies, and filtering. Check out my implementation <a href="https://github.com/luuj/Web-Parser">here</a>.



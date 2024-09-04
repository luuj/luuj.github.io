---
title: Projects
subtitle: What I've been working on lately.
description: Projects I am working on
featured_image: /images/portraits/projects.webp
---



#### Correlation between surrogate endpoints and overall survival in cancer trials
Overall survival (OS) is the most common outcome used to determine effectiveness of new drugs for cancer. However, OS may be difficult to measure due to longer survival, issues with follow-up, treatment crossover, and successive lines of therapy. The use of surrogate endpoints, another indicator used in place of OS to judge efficacy, is appealing to investigators as it permits shorter trial duration, smaller patient cohorts, and may even allow for single-arm trial designs. Two common surrogate endpoints include progression-free survival (PFS) and objective response rate (ORR).

However, it is difficult to determine if PFS and ORR are valid surrogates for OS. Furthermore, this relationship changes depending on the type of cancer and intervention. To quantify the validity of these surrogates, we establish a clear relationship between the three endpoints using Prentice criteria. We explore several correlation coefficients (Pearson's, Spearman's Rho, Kendall's Tau, Harrell's C-index) and apply a variety of models to explore the relationship between PFS, ORR, and OS for several indications of cancer. 

#### Hierarchical models for longitudinal clustered semi-continuous data subject to mortality
During the COVID-19 pandemic, nursing homes were at the forefront of the response due to the frail nature of their population. Two key markers for quality of care in nursing homes discussed were costs and healthcare utilization. However, this type of data often follows a semi-continuous distribution consisting of a mass of zero values and a long right tail. This distribution introduces challenges in both model fitting and interpretation. Furthermore, residents of nursing homes are at high risk of mortality which acts as a competing risk. We developed a novel Bayesian hierarchical discrete time model for analyzing clustered and/or longitudinal semi-continuous data truncated by death. The model jointly captures the semi-continuous nature by modeling the probability mass at zero and skewed cost separately and combines it with a discrete time framework for semi-competing risks. 

We demonstrate the applicability of this novel model first through simulation and then by examining factors longitudinally associated with cost and health care utilization in and across nursing homes using nationally collected data from CMS. 

#### Measuring performance for costs in nursing homes 
Expanding on our hierarchical discrete-time model, we wanted to create a quantifiable measure of performance for clustered longitudinal semi-continuous data subject to mortality. Comparing and understanding nursing home costs is essential for families, policymakers, and healthcare providers. These costs are a significant component of financial planning for aging individuals, and the rising demand for long-term care due to an aging population places a substantial economic burden on public and private healthcare systems. However, several statistical issues must be considered when analyzing these data such as the semi-continuous distribution and semi-competing risk of death. We propose several metrics for profiling nursing homes in this project. We validate our metrics through simulation and then applied them to profile nursing homes on the basis of 90-day costs and mortality for nursing homes in Massachusetts and California using nationally collected data from CMS. 

#### Comparing methods for multiple-period cluster-randomized crossover trials
CRTs are becoming more commonly used to assess the effectiveness of health interventions; however, they are often designed with a small number ($< 10$) of clusters. It is unclear which statistical methods are optimal in this extreme scenario, as common approaches typically assume for more than 40 clusters. More complex designs such as the multiple period cluster randomized crossover trial (MPCRCT) can be used to mitigate issues caused by a small number of clusters, but little work has been done on analyzing their properties in this setting. This project looks at the effectiveness of generalized linear mixed models (GLMM) and generalized estimating equations (GEE), along with their corresponding small sample variance corrections, for MPCRCTs with fewer than 10 clusters. Results of this simulation trial will be used as guidance for MI-VACUNA, an ongoing MPCRCT examining the effectiveness of motivational interviewing on vaccine hesitancy at two Boston community health centers.

#### Motivational interviewing for vaccine uptake in Latinx adults
Prior to the COVID-19 pandemic, the WHO declared vaccine hesitancy, defined as a delay in the acceptance or refusal of vaccination despite availability of vaccination services, as one of the top 10 threats to global health. Today, despite massive recent and ongoing global efforts, vaccine hesitancy remains a major threat.

This project proposes to address vaccine hesitancy with a novel intervention that integrates evidence-based motivational interviewing (MI) into behavioral health (BH) services, coupled with electronic prompting, and vaccination access at the point of care. As a collaboration between Boston College, Harvard University, and East Boston Neighborhood Community Health Center, we will conduct a multiple-period cluster-randomized crossover trial within four programs at EBNHC. This trial will test the effectiveness of MI and BH interventions on COVID-19 vaccine uptake among Latinx adults and examine theory-based elements of vaccine hesitancy on the causal pathway between the intervention and vaccine uptake.

#### Duration of viral shedding and culture positivity with post-vaccination breakthrough delta variant infections
Isolation and distancing practices are fundamental elements of COVID19 epidemic control. However, the CDC currently recommends only 5 days of quarantine after a positive test. We were interested in whether this recommendation should be re-extended to 10 days.

For this study, we collected longitudinal viral load, viral culture samples, and CT values from Massachusetts General Hospital employees who tested positive for SARS-CoV-2. For our analysis, we adjusted for covariates including variants of the virus (original, delta, omicron) and vaccine status. We determined that the previous CDC recommendation of 10 days was needed. Check out our <a href="https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8855795/">paper</a> and <a href="https://github.com/luuj/SARS-CoV-2-Infection-Time">analysis code</a>.

#### Prevalence, incidence, and reversal pattern of childhood stunting from birth to age 2 years in Ethiopia
Although there has been a reduction in stunting (low height/length for age), the prevalence of malnutrition in Ethiopia is still high. Child growth patterns and estimates of stunting are needed to determine vulnerabilities and potential for recovery. We collected longitudinal data to determine the prevalence, incidence and reversal of stunting among children aged 0-24 months. Overall, the evidence from this study highlights a chronically malnourished population with much of the burden driven by growth faltering during the neonatal periods as well as after 6 months of age. To end all forms of malnutrition, growth faltering in populations such as that in young children in Amhara, Ethiopia needs to be addressed. Check out the HaSET project <a href="https://www.hsph.harvard.edu/haset/">here</a> and our <a href="https://jamanetwork.com/journals/jamanetworkopen/article-abstract/2814235">paper</a>.

#### Determinants of social risk screening and response equity in community health centers

Social determinants of health (SDH) include factors such as age, race/ethnicity, sex, language, comorbidities, cultural group membership, and stress. In collaboration with Caring Health Center and the Implementation Science Center for Cancer Control Equity, we want to analyze the role that SDH play in health inequity. 

The data was collected in electronic health record (EHR) format. However, this introduces the statistical complexity of incomplete / missing data. We want to develop methods that acknowledge the complexity and heterogeneity of the incomplete / missing EHR data, specifically in regard to SDH factors. Check out the analysis code for the project <a href="https://github.com/luuj/Caring-Health-Study">here</a>.

#### A simulation evaluation of the effectiveness and usability of the 3+3 design for phase I clinical trials
Before a drug can be introduced to market, it needs to undergo extensive testing. The first stage of this testing procedure is the phase I clinical trial, where drugs are tested for toxicity and the correct dosage. Currently, the most common design for phase I clinical trials is the 3+3.

Supervised by Susan Groshen of USC Norris Cancer Center, I wanted to compare the 3+3 to more modern methods at evaluating dose limiting toxicity and maximum tolerated dose. We found that despite the lack of statistical theory backing the 3+3, it performed very well when compared to the continual reassessment method, several Bayesian methods, and the rolling 6. Additionally, its simplistic implementation was more desirable for researchers. Check out <a href="https://www.proquest.com/openview/88a141f4bfd493b69231606fc30a02cb/1?pq-origsite=gscholar&cbl=18750&diss=y">my paper here</a>.

#### Improving the SEIR model for analyzing COVID19 spread
The SEIR (susceptible, exposed, infectious, recovered) model is commonly used to model infectious disease spread. In a recent paper by <a href="https://www.nature.com/articles/s41586-020-2554-8">Hao et al</a>, they propose expanding this model by appending 3 transition states: presymptomatic infectious, unascertained infectious, and isolation in hospital. 

Although the model was effective in predicting how COVID19 would spread through Wuhan, China, we wanted to improve on their implementation. Within their Metropolis-Hastings step, we introduced a relatively new algorithm called DRAM (Delayed Rejection Adaptive Metropolis), allowing for more flexibility and adaptability of the algorithm. This allowed us to increase simulation speed significantly (from 1103 to 593 seconds) while not affecting statistical performance. See our implementation, proposal, and presentation <a href="https://github.com/luuj/Bayesian-Methodology/tree/main/SAPHIRE-master">here</a>.

#### Blinded sample size re-estimation
Sample size and power calculations are critical when designing a clinical trial. In the past, clinical trials only performed these calculations at the start of the trial; however, researchers have begun implementing more adaptive procedures recently. For example, trials are often stopped to monitor if the treatment being evaluated is efficacious enough, or if the trial should be stopped for futility. During this stage, a common method of adaptation is performing sample size re-estimation to ensure that the trial has enough power to detect a difference between treatments.

For this project, I was tasked to perform sample size re-estimation for the <a href="https://www.thelancet.com/journals/landia/article/PIIS2213-8587(19)30346-8/fulltext">Long-term Odanacatib Fracture Trial (LOFT)</a>. Furthermore, I wanted to test through simulation how the type I error would be affected from changes to the sample size, power, accrual rate, and how many years patients would be followed up for. Check out my analysis and simulation code <a href="https://github.com/luuj/Recurring-endpoints---SS-reestimation">here</a>.

#### Comparing naive vs. robust methods for cluster randomized trials
Clustered randomized clinical trials are trials where patients are recruited in "clusters". These clusters are typically locations where individuals are likely to be correlated with one another, such as a school, nursing home, or village. These types of trials are becoming increasingly popular; however, methodology is still being developed.

When performing survival analysis on clinical trials, the proportional hazards Cox regression model is often used. The goal of this project was to determine if performing a naive analysis using the standard Cox model would be sufficient. I compared results from the naive model to the robust sandwich and randomization-based variants in 27 different scenarios. We discovered that despite not accounting for the correlation inherent in these clusters, the naive Cox model still performed just as well as the other two models. Check out the code and presentation for my project <a href="https://github.com/luuj/Clustered-RCT-simulations">here</a>.

#### Expanding access to home-based palliative care: A randomized controlled trial
Palliative care focuses on providing relief from the symptoms and stress of an illness. The goal is to improve quality of life for both the patient and the family. However, some patients and families prefer receiving treatment in the comfort of their own home compared to at the hospital. We were interested in whether or not home-based palliative care was as effective as hospital-based palliative care.

This was a 5-year clinical trial enrolling 1155 participants. My main tasks involved managing confidential patient files sent from Blue Shield, creating surveys and scripts in the REDCap database, and recording/monitoring new inpatient referrals. I also created scripts to automatically create summaries of demographic information, ineligibility criteria, and patient concerns so that we could present them to the DSMB and funding agencies. Check out the <a href="https://pubmed.ncbi.nlm.nih.gov/31486727/">study</a> and my <a href="https://github.com/luuj/Palliative-care-clinical-trial">code here</a>.

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



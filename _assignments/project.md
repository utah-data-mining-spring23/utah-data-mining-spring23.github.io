---
title: Project
include_nav_home: true
---

# Project

The class project is an avenue for trying out ideas that you have seen in the class in a practical setting. Project groups should consist of 1-2 students. If your project had two members, your final report should explain what each of you did.  Ideally, the project idea could come from you and you should explore some new directions. It could be about something that you are interested in or working on already. Of course, we are willing to brainstorm about the project with you and offer suggestions. 

Irrelevant after the project proposals: **[This document](https://docs.google.com/document/d/1zPzgGtmRCDrjZISDDgyC4ORUeu_NdChupAs9GjgPD7Y/edit?usp=sharing)** is meant as a starting point for generating **project ideas** - you are welcome to explore topics beyond the ones outlined here. We encourage you to choose a topic of interest, read a few related papers, and think of possible extensions. Keep in mind some topics have more available data than others. [This website](https://exnlpdatasets.github.io/) collects datasets for Explainable NLP. 

## Questions to consider in choosing a topic

Projects do not need to be a standard model-driven task. Students are welcome to explore a range of types of projects including:
* New explainability method for an existing task               
* New evaluation of an explanability method                  
* Collecting human-authored explanations for supervision               
* Survey 
    * To evaluate such projects I’ll follow [TACL](https://transacl.org/ojs/index.php/tacl/about/submissions): "To meet the bar of originality and significance, surveys should be such that even experts in the domain covered will say “I learned something interesting from this paper."  They should thus not simply be a descriptive enumeration of the contents of papers, but draw broad themes and (importantly) provide new insights on the topic.  These insights should be major contributions of the submission."
    * See [Wiegreffe and Marasović (2021)](https://arxiv.org/abs/2102.12060) for an example            
* Formalization
    * See [Jacovi et al. (2021)](https://arxiv.org/abs/2010.07487) and [Jacovi and Goldberg (2020)](https://aclanthology.org/2020.acl-main.386/) for examples                         
* Replication                
    * Applying an existing model to a different domain or data set or modality                
    * e.g. Low resource NLP -- extend any of the papers below to a multilingual / low resource setting

Project proposal should be well-structured (✨ see below) with clear research questions relevant to the course. Questions to consider in choosing a topic: 
* What topics do I care about and/or have domain knowledge in?
* What new skills do I want to develop? Modeling/analysis/data collection/research survey project?
* What are available data sets?
* What are existing baseline models to compare against?
* What is the evaluation plan?
* What is the analysis/qualitative evaluation plan? 

✨ That said, we encourage you to work on risky projects! ✨ Think about these levels: 

1. **Structured:**
    * Task and data sets are well defined, can make rapid progress with existing NLP models
    * Work will likely not result in publication (maybe suitable for workshop venues), though it depends how good your model is!
2. **Semi-structured:**
    * Some prior work on task. Data exists but may not be well-formatted or easy to approach
    * Research questions are clear but exact formulation of task is not
    * Project will require creativity in structuring tasks and may result in publishable work
3. **Unstructured:**
    * Topic may be interesting, but research questions are unclear and hard to define
    * Not clear what the correct data set is, may need to create one
    * Could result in really great work, but will require substantial student effort (High risk high reward!)

All of them are fine, and you should pick whatever project type suits what you aim to achieve from this course. 

## Grading 

Your project is worth 50% of the class grade. This is broken down across the following milestones:

* **Form a project team and submit project team information (2.5pt).**
* **Submit a project proposal (10pt).** A document no longer than 2 pages, consisting of the following information (following "[Heilmeier Catechism](https://www.darpa.mil/work-with-us/heilmeier-catechism)"):
    * What are you trying to do? Articulate your objectives using absolutely no jargon.
    * How is it done today, and what are the limits of current practice? 
    * The survey of prior work doesn’t need to be complete, but you should include high-level information about how your problem has been approached in the literature. This will help you think about baselines to compare against in your experiments.
    * What is new in your approach and why do you think it will be successful?
    * A success can also be showing that a published method does **not** work on a new language, domain, culture, etc.
    * Who cares? If you are successful, what difference will it make? 
    * What are the risks?
    * What are the intermediate (Nov 3) and final "exams" (Dec 6) to check for success? 
    * You should describe here how you will evaluate your approach. 
    * For a data-driven project, you should describe the data that you have at hand. Ideally, you should have all the data that you need – or have a plan that will get you the data within the next couple of weeks.   
    * If you are working on a standard data set, there is probably a standard evaluation that has been followed in the literature. You could describe this.
    * For a survey paper, you can commit to saying that success is providing X number of new insights. 
    * A successful formalization provides a clearly articulated framework for an old concept.
* **Submit an intermediate status report (10pt).** Upload [here](https://drive.google.com/drive/folders/1ha_jKmwyfffNOZdno6VbBTrzx6PYzTug?usp=share_link). A max 2-page document that says what you have done on the project so far. You can use your project proposal and add at the end a new section for new content. The new content should be max 2 pages, not everything including your proposal. The report should describe:
    * The progress you have made towards your goal. (This cannot be just "We collected data".) (5pt)
        * You **must** include a link to a github repository for your project.
    * Details of your plan for rest of the semester (3pt)
        * Here you **must** integrate the feedback you received on your proposal, unless I just suggested you could do something but didn't give a signal it's crucial. 
    * Pointers to literature (2pt)
        * Here you should integrate the feedback you received on the literature. 
* **Presentation (12.5pt):** Upload a **pdf** [here](https://drive.google.com/drive/folders/1HIgZkF31ODPXIVBSPFH473hnxfF2Iwg9?usp=share_link). 
    * **All** presentations MUST be uploaded by **Tuesday, Nov 29, 9 AM**. 
    * Please check Canvas (Home > Project Presentations) to see when your presentation is scheduled. **If you can't present on that day, let me know immediately.** Everyone (including those who are scheduled for Thrusday) **will use the version of slides available in the drive on Tuesday morning** (I'll remove access to the drive on Tuesday). If you miss the deadline for uploading your slides you will loose all points.  
    * Every presentation has to be presented **max. 20' long**. There will be a hard stop. _Plan what you will say beforehand._   
    * Your presentation has to have the following structure:
        * Title slide with the project name, your name, and a link to your github repo. **(0.5 point)**
        * A _brief_ introduction to the project topic **(1 points)** and the research question written as a _concrete_ question (e.g., Does X improve Y?) **(1 point)**. Demonstrate why addressing this question is relevant: what does every possible answer to the question entail? **(1 points)** 
        * Describe your approach to answering the research question. **(2 points)** 
        * _Precisely_ describe your experimental setup: tasks **(0.5 point)**, dataset names **(0.5 point)** + their main characteristics **(0.5 point)**, and evaluation metrics **(1 point)**. 
        * Present your results with figures/tables that are well organized and labeled **(1 points)**. Walk us through how to read them (what's x-axis, what's y-axis, where are the baselines, where is your method, point where we can see every result you're commenting, etc.) **(1 point)** Discuss and interpret results in the context of your research questions.
        * Given your research question, what do you conclude from your results? **(1.5 points)**
        * Tell us what you would do differently and/or what would you do if you had more time. **(1 point)**
* **Submit a project report (15pt):** Upload [here](https://drive.google.com/drive/folders/1D5lTKslXLneDN5_rlN5shDxxxnJ59KZQ?usp=share_link). Try to structure it like a research paper.
    * What problem did you work on? Why is it interesting?
    * What have you done to address the problem? 
    * What ideas from the class did you use?
    * Provide your results and conclusions. 
    * What did you learn?
    * If you had much more time, how would you continue the project?
    * Notes:
        * Each of these components will be equally weighted in the report grade.
        * Points will be deducated if the report has many grammatical mistakes and poor coherence. 
        * If your project had two members, your report should explain what each of you did.


<!-- * Pre-proposal: A 1-2 paragraph document describing the focus area of the project and defining team members (Due 1/23) -->
<!-- * Proposal: (7.5%) A 2-3 page document (ACL format) containing a literature review, concrete problem definition, identification of baseline models, and ideas for final models. Sections should include Introduction, Related Work, Data, Baseline, Proposed Approach. Baselines should be clearly defined but do not need to be implemented yet (Due 2/25) -->
<!-- * Midterm Presentations: (7.5%) An in-class presentation of project and current progress. Presentation should include problem definition, baseline models and results, and description of proposed models (3/19-3/24) -->
<!-- * Final Report and Presentations: (15%) In-class presentations of the project will be held during the final week of class. A final project report will be due the following week. The final report should be formated as a standard research paper with appropriate sections (ACL format, 8 pages) (Presentations 4/28-4/30; Report due 5/8) -->
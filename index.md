---
layout: home
title: Deep Mining
nav_exclude: true
toc: true
seo:
  type: Courses
  name: Deep Mining
---

# {{ site.tagline }}
{: .no_toc .mb-2 }
{{ site.description }}
<br>
MoWe / 3-4:20PM, [L101 WEB](https://bit.ly/3wBNjzE); will be recorded
{: .fs-6 .fw-300 }

{% assign instructors = site.staffers | where: 'role', 'Instructor' %}
{% for staffer in instructors %}
{{ staffer }}
{% endfor %}

{% assign teaching_assistants = site.staffers | where: 'role', 'Teaching Assistant' %}
{% assign num_teaching_assistants = teaching_assistants | size %}
{% if num_teaching_assistants != 0 %}

{% for staffer in teaching_assistants %}
{{ staffer }}
{% endfor %}
{% endif %}


## Communication

We will use **Canvas** for **Announcements**, **Discussions** (for instance questions on homework, projects, material covered in class, schedule, etc.), **turning in Assignments and Project** components, and for **communicating grades**. Please use the discussion forum as the preferred medium for interacting with the instructor and the teaching assistants rather than emailing/messaging directly. 

The **schedule**, links to class **notes**, and links to **videos**, will be through **this website**.

Take advantage of the instructor and TA office hours. We will work hard to be accessible to students. Don’t be shy if you don’t understand something: come to office hours, send emails, or speak up in class!

## Description

Data mining is the study of efficiently finding structures and patterns in large data sets. We will focus on several aspects of this: (1) converting from a messy and noisy raw data set to a structured and abstract one, (2) applying scalable and probabilistic algorithms to these well-structured abstract data sets, and (3) formally modeling and understanding the error and other consequences of parts (1) and (2), including choice of data representation and trade-offs between accuracy and scalability. These steps are essential for training as a data scientist.

Algorithms, programming, probability, and linear algebra are required tools for understanding these approaches.

Topics will include: similarity search, clustering, regression/dimensionality reduction, graph analysis, PageRank, and small space summaries. We will also cover several recent developments, and the application of these topics to modern applications, often relating to large internet-based companies.

Upon completion, students should be able to read, understand, and implement ideas from many data mining research papers.

## Calendar

Calendar is **tentative and subject to change**.
More details will be added as the semester continues.

<table>
  <thead>
  <tr>
    <th>Week</th>
    <th>Date</th>
    <th width="20%">Theme</th>
    <th width="30%">Contents</th>
    <th width="13%">Work due</th>
  </tr>
  </thead>
  <tbody>
  {% for week in site.data.calendar %}
    {% for day in week.days %}
      <tr>
        {% if forloop.index == 1 %}
        <td rowspan="{{week.size}}">{{week.week}}</td>
        {% endif %}
        <td>{{day.date}}</td>
        <td>{{day.theme}}</td>
        <td class="cal-content">
          {{day.topics}}
          {% if day.slides %}
            <a href="{{day.slides}}" class="cal-content-link">[slides]</a>
          {% endif %}
          {% if day.readings %}
            <a href="{{day.readings}}" class="cal-content-link">[readings]</a>
          {% endif %}
        </td>
        <td class="cal-content">{{day.due}}</td>
      </tr>
    {% endfor %}
  {% endfor %}
  </tbody>
</table>


## Resources

* **MS Teams.** Course communication will be via MS Teams.  You should sign into using your uNID and join the "team" for the class by clicking on [this link](https://teams.microsoft.com/l/team/19%3ait66PgoRabiGRMhXIEr67O1_XTkjExhyqn3rxIf2vI81%40thread.tacv2/conversations?groupId=d69b57e3-80a0-4b92-88fb-a54bd9145bab&tenantId=5217e0e7-539d-4563-b1bf-7c6dcf074f91). It's also the preferred way of communicating with the instructor. Please note that discussion threads and emails are all considered to be equivalent to the classroom, and your behavior in all these venues should conform to the university’s student code.

* **Google Drive.** Course materials, including lectures, reading lists, etc., are in a
  [Google Drive folder](https://drive.google.com/drive/folders/13i2Sor2M7it72aGlMd87Iejw6fzqsBxI?usp=sharing) which has been shared with all students. You can access it (only) with your **@gcloud.utah.edu account**. 

## Assignments/Grading

There will be three components to course grades. There are 100 points overall.


* **[Project](assignments/project/) (50 points / 50%).**
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
    * **Submit an intermediate status report (10pt).** A two page document that says what you have done on the project so far. By this time, you should have interacted with the instructor about your project. The report should describe:
      * The progress you have made towards your goal. (This cannot be just "We collected data".) (5pt)
      * Details of your plan for rest of the semester (3pt)
      * Pointers to literature (2pt)
    * **Presentation (12.5pt):** Instead of the final exam, we will have a presentation of the projects in the class. More details as we go along.
    * **Submit a project report (15pt):** A document no longer than 8 pages, structured like a research paper.
      * What problem did you work on? Why is it interesting?
      * What are the important ideas you explored?
      * What ideas from the class did you use?
      * What did you learn?
      * Results (or for theoretical project, proofs)
      * If you had much more time, how would you continue the project?
      * If your project had two members, your report should explain what each of you did.
      * Each of these components will be equally weighted in the report grade.

* **[Paper readings and discussion](assignments/paper_discussions/) (30 points / 30%).**
    * 20pt: Submit discussion questions before class and participate regularly during class. Note that not every question gives you points (e.g., a question cannot be just "What's X?" where X is explicitly described in the paper.)
    * 10pt: Lead at least one discussion.
* **[Paper review](assignments/review/) (20 points / 20%)** Review ACL/EMNLP reviewing guidelines and write a review for a research paper in explainable AI.

Assignments, including discussion questions, have to be submitted **by 11:59pm (Salt Lake City time), unless stated otherwise.**

**Do not submit assignments via email.** Questions for paper discussion have to be submitted to MS Teams. We will announce how to submit other assignments soon.

### University of Utah grading scale

| Letter      | Scoring |
| ----------- | ----------- |
| A      | 100%-94%       |
| A-   | 93.9%-90%        |
|B+ |	89.9%–87%|
|B	|86.9%–84%|
|B-	|83.9% - 80%|
|C+	|79.9%–77%|
|C	|76.9%–74%|
|C-	|73.9% - 70%|
|D+	|69.9%–67%|
|D	|66.9%–64%|
|D-	|63.9% - 60%|
|E	|59.9%–0%|

<!-- * **Late policy.** Students will have 4 late days that may be used for HW assignments at any point during the semseter. Late days may not be used for project benchmarks. After all late days have been used, no credit will be given for homework submitted late. -->

### Late Policy

 All submissions should be made by the deadline. We will use the timestamp on Canvas/Teams as the submission time. Submissions, **except paper discussion**, will be accepted up to 24 hours after deadline, but will be assessed a 10% penalty. That is, if your submission is late and scores 90, then your actual grade will be 81=90-9. 
 
 Submissions will not be accepted 24 hours after the deadline. 
 
 **We will be strict about this policy: If the deadline is midnight and you submit the assignment at 12:01 AM, you will face the 10% penalty!**

### Cheating 

Collaboration is encouraged; cheating will not be tolerated.
    
*<center><u>Honor code for this class</u></center>*
 
> You are encouraged to discuss class materials with your peers. If you want you
> can form study groups because discussions help understanding. You are also
> welcome to discuss assignments.
> 
> However, you must write your own solutions and code and submit your
> own solution. Do not copy or ask for assignments from other students or the
> internet. Do not let someone else copy your submissions either.

If you are caught cheating once, you *will* receive a failing grade for that
submission. If you are caught cheating again, you will fail the class.
 
For projects, you are free to discuss the project with your classmates, but your
work should be your own.
 
For both assignments and the project, you should cite all sources that you refer
to. This includes personal communication, books, papers, websites, etc. Doing so
reflects academic integrity.

### No double dipping projects across multiple classes

You can not submit the same project to this class and another class that you may be taking at the same time. If you are doing related projects in two different classes, there may be some overlap (e.g. in code libraries, etc.), but they should not be identical. A project that is found to be double-submitted will receive zero credit. If you have questions about this policy, please contact the instructor.

## Diversity

It is our intent that students from all diverse backgrounds and perspectives be well-served by this course, that students' learning needs be addressed both in and out of class, and that the diversity that the students bring to this class be viewed as a resource, strength and benefit. It is our intent to present materials and activities that are respectful of diversity: gender identity sexuality, disability, age, socioeconomic status, ethnicity, race, nationality, religion, and culture. Your suggestions are encouraged and appreciated. Please let us know ways to improve the effectiveness of the course for you personally, or for other students or student groups.

## SoC Policies and Guidelines  

The class operates under the School of Computing's [policies and guidelines](https://handbook.cs.utah.edu/2019-2020/Academics/policies.php). Among other things, linked page provides information about the [academic misconduct policy](https://www.cs.utah.edu/docs/misc/cheating_policy.pdf) that we will adhere to. 

Also see the [College of Engineering guidelines](https://www.coe.utah.edu/students/current/semester-guidelines/) for information about appeals procedures, withdrawal procedures, and adding and repeating courses.

### University Drop/Withdrawal Policy 

Students may drop a course within the first two weeks of a given semester without any penalties.

Students may officially withdraw (W) from a class or all classes after the drop deadline through the midpoint of a course. A “W” grade is recorded on the transcript and appropriate tuition/fees are assessed. The grade “W” is not used in calculating the student’s GPA.

For deadlines to withdraw from full-term, first, and second session classes, see the U's [Academic Calendar](https://registrar.utah.edu/academic-calendars/index.php).

### University Plagiarism and Cheating Policy

It is assumed that all work submitted to your instructor is your own work. When you have used the ideas of others, you must properly indicate that you have done so.

Plagiarism and cheating are serious offenses and may be punished by failure on an individual assignment, and/or failure in the course. Academic misconduct, according to the University of Utah Student Code,

>...Includes, but is not limited to, cheating, misrepresenting one’s work, inappropriately
> collaborating, plagiarism, and fabrication or falsification of information...It also includes
> facilitating academic misconduct by intentionally helping or attempting to help another to commit
> an act of academic misconduct.

For details on plagiarism and other important course conduct issues, see the U's [Code of Student Rights and Responsibilities.](http://regulations.utah.edu/academics/6-400.php).

### Course Materials Copyright

**The Content is made available only for your personal, noncommercial educational, and scholarly use.** You may not use the Content for any other purpose, or distribute, post or make the Content available to others unless you obtain any required permission from the copyright holder. Some Content may be provided via streaming or other means that restrict copying; you may not circumvent those restrictions. You may not alter or remove any copyright or other proprietary notices included in the Content.
 
Please see the [Code of Student Rights and Responsibilities](https://regulations.utah.edu/academics/6-400.php), Section III.A.5 regarding the [use and distribution of class Content](https://regulations.utah.edu/academics/6-400.php) and materials. Section III.A.5. prohibits the following:
Sale or distribution of information representing the work product of a faculty member to a commercial entity for financial gain without the express written permission of the faculty member responsible for the course. (“Work product” means original works of authorship that have been fixed in a tangible medium and any works based upon and derived from the original work of authorship.)

### University Safety Statement 

The University of Utah values the safety of all campus community members. You will receive important emergency alerts and safety messages regarding campus safety via text message.

For more safety information and to view available training resources, including helpful videos, visit safeu.utah.edu.

To report suspicious activity or to request a courtesy escort, contact:

* [Campus Police & Department of Public Safety](dps.utah.edu)
* 801-585-COPS (801-585-2677)
* 1735 E. S. Campus Dr., Salt Lake City, UT 84112

### Wellness

** Note from the instructor:** Take care of yourself! As a student, you may experience a range of challenges that can interfere with learning, such as strained relationships, increased anxiety, substance use, feeling down, difficulty concentrating and/or lack of motivation. All of us benefit from support during times of struggle. There are many helpful resources available on campus and an important part of having a healthy life is learning how to ask for help. Asking for support sooner rather than later is almost always helpful. 

**University Statement:**

Your personal health and wellness are essential to your success as a student. Personal concerns like stress, anxiety, relationship difficulties, depression, or cross-cultural differences can interfere with a student’s ability to succeed and thrive in this course and at the University of Utah.

Please feel welcome to reach out to your instructor or TA to handle issues regarding your coursework.

For helpful resources to manage your personal wellness and counseling options, contact:

* [Center for Student Wellness](https://www.wellness.utah.edu)
  * 801-581-7776
  * 2100 Eccles Student Life Center, 1836 Student Life Way, Salt Lake City, UT 84112
* [Women's Resource Center](https://womenscenter.utah.edu/)
  * 801-581-8030
  * 411 Union Building, 200 S. Central Campus Dr., Salt Lake City, UT 84112 


### Addressing Sexual Misconduct

Title IX makes it clear that violence and harassment based on sex and gender (which includes sexual orientation and gender identity/expression) is a civil rights offense subject to the same kinds of accountability and the same kinds of support applied to offenses against other protected categories such as race, national origin, color, religion, age, status as a person with a disability, veteran's status or genetic information.

If you or someone you know has been harassed or assaulted, you are encouraged to report it to university officials: 

* [Title IX Coordinator in the Office of Equal Opportunity and Affirmative Action](https://oeo.utah.edu/)
  * 801-581-8365
  * 135 Park Building, 201 Presidents' Cir., Salt Lake City, UT 84112

* [Office of the Dean of Students](https://deanofstudents.utah.edu/)
  * 801-581-7066
  * 270 Union Building, 200 S. Central Campus Dr., Salt Lake City, UT 84112 
 
To file a police report, contact:

* [Campus Police & Department of Public Safety](dps.utah.edu)
* 801-585-COPS (801-585-2677)
* 1735 E. S. Campus Dr., Salt Lake City, UT 84112

If you do not feel comfortable reporting to authorities, the U's Victim-Survivor Advocates provide **free**, **confidential**, and **trauma-informed** support services to **students**, **faculty**, and **staff** who have experienced interpersonal violence.

To **privately** explore options and resources available to you with an advocate, contact:

* [Center for Student Wellness](wellness.utah.edu)
  * 801-581-7776
  * 328 Student Services Building, 201 S. 1460 E., Salt Lake City, UT 84112


### The Americans with Disabilities Act

The University of Utah seeks to provide equal access to its programs, services and activities for people with disabilities. 

All written information in this course can be made available in an alternative format with prior notification to the Center for Disability & Access (CDA). CDA will work with you and the instructor to make arrangements for accommodations. Prior notice is appreciated. To read the full accommodations policy for the University of Utah, please see Section Q of the [Instruction & Evaluation regulations](http://regulations.utah.edu/academics/6-100.php).

If you will need accommodations in this class, or for more information about what support they provide, contact:

* [Center for Disability & Access](disability.utah.edu)
  * 801-581-5020
  * 162 Union Building, 200 S. Central Campus Dr., Salt Lake City, UT 84112
  



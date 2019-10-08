# Computational Linguistics 1 (CMSC723, INST735, LING723), Fall 2019, University of Maryland

Computational linguistics (CL) is the science of doing what linguists
do with language, but using computers. Natural language processing
(NLP) is the engineering discipline of doing what people do with
language, but using computers. We'll cover both, though the emphasis
is on NLP. We will largely focus on machine learning-based approaches
to a wide variety of challenging problems in NLP, with an emphasis on
recent deep learning-based techniques. Class time and readings will
focus on techniques; homeworks will largely focus on using NLP techniques
to address socially relevant problems. A focus throughout the course
will be on bias and fairness in machine learning systems.

  - [Basic Course Information](#basic-course-information)
  - [Prerequisites](#prerequisites)
  - [Coursework and Grading](#cousework-and-grading)
  - [Course Project](#course-project)
  - [Class Policies](#class-policies)
  - [Course Schedule](#course-schedule)


___
## Basic Course Information

| | | |
| :--- | :--- | :--- |
| **Instructor** | [Hal Daumé III](http://hal3.name) (he/him) | [![Photo of Hal Daumé III](images/hal-small.jpg)](images/hal.jpg)
| **When** | T/R 3:30pm-4:45pm |
| **Where** | IRB 1116 |
| **TAs**<br/><br/><br/> | [Kianté Brantley]() (he/him)<br/> [Trista Cao]() (she/her)<br/> [Amr Sharaf](http://www.cs.umd.edu/~amr/) (he/him) | [![Photo of Kianté Brantley](images/kiante-small.jpg)](images/kiante.jpg) [![Photo of Trista Cao](images/trista-small.jpg)](images/trista.jpg) [![Photo of Amr Sharaf](images/amr-small.jpg)](images/amr.jpg)
| **Discussion &**<br/>**Homework** | [ELMS](https://umd.instructure.com/courses/1267356) |
| **Office Hours**<br/><br/><br/><br/> | Hal: Thr 1:45p-2:30p, IRB 4150<br/>Trista: Mon 4:00p-5:00p, IRB 4th floor, in front of 4105 <br/>Amr: Wed 10:00a-11:00a, IRB 4th floor, in front of 4105  |
| | |





___
## Prerequisites

The required prerequisite for this course in an undergraduate AI
course, though a machine learning course, an algorithms course, or
LING 689/889 (Computational Psycholinguistics) should be
sufficient. In particular, you should be able to:

- Program in python
- Use core unix commands ([backgound](http://www.stanford.edu/class/cs124/kwc-unix-for-poets.pdf))
- Function with foundational probability and statistics ([background](https://stanford.edu/~shervine/teaching/cs-229/refresher-probabilities-statistics))
- Apply essential linear algebra ([background](http://users.umiacs.umd.edu/~hal/courses/2013S_ML/math4ml.pdf))
- Implement and understand central machine learning techniques (e.g., [CIML](http://ciml.info) chapters 1-5 and 7)

If you cannot handle all of these things (and cannot pick them up quickly), you should expect to run into challenges in the course.




___
## Cousework and Grading

The components of grading are:

- Homework assignments (7% each, 35% total)
- Course project (35% total)
- Early exam (10%) and late exam (15%)
- In-class/elms participation (5%)

Final class grades will be assigned based on the following mapping, possibly with thresholds adjusted down (*but never adjusted up*):

| Score | Grade |&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;| Score | Grade |&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;| Score | Grade |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| | || >=94 | A || >= 90 | A- |
| >=87 | B+ || >=84 | B || >= 80 | B- |
| >=77 | C+ || >=74 | C || >= 70 | C- |
| >=67 | D+ || >=64 | D || >= 60 | D- |




During this course, you will have five homework assignments that include both *programming* and *written* aspects. The written aspects are largely designed to help you do the programming more efficiently, by working through some of the details of what you will implement. These assignments are to be completed *individually*, and will be graded individually (see "collaboration policy" below). The goal of these assignments are to ensure that you learn and can implement standard NLP techniques, and understand and process language data effectively. These are:

- [HW1: Distributional semantics and text categorization (no code hand-in)](homework/HW1)
- [HW2: Neural networks and word embeddings](https://ec2-35-173-35-134.compute-1.amazonaws.com:9443/)
- HW3: Data collection and evaluation
- HW4: Sequence labeling
- HW5: Encoder-decoder models with attention


You will also complete one, large, course project, in teams of 4-5 students (exceptions are possible). The goal of this project is to enable you to work on a more significant, potentially impactful, project dealing with natural language. See the [course project description](#course-project) for more information.

**Participation:** You are to participate actively in class or in the online discussions. If you participate online, every question you answer well will get you 1% credit (marked by "instructor approved answer"); every question you ask will get you 0.5% credit (marked as "good question" by the instructor or a TA). Asking/answering questions in class counts the same.

**Late-ness:** In general, nothing may be handed in late without prior approval. However, every student may use one "stuff happens" card for one homework deadline, and every team may use one "stuff happens" card for one project deadline. These cards give you an additional 48 extra hours at no penalty in grade.

**Score adjustments:** Everyone makes mistakes, including us on grading. If you handed something in and do not get a score for an assignment, or if you believe there is an error in grading (either a homework or exam or project), you may raise this issue with us within *one week* of when we hand back grades.


___
## Course Project

A substantial portion of your coursework is a team-based project. You will work in teams. We highly recommend interdisciplinary teams are; and because diverse teams often produce better outcomes than homogenous teams, we encourage you to reach out and work with people who aren't (yet) your friends. As a team, you will complete a project of your choosing throughout the semester. The topic of the course project is **open-ended**, though it must fulfill certain requirements (most notably, relevance to natural language processing or computational linguistics). This is your opportunity to put your NLP/CL knowledge to use in a project of your choosing.

There are several *deliverables* for the course project, with associated grade percentages:
- P1: Project brainstorming, pitch, and feedback (5%)
- P2: Survey of related work, and plans for data (5%)
- P3: Description of proposed approach and measures of success (5%)
- P4: Prototype/baseline implementation and initial results (5%)
- P5: Final write-up and presentation (15%)

Each team will be assigned one of the TAs with whom you should meet once before 12 Nov (the due date for P3). You should also meet with Hal once before Thanksgiving break. We will create a signup sheet early on in the semester; use your own judgment for when would be most useful for *you* to meet with us.

*Credit: Some ideas for course project implementation are from Walter Lasecki's course on [Social Computing Systems](https://web.eecs.umich.edu/~wlasecki/courses/socs_current/) and/or Chris Callison-Burch's course on [Crowdsourcing](http://crowdsourcing-class.org/project.html).*

___
## Class Policies

**Disability Support:** Any student eligible for and requesting
reasonable academic accommodations due to a disability is requested to
provide, to the instructor in office hours, a letter of accommodation
from the Office of Disability Support Services (DSS) within the first
TWO weeks of the semester.

**Laptops in Class:** It's been repeatedly documented in many studies
that if you can, you are likely better off not using a laptop in
class ([example study](https://www.nytimes.com/2017/11/22/business/laptops-not-during-lecture-or-meeting.html); h/t Jacob Eisenstein).
You can make your own decision, but if your laptop use is distracting
others, an instructor may ask you to cease using it (in particular,
please avoid using websites with popup videos and the like). 
Please reach out to any instructor if we can help.

**Academic Integrity:** Any assignment or exam that is handed in must
be your own work. However, talking with one another to understand the
material better is strongly encouraged. Recognizing the distinction
between cheating and cooperation is very important. If you copy
someone else's solution, you are cheating. If you let someone else
copy your solution, you are cheating. If someone dictates a solution
to you, you are cheating. Everything you hand in must be in your own
words, and based on your own understanding of the solution. If someone
helps you understand the problem during a high-level discussion, you
are not cheating. We strongly encourage students to help one another
understand the material presented in class, in the book, and general
issues relevant to the assignments. When taking an exam, you must work
independently. Any collaboration during an exam will be considered
cheating. Any student who is caught cheating will be given an E in the
course and referred to the University Student Behavior
Committee. Please don't take that chance---if you're having trouble
understanding the material, please let us know and we will be more
than happy to help.

**Anti-Harassment:** The open exchange of ideas, the freedom of
thought and expression, and respectful scientific debate are central
to the aims and goals of a this course. These require a community and
an environment that recognizes the inherent worth of every person and
group, that fosters dignity, understanding, and mutual respect, and
that embraces diversity. Harassment and hostile behavior are unwelcome
in any part of this course. This includes: speech or behavior that
intimidates, creates discomfort, or interferes with a person’s
participation or opportunity for participation in the conference. We
aim for this course to be an environment where harassment in any form
does not happen, including but not limited to: harassment based on
race, gender, religion, age, color, national origin, ancestry,
disability, sexual orientation, or gender identity. Harassment
includes degrading verbal comments, deliberate intimidation, stalking,
harassing photography or recording, inappropriate physical contact,
and unwelcome sexual attention. Please contact an instructor or CS
staff member if you have questions or if you feel you are the victim
of harassment (or otherwise witness harassment of others). (Adapted
from the [ACL Anti-Harassment Policy](https://www.aclweb.org/adminwiki/index.php?title=Anti-Harassment_Policy).)

**Web Accessibility:** The University of Maryland is committed to [equal access to Web content](https://www.umd.edu/web-accessibility). If you need to request Web content in an alternative format or have comments or suggestions on accessibility, contact itaccessibility@umd.edu. 

___
## Course Schedule

Note that readings and homeworks are to be completed *before* the class period on which they are marked. For instance, you should have completed reading TODO before class on 29 Aug, and you must hand in HW1 before class on 12 Sep.

Readings may be from:
* SLP3: Jurafsky and Martin, [Speech and Language Processing (3rd edition)](https://web.stanford.edu/~jurafsky/slp3/)
* CIML: Daumé III, [A Course in Machine Learning](http://ciml.info)
* NLP: Eisensten, [Natural Language Processing](https://github.com/jacobeisenstein/gt-nlp-class/blob/master/notes/eisenstein-nlp-notes.pdf)
* Neu: Neubig, [Neural Machine Translation and Sequence-to-sequence Models: A Tutorial](https://arxiv.org/pdf/1703.01619.pdf)

| Date | Topic | Reading | Deadline |
| :--- | :---  | :--- | :--- |
| T 27 Aug | [Introduction to computational linguistics](slides/01_welcome.pdf) |  | 
| R 29 Aug | [Distributional semantics](slides/02_distributional.pdf) | SLP3 6.2-6.5 | 
| T 03 Sep | Review: linear models and loss functions | CIML 7 | [OH Poll](https://www.when2meet.com/?8039682-QmEKZ)
| R 05 Sep | [Text categorization: linguistic features and evaluation](slides/04_representations.pdf) | SLP3 4.7,<br/>and [Stylometry §2,5](https://www.aclweb.org/anthology/N15-1010) |
| T 10 Sep | Bias and fairness in NLP systems | [Webinar](https://note.microsoft.com/MSR-Webinar-Machine-Learning-and-Fairness-Registration-LIVE.html)* |
| R 12 Sep | [Computation graphs and backpropagation](slides/06_nnets.pdf) | NLP 3.1-3.3 | HW1
| T 17 Sep | [Word meaning as classification](slides/07_meaning.pdf) | SLP3 6.8-6.9,<br/>and [RacistAI](http://blog.conceptnet.io/posts/2017/how-to-make-a-racist-ai-without-really-trying/) | 
| R 19 Sep | [Data collection and annotation](slides/08_data.pdf) | [DataInNLP](https://www.aclweb.org/anthology/W17-1603),<br/>and [AnnCaseStudy](https://www.aclweb.org/anthology/W13-1703) | 
| T 24 Sep | [Measurement and validity](slides/09_measurement.pdf) | [Measurement](https://cehs01.unl.edu/aalbano/intro-measurement-r/validity.html),<br/>and [MeasurementCaseStudy, Sec "Reliability, Validity, ..."](https://onlinelibrary.wiley.com/doi/full/10.1111/j.1540-5907.2009.00427.x) | 
| R 26 Sep | [Crowdsourcing annotations](slides/10_crowdsourcing.pdf) | [CrowdsourcingNLP](https://www.researchgate.net/profile/Marta_Sabou/publication/315380496_Corpus_Annotation_through_Crowdsourcing_Towards_Best_Practice_Guidelines/links/5afc2040a6fdccacab199b4b/Corpus-Annotation-through-Crowdsourcing-Towards-Best-Practice-Guidelines.pdf),<br/>and [AnnMyths](https://www.aaai.org/ojs/index.php/aimagazine/article/download/2564/2468) | HW2
| T 01 Oct | **CLASS CANCELLED (Hal sick)** Multilinguality and linguistic variety | [TheBenderRule](https://thegradient.pub/the-benderrule-on-naming-the-languages-we-study-and-why-it-matters/),<br/>and [Elicitation, Sec 3](https://www.jstor.org/stable/pdf/40008189.pdf),<br/>and [optional: ActiveElicitation](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.180.8103&rep=rep1&type=pdf) | 
| R 03 Oct | *Early exam* |  | 
| T 08 Oct | [N-gram language models](slides/11_lms.pdf) | SLP3 3 | 
| R 10 Oct | Recurrent neural language models | SLP3 9 |
| T 15 Oct | Sequence labeling | CIML 17 | HW3
| R 17 Oct | Encoder-decoder models | Neu 7-7.3.1 | 
| T 22 Oct | *Project Pitches* | |  P1
| R 24 Oct | Contextual word embeddings | BERT??? | 
| T 29 Oct | *Catch-up* | | 
| R 31 Oct | Attention mechanisms | Neu  8 | P2
| T 05 Nov | Multilingual models | TBA | HW4
| R 07 Nov | Imitation learning | CIML 18 | 
| T 12 Nov | Program synthesis from language | TBA | P3
| R 14 Nov | *Late exam* |  | 
| T 19 Nov | Grounded semantics: language to actions | TBA | 
| R 21 Nov | Reading comprehension and question answering | TBA | HW5
| T 26 Nov | Bias in language systems | TBA | P4
| R 28 Nov | *Thanksgiving Break* |  | 
| T 03 Dec | Interpretation of neural models | TBA | 
| R 05 Dec | Machine translation | TBA | 
| T 17 Dec | *Project Poster Session (10:30a-12:30p)* |  | P5

\* The webinar link requires you to "register"; if this is an issue for you for any reason, please let any instructor know at least three days ahead of time so we can find a work-around.

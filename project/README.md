# CL1 Fall 2019 Course Project

The goal of the course project for [CL1 Fall 2019](https://github.com/hal3/cl1f19umd) is to give you an opportunity to demonstrate what you've learned over the semester and put it together in a unifying(ish) whole. You will work in teams of six or seven students. We highly recommend interdisciplinary teams; and because diverse teams often produce better outcomes than homogeneous teams, we encourage you to reach out and work with people who aren't (yet) your friends. The scope of the project (more details [below](#project-scope)) should be roughly "project plus two months of additional work = publishable paper." Of course, we don't expect every (or even most) projects to turn into papers, and that's certainly not how they'll be graded. We've given a few suggestions for [possible projects](Ideas.md) as well.

There are several deliverables for the course project, with associated grade percentages (percentages apply to your *entire* class grade, of which the project is 35%):

* [P1: Project brainstorming, pitch, and feedback](P1.md) (5%)
* [P2: Survey of related work, and plans for data](P2.md) (5%)
* [P3: Description of proposed approach and measures of success](P3.md) (5%)
* [P4: Prototype/baseline implementation and initial results](P4.md) (5%)
* [P5: Final write-up and presentation](P5.md) (15%)



## Project Scope

A good project is one that puts in place some sort of *baseline* for future development. For example: 

* **Replicability Study**: You may pick an NLP paper and reimplement it from scratch (in the sense that you don't use a ready-made implementation). If the authors made data available (or if it's on a public dataset), you can try to match the published results. This is a *replicability* study because you're literally trying to replicate their results with your own implementation.
  
* **Reproducibility Study**: You may pick an NLP paper, and try to reproduce it by changing some key aspects of the study. Data may be one such aspect. For instance, the original paper may have conducted experiments on English news data; you may wish to experiment with English social media data or Amharic news data. This would not necessarily involve reimplementing the approach (though you could do it if that would be educational): you are free to use a public implementation.
  
* **Extension Study**: You may pick an NLP paper that you find interesting, and extend the proposed approach in some interesting way. I would recommend only doing this if the data and implementation of the baseline is available online; trying to reimplement *and* extend would be more work than may be appropriate for a course project.
  
* **Meta-Analysis**: You may pick a few (three to five) NLP papers all on the same topic and do a meta-analysis of that area. Note that this is *not* just writing a survey. You should pick papers for which public implementations exist, and then do a head-to-head comparison of those approaches. A good meta-analysis will not just report how they do, but how they differ and how they compare and contrast, both qualitatively and quantitively.

*(Side-note: on replicability vs reproducibility, see [Drummond, ICML WS 2009](http://cogprints.org/7691/7/ICMLws09.pdf), but don't be scared away from a replicability study as a course project as a result of reading that.)*

You can also do a project that doesn't nicely fit into one of these categories; these are mostly there to help you think and formulate what you'd like to do.

**Use of public code:** No matter what type of project you do, there will be the question of: what about public implementations? Many papers these days now come with implementations that you can clone off of github (or elsewhere) and run yourself (some either come dockerized for you). Regardless of what type of project you do, you should feel free to use whatever public code you wish. If you want to reimplement things yourself for educational purposes, great. If you want to almost exclusively use other people's code, great. However, from a grading/assessment perspective, the less you implement, the more we expect in terms of analysis and discussion (and vice-versa). So if you really want to work on analysis stuff, take open source code. If you really want to work on implementation, write it yourself. Both are completely fine.


## Credits

Thanks to Walter Lasecki for his [SOCS class project](https://web.eecs.umich.edu/~wlasecki/courses/socs_current/) description, from which this is adapted.

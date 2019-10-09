## Project Ideas for CL1 Fall 2019 Project

For the [course project](README.md) for [CL1 Fall 2019](https://github.com/hal3/cl1f19umd), we give some project ideas that you're free to take completely, to use as inspiration, or to discard entirely. Some of these are unabashedly based on prior work by folks in the [UMD CLIP Lab](http://clip.umiacs.umd.edu); that's mostly because this is work that we're familiar with--don't shy away from things from elsewhere, we won't give extra credit points for picking a CLIP-related topic :P. These are listed alphabetically. Some are more or less fleshed out than others; such is the nature of things.... feel free to also take inspiration from some but not to do exactly what is suggested.

1. **Counterfactual Data Augmentation for Coreference Resolution**<br/>
  (Extension Study)<br/>
  Your TA Trista has recently finished a study of gender bias in coreference resolution systems (and human annotations), in particular the degree to which they are (not) able to adequately handle third person pronouns other than he/she and perform poorly for people who use singular-"they" or neopronouns for reference. (The data from HW3 is based on this study.) However, we have ways of doing counter-factual data augmentation (basically taking existing data and making new data that covers cases not covered by the original data). The goal of this project would be to retrain existing coreference systems using this data augmentation to see if their performance can improve. Given sufficient time, you could also try extending the models to better capture various anaphoric phenomenon where the models still do not perform well.

1. **Do It Not On English**<br/>
   (Reproducability)<br/>
   Very similar to "pick a paper you like," but add to it "and do it on a langauge other than English." (Assuming the original paper evaluated on English.) There's a good chance this will require data collection, which is fine so long as you have a good plan for how to do that.

1. **Identification of Translator**<br/>
   (Extension)<br/>
   It's [been shown recently](https://arxiv.org/pdf/1805.07697) that it's possible to identify with high accuracy, given a sentence in one language and its translation into a second, what was the direction of translation. A related question is: can we identify *who* did the translation? This is interesting because translators usually have a fair degree of autonomy in how they translation (translation *is* a creative process, after all), and each has their own style. It's an open question whether this style can be captured when the authors (translators) are constrained as much as they are in a translation setting. This would involve collecting a dataset (Global Voice is a good place to look!) and training a system to do authorship attribution. (Idea credit: Marine Carpuat)

1. **Language to Code**<br/>
  (Replication Study or Extension Study)<br/>
  Later in class, we will discuss models for mapping language to executable code. Together with colleagues from Cornell, CLIP grad study [Chen Zhao](http://users.umiacs.umd.edu/~chenz/) has put together a nice dataset together with a model that generates the code in a tree-based manner. One option would be to replicate this (or an alternative) model, perhaps implementing it yourself from scratch. Another possibility would be to extend the [human in the loop parsing](https://www.aclweb.org/anthology/D16-1258/https://www.aclweb.org/anthology/D16-1258/) paper we discussed to the code setting.

1. **Lottery Tickets in Embeddings**<br/>
  (Extension Study)<br/>
  There is a recent ["Lottery Ticket" hypothesis](https://arxiv.org/pdf/1803.03635) that suggests that the reason that really big neural networks work is because upon initialization, some of the randomly initialize parameters "win the lottery" and happen to be initialized in a good location. The paper proposes a clever procedure to validate this hypothesis. Can you extend this technique to word embeddings? That is, do we really need 1024-dimensional word embeddings, or are they just that big because we need 1024 dimensions in order for 100 of them to be "lucky."

1. **Measurements of Bias in Language**<br/>
  (Meta-Analysis or Reproducibility Study or Extension Study)<br/>
  There are now three high profile ways of measuring bias in language: the original subspace method (Boloukbasi et al.), the "Lipstick on a Pig" approach (Gonen & Goldberg), and the implicit association test approach (Calyskan et al.). (There are more; we're happy to provide pointers.) You could implement these, or find implementations, and do a meta-analysis of what each captures and what each misses, possibly framed from the perspective of measurement models.<br/><br/>
  You could also do a reproducibility study by thinking about how to extend such approaches to other languages, or to other theories of gender beyond the trans-exclusive ones used so far. There's been some work on other languages (e.g., [McCurdy & Serbetci](http://anacode.de/wordpress/wp-content/uploads/2017/06/mccurdy_grammatical_gender.pdf), [Sun et al.](https://arxiv.org/abs/1906.08976)), but the most interesting cases are possibly extensions to language that realize gender in different ways. How robust are these approaches on other languages?<br/><br/>
  Alternatively, you could do an extension study to look at topics other than gender bias. These methods have also been used to look at other sorts of bias along the lines of race (class reading), age (Díaz et al.), and religion (only informally as far as I know). You could consider other axes and think of ways to measure them. For instance, [Leah Findlater](http://faculty.washington.edu/leahkf/) suggested recently looking at detecting bias around how language reflects how people talk about disability (note: this may have been done, I'm not 100% sure).

1. **Non-monotone Sequence Generation**<br/>
   (Reproducibility or Extension or Meta-Analysis)<br/>
   There have been [several](https://arxiv.org/pdf/1902.01370) [papers](https://arxiv.org/pdf/1902.03249) [recently](https://arxiv.org/pdf/1902.02192) (that last one by TA Kiant&eacute;!) that propose to do langauge generation in a machine-learned order, rather than simply left-to-right (or right-to-left). You could (a) compare these in a meta-analysis; (b) do a "not on English" study, in particular on languages with freer word order, to see if these methods behave substantially differently; (c) extend these methods based on linguistic knowledge about the grammar of the respective languages (perhaps by using typological information).

1. **Pick A SemEval Task**<br/>
   (Various)<br/>
   The [SEMEval 2019](http://alt.qcri.org/semeval2019/index.php?id=tasks) tasks have been published; pick one and participate in the shared task!

1. **Searching for a Good State Machine**<br/>
   (Extension)<br/>
   Many prediction tasks in NLP involve producing discrete graph-like output structures (trees for parsing, graphs for semantic parsing, etc.). Most of the popular efficient algorithms for these approaches are essentially search processes over relatively simple state machines (e.g., [shift/reduce dependency parsing](https://www.youtube.com/watch?v=f5-hTA9hA3)). There are several popular such machines, but many possibilities that have not been explored. One could define an abstraction notion of a search space of possible machines (e.g., that involve things like stacks, buffers, arcs, etc.) and then and objective function over those (e.g., how good is greedy search on linguistic data? how easy is it to learn a good parser?) and use a discrete optimization search technique (e.g., [tabu search](https://en.wikipedia.org/wiki/Tabu_search)) to optimize the parsing *algorithm*. (Idea credit: Tim Vieira)

1. **What Are These Representations Encoding?**<br/>
  (Replication Study or Reproducibility Study or Extension Study)<br/>
  There have been many papers proposing ways to discover what is actually encoded in word representations (much of this in the context of static embeddings; some more recently with contextual embeddings), for instance by creating linguistically informed probes and seeing whether embeddings can be used to predict the correct answers (e.g., [Ettinger et al.](https://www.aclweb.org/anthology/W16-2524/)). You could pick one of these papers and either replicate its findings, extend them to other sorts of checks (linguistic or otherwise). You could alternatively develop new measurements; for instance it might be interesting to look at sparse models, or otherwise explainable models (like [decision rule lists](https://www.nature.com/articles/s42256-019-0048-x)) to see if the relevant information is encoded in an easy to interpret way.

1. **Writing Error Detection/Repair**<br/>
  (Reproducibility Study)<br/>
  There has been a fair amount of work looking at ways to build useful tools for helping people use language better. One form of this that we've already talked about is grammatical error correction for English langauge learners (NUCLE). Another form of this that we will discuss is [spell correction](http://www.cs.cmu.edu/~jbigham/pubs/pdfs/2015/realcheck.pdf) or [text simplification](http://readabilityguidelines.wikidot.com/local--files/sentence-length/Simplify%20or%20Help%20Rello%20et%20al.pdf) for Spanish speakers with dsylexia. You could take some technique that we'll have covered in class, or something more complex, and apply it to one of these two problems. (Or, if you find other data that is interesting, to that. Or collect new data.)


## Welcome 

Welcome to the Corpus Studies workshop for the SMT Jazz Interest Group (2019).

Today we will:

- Discuss how corpus studies might be useful for your research. 
- Discuss the constraints and issues related to corpus studies.
- Look at the essential tools and datasets.

## Installation

- You might want to consider installing **git** if you don't already have it.
  There's a nice guide on how to do this on the [Humdrum
website.](http://www.humdrum.org/install/github/#installing-git)

## Some Reading

Broze, Y., & Shanahan, D. (2013). Diachronic Changes in Jazz Harmony A
Cognitive Perspective. Music Perception: An Interdisciplinary Journal, 31(1),
32–45.

Katz, J. (2017). Harmonic Syntax of the Twelve-Bar Blues Form. Music
Perception, 35(2), 165–192.

Norgaard, M. (2014). How Jazz Musicians Improvise: The Central Role of Auditory
and Motor Patterns. Music Perception: An Interdisciplinary Journal, 31(3),
271–287.

Salley, K., & Shanahan, D. (2016). Phrase Rhythm in Standard Jazz Repertoire: A
Taxonomy and Corpus Study. Journal of Jazz Studies, 11(1).

Shanahan, D., & Broze, Y. (2012). A diachronic analysis of harmonic schemata in
jazz. Proc. 12th Int. Conf. on Music Perception and Cognition and the 8th
Triennial Conf. of the European Society for the Cognitive Sciences of Music,
Thessaloniki, Greece, 23, 909–917.

## Introduction

Rather than beginning on a typically optimistic note, let's begin by talking
about what we won't be able to do in this brief, hour-long workshop:

- we **won't** be able to learn a programming language in two hours
- we **won't** even be able to learn about a single toolkit terribly well (be
  it music21, Humdrum, or anything else you might be interested in using).
- we **won't** be able to have a complete grasp on a broad interdisciplinary
  field that encompasses computer science, psychology, machine learning,
musicology, music theory, statistics, and data visualization (among others!).

But all is not lost! Hopefully in this all too brief window we will:

- formulate a research question
- build a corpus that will try to get at aforementioned research question
- begin to tackle the research question in either an empirical or a descriptive
  fashion (although these two terms aren't necessarily diametrically opposed)
- TBD
- world domination.


### Some questions we will be addressing today

- How might "distant readings" be employed in our research?
- What does it mean to operationalize something, and how skeptical should we be
  of the operationizations of others?
- What can we learn from global variables?

## What is a corpus study?

For the purposes of today's workshop, we might think of a corpus study as a
"distant reading", defined as:

- "a form of analysis that focuses on larger units and fewer elements in order
  to reveal patterns and interconnections through shapes, relations, models,
and structures." (Burdick, *et al.*, 2012)
- "a term that is specifically arrayed against the deep hermeneutics of
  extracting meaning from a text through ever-closer, microscopic readings."
(Burdick, *et al.*, 2012)
- "not just a “digitization” or “quickener” of classic humanities
  methodologies. It is, rather, a new way of doing research wherein
computational methods allow for novel sets of questions to be posed about the
history of ideas, language use, cultural values and their dissemination, and
the processes by which culture is made" (_ibid._)

For the purposes of today's workshop, let's define a corpus study as: _what we
do when we look at the relationships of music from a bird's-eye view_.


### Corpus Studies without Computers

Knud Jeppesen (1922, 1927) approached Palestrina's work in a "strictly
scientific spirit". 
- Work was done completely by hand.
- Toward the end of the dissertation, he a melodic idea and then cites the 143
  spots in Palestrina's output. 
- Elsewhere, he cites a cambiata figure and then lists 300 or more exemplars.

* Gjerdingen's Work in _Classic Turn of Phrase_
* Byros's (2009) dissertation on the *le-sol-fi-sol* motive in Beethoven.

Could we argue that Caplin's *Classical Form* and Hepokoski and Darcy's
*Elements of Sonata Theory* are also corpus studies? 

Their theories are constructed from the analysis of large collections of
pieces. Is that a corpus analysis?

### Why Corpus Studies?

- Analyzing the relationship of pieces to the larger whole allows for us to
  better understand relationships and context.
- All the cool kids are doing it.

### What Data is Available?


- The [iRealB Lead Sheet Corpus](iRb_v1-0.zip) (see Shanahan and Broze, 2012;
  Broze and Shanahan, 2013)

- [The Omnibook Corpus](omnibook_kern.zip ) (see Baker, Shanahan, Rosado, and
  Shanahan, 2016).

- Audio data is available via the Spotify API and other services.

### Audio Data vs. Symbolic Data

**Symbolic Data** is data encoded from a score. This can mean data encoded into
musicXML, MEI, Kern, or MIDI.

**Audio Data** is data taken directly from a recording. It can be taken from
something like Spotify (with the Spotify API) or it can be extracted with a
tool such as [Sonic Visualiser](https://www.sonicvisualiser.org/).

#### Symbolic Data

- PRO: Allows for the analysis of specific musical features, including
  scale-degree information, harmonic information, and meter.
- CON: Laborious to encode. It has to be done manually, meaning that your
  corpus will likely be a bit smaller.


#### Audio Data

- PRO: Most often extracted automatically, meaning you can get a lot more data.
- NEUTRAL: The "musical object" is not the score, but the performance.
- CON: Data extracted can be somewhat unreliable (beat finding, for example, is
  problematic; harmonies are very problematic), and often the metrics are
somewhat difficult to decipher, and the mechanics are often kept a trade secret
(what does danceability mean? Acousticness?).

- Operationalizing is "a process which is absolutely central to the new field
  of computational criticism, or, as it has come to be called, of the digital
humanities." (p.1)
- "A theory-driven, data-rich research program has become imaginable, bent on
  testing, and, when needed, falsifying the received knowledge of literary
study. **Of this enterprise, operationalizing, will be the central
ingredient.**" (p.13, emphasis added)

## Falisifiability

As humans, we are extremely good at coming up with narratives and reasons for
why something might be the case.

- Birds of a feather flock together.
- Opposites attract. 

It's worth making the distinction between:

- exploratory analysis
- hypothesis-driven analysis

While these exploratory studies can be useful, at some point we need to come up
with a way of minimizing our own ability to construct a narrative.

**This is where a falsifiable hypothesis comes into play.**

The most important thing to keep in mind is:

- _**What would it look like for me to be wrong?**_ 

One way to do this would be to construct an _a priori_ hypothesis. Using
_inferential statistics_, you could then test this hypothesis against a _null
hypothesis_ (in which there would be no significant difference between
something observed and chance, for example.)

- With descriptive statistics, we describe a sample of a population, makes no
  broad claims about how something relates to broader populations.
- With inferential statistics, we are using the sample we have to infer
  conclusions about the broader sample. 


Sometimes these lines can be a little blurry, at first. For example, we can
have a _directionless_ hypothesis, such as "these things are related", but not
necessarily saying if they're positively or negatively correlated.

# Final thoughts

- What questions might we have about a corpus?
- How might you go about asking a computer to find these things?

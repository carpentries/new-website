---
date: 2016-12-20
layout: page
subheadline: "Data in the Field"
title: How I Developed a Workflow for Success in Graduate School
teaser: ""
categories:
   - blog
comments: true
show_meta: true
tags: ["Skillshare", "Data Carpentry"]
authors: ["Marian Schmidt"]
redirect_from: /blog/schmidt/
--- 

**This post originally appeared on the [Data Carpentry website](https://datacarpentry.org)**

My home state of Michigan and the surrounding Great Lakes area cradles 20% of our planet’s freshwater resource and yet growing up
next to these ecosystems, I knew almost nothing about their biological inner workings.  Now, as a PhD student and environmental microbial ecologist, I explore the most abundant and amazing inhabitants of the
lakes in my backyard: the diverse communities of tiny microbes.  

When I started my PhD in 2012, my ecological skillset was based on a low-throughput method of discovering
who a few of the bacteria were in our environmental samples.  I would spend weeks doing molecular biology in the lab and
Sanger sequence up to 10 sequences to manually identify my bacteria through [NCBI blast](https://blast.ncbi.nlm.nih.gov/Blast.cgi). It would take me several weeks to
learn the identities of just a few of the bacteria in my samples.   

Instead of learning about a single microbe, I am now interested in the millions of microbes that contribute to the complex lake
bacterial community. My dissertation research questions include: How do so many species of microbes live together?  Who are all of
these microbes?  Where within freshwater lakes do these bacteria live? How do they contribute to the food web and biological processes
that happen within lake ecosystems?  

**Scaling up my science**  

A high-throughput approach is needed to answer these ecological questions. I isolate lake bacterial community DNA and RNA and sequence
it with Illumina sequencing, resulting in millions of sequences. A million times more data than I had before! It would take years to do
the manual work I had depended on earlier. I needed to learn how to scale up my analyses, match these sequences to a database, and
uncover interesting ecological patterns.  

I had to learn how to program. Already a graduate student, I had never taken a single class on programming or computer science!
How did this happen? How would I learn how to code in addition to the fundamentals of ecology and evolutionary biology?
I had a lot of catching up to do.  

**Developing my data analysis workflow**  

After 2 years of attempting to teach myself, with some progress, I enrolled in Dr. Pat Schloss’s semester-long [*Microbial
Informatics*](http://microbialinformatics.github.io/) class.  The class included many of the topics of Software and Data Carpentry (i.e. reproducible research, git/GitHub, and R).
It was in this class that I was introduced to the basics of programming and version control with git/GitHub for the first time.  At the end of the course, Pat invited the class to be helpers at the first ever Software Carpentry workshop at U of M that he was
co-organizing with Dr. Meghan Duffy. I took him up on his offer and decided to help out.  

Through Pat’s class and helping out at the workshop, I was introduced and empowered to use what is now my current data analysis
workflow: obtain millions of sequences, use the unix shell to quality filter and assign my sequences to their matching bacteria
using [mothur](https://www.mothur.org/), a program written in C++.  Next, I import large data files into R where I apply reproducible coding practices in
RMarkdown (this was so influential - I even wrote a tutorial) in which I do all of my analysis. While I work through my analysis,
I save and keep track of all my changes with git and GitHub using 5 main commands:
`git add &lt;file&gt;`, `git commit -n “message about the file`, `git push`, `git pull`, and `git status`.
(My remote copy of [my work on GitHub](https://github.com/marschmi) saved my data analysis two times when my computer died!) Once my analysis is finished, I add a README to my github page and add the link to the methods section of my current paper
([click here for an early example](http://marschmi.github.io/Final_PAFL_Trophicstate/)).  Therefore, if people reading my paper are curious about how I did my analysis or
how my figures were made, they can see the real deal and I am accountable to my science.  

**Expanding into other realms: remote, high performance computers & collaboration**   

I originally worked on my own laptop during my first dissertation project as I only had tens of samples, however,
my second dissertation project has ten times more samples! So, I now use remote, high performance computers to do
the heavy lifting of my research for me.  With help from the [SWC unix lesson](https://swcarpentry.github.io/shell-novice/), I mastered how to work with files using unix.
I submit the work to the remote computers, it runs the most computationally intensive steps of my work and when it is finished
I use [globus](https://www.globus.org/) to transfer the important files to my laptop.    

Building on the foundation above, I have started and am excited to evolve a new branch of my workflow: collaboration.
Now, I am beginning to [build collaboration](https://github.com/rprops/Mothur_oligo_batch) in my workflow to develop reproducible scripts that are useful for others in
similar situations (or me in the future).  To do so, I use git and GitHub to share and develop scripts with collaborators
that have overlapping research goals.  Together we can create [GitHub issues](https://guides.github.com/features/issues/) to remind ourselves of what needs to be done
or of dreams that we have for our work.  To suggest changes and have a conversation about what we are working on we can send
[pull requests](https://help.github.com/articles/about-pull-requests/) to each other. And who knows - maybe what we are working on could be helpful for others!  

**What I wish I would have known**

First, I wish that I had been told earlier in my career that **learning how to program is a fundamental skillset that all biologists
should have.**  Second, **don’t learn how to program alone.**  I tried it and it was less efficient than learning alongside others and
learning through teaching and helping in SWC/DC workshops. Search for workshops happening around you or contact local people who
are involved in SWC/DC.  If there’s no one geographically close,
[**sign up for a mentorship discussion**](http://pad.software-carpentry.org/instructor-discussion) and lean on those who are in
other locations.  This community is dedicated to sharing their erudition, excitement, and resources for those seeking to learn
this ever so important skillset.  

**Developing a community of learners**

Here at U of M, I am working with the University of Michigan’s Software Carpentry partner organization to develop a community
of instructors/learners and to host workshops throughout campus.  While our organization is still young, we have hosted several
workshops and are starting to grow more. Even last week, I attended a
[two half-day Python workshop](https://umswc.github.io/2016-12-14-umich/) taught by Byron Smith and
Jackie Cohen to learn how to use python with the Jupyter notebook.  This community is an immense resource and provides an opportunity
for all levels of expertise, a space to learn, grow, and depend on others while we develop programming proficiency.  

Academia can learn from the SWC/DC community.  The bottom-up design that SWC/DC uses empowers people at all levels to contribute,
teach, and learn.  Helping to host a workshop or submitting to the development of a lesson also provides a place for people to develop
collaborative, leadership, and teaching skills that can also help benefit people’s next career stages.  I am ever thankful to this
community!  

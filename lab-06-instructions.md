Lab 6: Individual Research Project
================
Jonathan Gilligan
Lab: Feb. 17; Report due Mar. 12.; Presentations Mar. 16

  - [Introduction](#introduction)
      - [Solo or Team Projects](#solo-or-team-projects)
      - [Choosing a Topic](#choosing-a-topic)
  - [Writen Report (Due Mar. 12)](#writen-report-due-mar.-12)
      - [Making PDF output from
        RMarkdown](#making-pdf-output-from-rmarkdown)
  - [Presentation (Mar. 16)](#presentation-mar.-16)

# Introduction

You have done several structured labs that provided opportunities to
learn about R, RMarkdown, and several different aspects of climate
science (data analysis and several computer models).  
For the next few weeks, you will have a chance to utilize the skills you
have learned thus far in lab to explore a research question pertaining
to your specific interests. This series of labs consists of a written
lab report in RMarkdown and a presentation to the class. For this
project, you will choose a question or idea pertaining to one of the
previous labs and explore the topic a deeper. This may consit of
exploring the “why” portion of previous questions that only asked you to
describe patterns in the data or it may be evaluating relationships
between other variables not assesed in prior labs. To answer your
question, you may use the any of the data from lab 2, the MODTRAN model,
the RRTM model, the GEOCARB model, or a combination thereof.

Please get your topic approved by either Professor Gilligan or Ms. Best
by Feb. 21.

The lab report for your project is **due Mar. 12 at 11:59 PM**.

## Solo or Team Projects

You may choose to do this project individually or with a partner as a
team effort. If you work with a partner, you may work together to design
the question, obtain and analyze data, make a team presentation, and
write a report together. We expect teams to include a note in the report
that indicates which member contributed what to the report (this does
not need to be super detailed and can say, “Alice and Bob designed the
experiment together. Bob wrote the code to run the models. Alice wrote
the code for the data analysis. Alice and Bob contributed equally to
writing the discussion and conclusions.”) This is similar to the
requirement at many research journals that co-authored papers include a
statement of what each author contributed.

## Choosing a Topic

For undergraduates, we recommend that you choose a topic from one of the
exercises that you did in labs \#2–5 and think of a new question along
the same lines as the questions that exercise asked. For graduate
students, we expect you to try something more ambitious than just simple
extensions of the questions from the lab exercises, but it is still fine
to take one of the lab exercises as a starting point.

If you want to do something really different than what we have done
previously in lab, that is fine. But check with one of us to make sure
your plan is appropriate and feasible (we don’t want you to bite off
more than you can chew).

**Be CrEaTiVe\!** Now is the time to really explore parts of the class
that you have found interesting and present your findings in a unique,
exciting way.

# Writen Report (Due Mar. 12)

Your report should be comprehensive, yet not overly verbose. One
recommendation for achieving this is to create an outline to organize
your thoughts before initializing writing and data analysis. The report
needs to include the following components:

  - Introduction
    
      - *Provide background information that frames the problem you are
        addressing. At the end of the introduction, the reader should
        understand exactly **what the problem is** that you are
        addressing and why that problem is **interesting** and
        **relevant** to the climate system.*

  - Methods
    
      - *Describe the methods for answering your question. The methods
        section should be written such that someone completely
        unfamiliar with your project could follow your steps and
        recreate your results.*
    
      - This section should contain the R code you use to do the
        analysis:
        
          - Getting data into R: download from the internet, read it in
            from files on your computer, run models, etc.
        
          - Process data to clean it up: use functions like `mutate`,
            `gather`, `summarize`, etc. to convert the data into a
            useful form.
        
          - Analyze data: anything you do to analyze the data, such as
            generating descriptive statistics like the mean or standard
            deviation, fitting linear models to get slopes (rates of
            change), etc.

  - Results
    
      - *Describe the results of your analyses. Include apropriate
        charts, tables, graphs, and other quantitative representations
        of data.*
    
      - This section should have R code for making graphs, tables, etc.

  - Conclusions/Discussion
    
      - *Discuss the implications for the results you found using data
        from your results section.*
        
          - Why are these results significant or interesting?
        
          - What data supports these conclusions?
        
          - What are the broader implications of these results?
        
          - From the results that you have found, what are the next
            steps to take in this line of research? What other questions
            have arisen as a result of your analyses?

  - Works Cited
    
      - *Include a works cited section to credit the research and
        thoughts that are not your own. Be sure to use citations
        throughout your report where necessary.*
    
      - We will post a separate document that explains how to do
        citations and bibliographies in RMarkdown.

Final reports are to be pushed to your Lab 6 Github repository *no later
than 11:59 PM on Mar. 12*. **You must push the .Rmd file *and* the
knitted PDF** to Github. A portion of your final report grade will
reflect effective use of R/RMarkdown/Github, the clarity and
succinctness of your writing, visual representations of data,
appropriate discussion of results, and insights into future analyses.

## Making PDF output from RMarkdown

To make PDF output from RMarkdown, you need to install a program called
“LaTeX” (pronounced “layteck”, rhyming with “tech”). I describe how to
do this on [“Tools”
section](https://ees3310.jgilligan.org/tools/#installing-latex) of the
class web site, but I will summarize here: The easiest way to install
LaTeX for RMarkdown is to use the `tinytex` package in R. To do this,
execute the following commands at the RStudio console:

``` r
install.packages("tinytex")
library(tinytex)
install_tinytex(extra_packages=c("mhchem", "mathptmx"))
```

This may take 5-10 minutes to complete, so you probably want to wait
until a time when you won’t need your computer for a bit before you do
it.

An alternative, but which is more involved and will use more space on
your disk, would be to install the [MikTeX package](https://miktex.org)
from [miktex.org](https://miktex.org). Instructions for doing this are
presented on the
[Tools](https://ees3310.jgilligan.org/tools/#installing-latex) section
of the class web site.

# Presentation (Mar. 16)

Presentations will be limited to five minutes per student. Allot
approximately 3.5 to 4 minutes for the presentation of your project and
approximately 1 minute for questions. Team projects will get five
minutes for each team member, and we expect you to coordinate so that
each member speaks for roughly equal time.

  - You can use Powerpoint to make your presentation, or if you are
    adventurous, you can use RMarkdown to make a presentation. I will
    post a separate document about how to use RMarkdown to make
    presentation slides.

  - A Powerpoint or PDF of your final presentation needs to be pushed to
    Github *no later than 2:10 PM on Mar. 16*.

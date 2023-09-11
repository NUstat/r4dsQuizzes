# r4dsQuizzes

r4dsQuizzes provides quizzes for R for Data Science (2e) by Hadley Wickham, Mine Çetinkaya-Rundel, and Garrett Grolemund. These interactive quizzes are made using `learnr` tutorials with exam adaptations from `tutorialExtras`. The goal of r4dsQuizzes is to provide a proficiency assessment with student mastery in mind. When a quiz is run, a set of questions will be randomly selected for the student to complete. At the end of the quiz the student will lock the quiz, download an html of their answers, and upload the html to a learning management system. After 24 hours, the 'retry button' will become active and the student will be able to take the quiz again with a new set of questions randomly selected. Each quiz allows for 3 attempts.

At this time exercises are not auto-graded and will need to be graded by an instructor or grader as there are often many ways to accomplish the exercise goal. Ideally, each student would be provided feedback on each attempt, however if you have a large class, resources may limit that ability and you might consider having each student only submit the attempt they would like to have graded.

# Installation

Install the latest version of r4dsQuizzes from GitHub with the remotes package.

```{r}
# install.packages("remotes")
remotes::install_github("NUstat/r4dsQuizzes", dependencies = TRUE)
```

# List of quiz tutorials

| Tutorial Name | Topics Covered                     | R for Data Science (2e) |
|---------------|------------------------------------|-------------------------|
| quiz-1        | Visualizations and Transformations | Chapters 1 - 3          |
| quiz-2        |                                    |                         |
| quiz-3        |                                    |                         |
| quiz-4        |                                    |                         |

# Running tutorials

There are two ways to run the tutorials. The recommended way to run a tutorial is to type the following line in the R console:

`learnr::run_tutorial("quiz-1", package = "r4dsQuizzes")`

This should bring up a tutorial in your default web browser. You can see the full list of tutorials by running:

`learnr::run_tutorial(package = "r4dsQuizzes")`

Alternatively, in Version 1.3 onwards after having executed `library(r4dsQuizzes)`, a list of tutorials appears in a tutorial tab (by default it will be in the upper-right pane). However, the print option is not executable if the tutorial is run through the tutorial tab.

# Submitting quiz

After completing each quiz, students can obtain their quiz in html format. Students can then upload the html to a learning management system like Canvas or Gradescope.

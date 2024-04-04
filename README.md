# DSLC Learning Statistics with R Book Club

Welcome to the DSLC Learning Statistics with R Book Club!

We are working together to read [_Learning Statistics with R_](https://learningstatisticswithr.com/) by Danielle Navarro (copyright 2019, released under a creative commons licence (CC BY-SA 4.0)).
Join the [#book_club-lsr](https://dslcio.slack.com/archives/C04FDL1HV7B) channel on the [DSLC Slack](https://dslc.io/join) to participate.
As we read, we are producing [notes about the book](https://dslc.io/lsr).

## Meeting Schedule

If you would like to present, please see the sign-up sheet for your cohort (linked below, and pinned in the [#book_club-lsr](https://dslcio.slack.com/archives/C04FDL1HV7B) channel on Slack)!

- [Cohort 1](https://docs.google.com/spreadsheets/d/1wUN-kBK83rWKXfJ1ubklXWtRCMEau8T4tAlWAGW8b6g/edit?usp=sharing) (started 2023-04-05): [Wednesdays, 10:00 CST/CDT](https://www.timeanddate.com/worldclock/converter.html?iso=20230809T150000&p1=24&p2=1440&p3=215&p4=155&p5=54) | [meeting videos](https://www.youtube.com/playlist?list=PL3x6DOfs2NGiuZtoxH4AMSs1ipevg0YFH)

<hr>


## How to Present

This repository is structured as a [{bookdown}](https://CRAN.R-project.org/package=bookdown) site.
To present, follow these instructions:

Do these steps once:

1. [Setup Git and GitHub to work with RStudio](https://github.com/r4ds/bookclub-setup) (click through for detailed, step-by-step instructions; I recommend checking this out even if you're pretty sure you're all set).
2. `usethis::create_from_github("r4ds/bookclub-lsr")` (cleanly creates your own copy of this repository).

Do these steps each time you present another chapter:

1. Open your project for this book.
2. `usethis::pr_init("my-chapter")` (creates a branch for your work, to avoid confusion, making sure that you have the latest changes from other contributors; replace `my-chapter` with a descriptive name, ideally).
3. `devtools::install_dev_deps()` (installs any packages used by the book that you don't already have installed).
4. Edit the appropriate chapter file, if necessary. Use `##` to indicate new slides (new sections).
5. If you use any packages that are not already in the `DESCRIPTION`, add them. You can use `usethis::use_package("myCoolPackage")` to add them quickly!
6. Build the book! ctrl-shift-b (or command-shift-b) will render the full book, or ctrl-shift-k (command-shift-k) to render just your slide. Please do this to make sure it works before you push your changes up to the main repo!
7. Commit your changes (either through the command line or using Rstudio's Git tab).
8. `usethis::pr_push()` (pushes the changes up to github, and opens a "pull request" (PR) to let us know your work is ready).
9. (If we request changes, make them)
10. When your PR has been accepted ("merged"), `usethis::pr_finish()` to close out your branch and prepare your local repository for future work.
11. Now that your local copy is up-to-date with the main repo, you need to update your remote fork. Run `gert::git_push("origin")` or click the `Push` button on the `Git` tab of Rstudio.

When your PR is checked into the main branch, the bookdown site will rebuild, adding your slides to [this site](https://dslc.io/lsr).

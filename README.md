# SWECOV.se

This site is built with [Hugo](https://gohugo.io/) using the [research-project-theme](https://github.com/adamaltmejd/research_project_theme). To build the site locally, make sure you have [Hugo installed](https://gohugo.io/getting-started/installing/) (extended version recommended) and run:

```bash
hugo serve
```

## Creating a new study page
To create a page for a new study, create a markdown file in the `content/research/` folder. Name the file as a stub of the title/shorttitle, as this will be the page url, e.g. `diabetes-risk-factor.md`. The markdown file should contain *fontmatter* with information about the study. Here is an example (taken from `content/research/covid-inequality.md`):

```md
---
title: "Inequality and COVID-19 in Sweden: Relative risks of nine bad life events, by four social gradients, in pandemic vs. prepandemic years"
status: 'Published'
date: 2023-11-09
subject: ['Inequality', 'Social policy']
paper_url: 'https://www.pnas.org/doi/10.1073/pnas.2303640120'
journal: 'Proceedings of the National Academy of Sciences'
authors:
    - 'Adam Altmejd'
    - 'Evelina Björkegren'
    - 'Torsten Persson'
    - 'Olof Östergren'
---

The COVID-19 pandemic struck societies directly and indirectly, not just challenging population health but disrupting many aspects of life. Different effects of the spreading virus—and the measures to fight it—are reported and discussed in different scientific fora, with hard-to-compare methods and metrics from different traditions. While the pandemic struck some groups more than others, it is difficult to assess the comprehensive impact on social inequalities. This paper gauges social inequalities using individual-level administrative data for Sweden’s entire population. We describe and analyze the relative risks for different social groups in four dimensions—gender, education, income, and world region of birth—to experience three types of COVID-19 incidence, as well as six additional negative life outcomes that reflect general health, access to medical care, and economic strain. During the pandemic, the overall population faced severe morbidity and mortality from COVID-19 and saw higher all-cause mortality, income losses and unemployment risks, as well as reduced access to medical care. These burdens fell more heavily on individuals with low income or education and on immigrants. Although these vulnerable groups experienced larger absolute risks of suffering the direct and indirect consequences of the pandemic, the relative risks in pandemic years (2020 and 2021) were conspicuously similar to those in prepandemic years (2016 to 2019).
```

- `title` is the title of the study (required)
- `shorttitle` is a shorter title for use in the research list if the real title is too long (optional)
- `status` should be either `'Published'` or `'Ongoing'`  (required)
- `date` is the publication date, only use for ongoing work if you want to manually adjust the sorting in the research list. If not set, date is generated automatically from the last time the page was updated.
- `subject` is a list of subjects. Note the syntax with `['<subject1>','<subject2>', ...]` (optional)
- `paper_url` is the url to the published paper or preprint (optional)
- `journal` is the journal where the paper was published (optional)
- `authors` is a list of all authors, in the order they appear on the paper, note syntax (required)

## Testing
During local development, make sure you have the depencies installed locally and remove the comments before the "replace" directives in `go.mod`. This will link the local modules for development.
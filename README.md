# Li Linye — Data Science Portfolio

This repository contains the source files for my CISC7204 data science portfolio. It presents a project that connects a research question with documented public data, reproducible Python analysis and readable visualizations.

## Portfolio Links

- [Open the portfolio website](https://mc65222.github.io/data-science-portfolio/)
- [View the analysis project repository](https://github.com/mc65222/data-science-project)
- [View the portfolio homepage source](index.md)

The website link uses the standard GitHub Pages address for this account and repository. It becomes available after Pages deployment; use the actual URL shown in this repository's Pages settings if it differs.

## About Me

My name is **Li Linye**. This portfolio documents my data science coursework and demonstrates how a data analysis project can be organized, reproduced and communicated through a public website.

**Technical skills demonstrated in the featured project:**

- Python programming and Jupyter Notebook
- Data cleaning and aggregation with pandas and NumPy
- Reading Excel workbooks with openpyxl
- Data consistency checks and reproducibility documentation
- Data visualization with Matplotlib
- Markdown documentation and website source preparation

## Featured Project

### Harassment and Bullying in U.S. Public Schools

**Research question:** How did reported harassment and bullying vary by basis in 2015–16, and how did the sex composition of reported students differ across categories?

**Project status:** Completed — local analysis, visualizations and documentation.

**Data source:** U.S. Department of Education, Office for Civil Rights, Civil Rights Data Collection (CRDC), 2015–16. The [official dataset catalog](https://catalog.data.gov/dataset/2015-16-harassment-or-bullying-by-basis-category-civil-rights-data-collection) identifies public access and a CC BY license. The figures are derived from seven aggregate Excel workbooks.

### Main Finding

The national table records **135,192 allegations**. Sex-based allegations form the largest category, with **55,579 allegations (41.1%)**. These are allegation counts rather than counts of unique students.

![Allegations by basis, showing sex-based allegations as the largest category](results/figures/01_allegations_by_basis.png)

Additional figures on the homepage compare reported and disciplined student counts as separate measures and show the sex composition of reported students within each basis. Female students make up **63.9%** of sex-based reported students; male students make up **63.5%** of race-based and **66.9%** of disability-based reported students. These composition shares are not population risk estimates.

### Main Limitation

Administrative records may reflect underreporting and differences in reporting coverage. Enrollment denominators are absent, so the analysis cannot establish bullying prevalence or compare population risks. Reported victims and disciplined students are different, unlinked groups; their ratio is not a case-resolution rate. A single historical year cannot establish trends or causation.

### Code and Reproducibility

The [project repository](https://github.com/mc65222/data-science-project) contains the Jupyter Notebook, dependencies, source workbooks, exported results and instructions for reproducing the analysis. This portfolio repository contains the website source and copies of the figures used by the site.

## Website Files

```text
data-science-portfolio/
├── README.md
├── index.md
├── _config.yml
├── _layouts/
│   └── default.html
├── assets/
│   └── style.css
└── results/
    └── figures/
        ├── 01_allegations_by_basis.png
        ├── 02_reported_and_disciplined.png
        └── 03_reported_students_by_sex.png
```

`index.md` is the website entry file. It uses the local Jekyll layout and stylesheet. The figure files must remain under `results/figures/` so the relative image links work.

## GitHub Pages Configuration

Publish this repository using **Settings → Pages** with:

- **Source:** Deploy from a branch
- **Branch:** main
- **Folder:** / (root)

After deployment, open the URL displayed in Pages settings and check the homepage, images and project repository link.

## Planned Improvements

Investigate reporting completeness, add compatible enrollment denominators and extend the analysis to other years. Collect classmate feedback on the project's purpose, main finding and limitation, then document an actual improvement with a descriptive commit.

## AI Assistance

OpenAI Codex assisted with the analysis code, documentation, notebook conversion and portfolio source. The student is responsible for reviewing the material and providing the required course AI declaration.

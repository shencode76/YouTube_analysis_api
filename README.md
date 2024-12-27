# 2024-dsan-5000-project

# Project: Unveiling the Secrets of Audience Engagement

This is a semester-long data science group project for my Data Science and Analytics class at Georgetown University when persuing Master degree.
Please find more details at [my website](https://yuxishen.georgetown.domains/portfolio_project/)

## Overview
This project focuses on the collection, preprocessing, and analysis of YouTube video data to extract meaningful insights. By utilizing the YouTube Data API, we systematically gather video metadata and analyze trends in content performance, audience engagement, and popularity. The project is structured to address key research questions using both supervised and unsupervised learning techniques.


## Features
- **Data Collection:**
  - Automated data collection from the YouTube Data API.
  - Metadata includes attributes like `viewCount`, `likeCount`, `duration`, and `topicCategories`.
  - Focus on English-speaking regions to maintain linguistic consistency.

- **Exploratory Data Analysis (EDA):**
  - Word cloud visualizations to analyze popular keywords.
  - Frequency plots and TF-IDF analyses for textual data.
  - Duration and engagement patterns across videos.

- **Supervised and Unsupervised Learning:**
  - Binary classification for predicting `popularity`.
  - Regression tasks for modeling `viewCount` and `likeCount`.
  - Cross-validation hyperparameter tuning
  - Clustering techniques to group videos by similarity.
  - Feature reduction by PCA and T-SNE.
  - Clustering videos using KMeans, DBSCAN, and Hierarchical clustering algorithms

## How to run our project
#### Clone the Repository:
```bash
git clone https://github.com/dsan-5000/project-YuxiShen1079.git
cd <root-of-this-project > 
# and then you can run each of the Jupyter Notebook in for each section
```

To run the project and navigate between sections, use:
```bash
quarto preview _site
```

## Data Storage:

If you want to take a look at our raw data and pre-processed data, please find them in the [Google Drive folder](https://drive.google.com/drive/folders/1R4t2YkfP8ainQQn9HT0QhGBYw1ruB1oK?usp=sharing) 


## Project Structure
directory tree:

```
.
├── README.md
├── _quarto.yml
├── _site
│   ├── assets
│   │   └── gu-logo.png
│   ├── index.html
│   ├── report
│   │   ├── pictures
│   │   │   ├── Video_duration_by_topic.png
│   │   │   ├── duration_popularity.png
│   │   │   ├── output.png
│   │   │   └── view_like_comment_corr.png
│   │   └── report.html
│   ├── search.json
│   ├── site_libs
│   │   ├── bootstrap
│   │   │   ├── bootstrap-icons.css
│   │   │   ├── bootstrap-icons.woff
│   │   │   ├── bootstrap.min.css
│   │   │   └── bootstrap.min.js
│   │   ├── clipboard
│   │   │   └── clipboard.min.js
│   │   ├── quarto-html
│   │   │   ├── anchor.min.js
│   │   │   ├── popper.min.js
│   │   │   ├── quarto-syntax-highlighting.css
│   │   │   ├── quarto.js
│   │   │   ├── tippy.css
│   │   │   └── tippy.umd.min.js
│   │   ├── quarto-nav
│   │   │   ├── headroom.min.js
│   │   │   └── quarto-nav.js
│   │   └── quarto-search
│   │       ├── autocomplete.umd.js
│   │       ├── fuse.min.js
│   │       └── quarto-search.js
│   └── technical-details
│       ├── data-cleaning
│       │   ├── closing.html
│       │   ├── instructions.html
│       │   ├── main.html
│       │   ├── methods.html
│       │   └── overview.html
│       ├── data-collection
│       │   ├── closing.html
│       │   ├── instructions.html
│       │   ├── main.html
│       │   ├── methods.html
│       │   └── overview.html
│       ├── eda
│       │   ├── instructions.html
│       │   ├── main.html
│       │   └── main_files
│       │       └── figure-html
│       │           ├── cell-11-output-1.png
│       │           ├── cell-12-output-2.png
│       │           ├── cell-13-output-1.png
│       │           ├── cell-14-output-1.png
│       │           ├── cell-15-output-1.png
│       │           ├── cell-5-output-1.png
│       │           ├── cell-6-output-2.png
│       │           ├── cell-7-output-1.png
│       │           └── cell-8-output-2.png
│       ├── llm-usage-log.html
│       ├── progress-log.html
│       ├── supervised-learning
│       │   ├── instructions.html
│       │   ├── main.html
│       │   └── main_files
│       │       └── figure-html
│       │           ├── cell-10-output-2.png
│       │           ├── cell-11-output-2.png
│       │           ├── cell-12-output-2.png
│       │           ├── cell-3-output-2.png
│       │           ├── cell-4-output-2.png
│       │           ├── cell-5-output-2.png
│       │           ├── cell-6-output-2.png
│       │           ├── cell-7-output-2.png
│       │           ├── cell-8-output-2.png
│       │           └── cell-9-output-2.png
│       └── unsupervised-learning
│           ├── instructions.html
│           ├── main.html
│           └── main_files
│               └── figure-html
│                   ├── cell-11-output-2.png
│                   ├── cell-11-output-4.png
│                   ├── cell-12-output-2.png
│                   ├── cell-12-output-4.png
│                   ├── cell-13-output-1.png
│                   ├── cell-13-output-3.png
│                   ├── cell-14-output-1.png
│                   ├── cell-14-output-3.png
│                   ├── cell-15-output-1.png
│                   ├── cell-15-output-3.png
│                   ├── cell-17-output-1.png
│                   ├── cell-17-output-2.png
│                   └── cell-9-output-1.png
├── assets
│   ├── gu-logo.png
│   ├── nature.csl
│   └── references.bib
├── build.sh
├── data
│   ├── processed-data
│   │   └── cleaned_data.csv
│   └── raw-data
│       └── youtube_data_raw.csv
├── index.qmd
├── index_files
│   └── mediabag 2
├── report
│   ├── pictures
│   │   ├── Video_duration_by_topic.png
│   │   ├── duration_popularity.png
│   │   ├── output.png
│   │   └── view_like_comment_corr.png
│   ├── report.qmd
│   └── report_files
│       └── mediabag 2
├── technical-details
│   ├── data-cleaning
│   │   ├── closing.qmd
│   │   ├── instructions.qmd
│   │   ├── main.ipynb
│   │   ├── main_files
│   │   │   ├── figure-html 2
│   │   │   └── mediabag 2
│   │   ├── methods.qmd
│   │   ├── methods_files
│   │   │   └── mediabag 2
│   │   └── overview.qmd
│   ├── data-collection
│   │   ├── closing.qmd
│   │   ├── instructions.qmd
│   │   ├── main.ipynb
│   │   ├── main_files
│   │   ├── methods.qmd
│   │   ├── methods_files
│   │   │   └── mediabag 2
│   │   ├── overview.qmd
│   │   └── overview_files
│   │       └── mediabag 2
│   ├── eda
│   │   ├── instructions.qmd
│   │   ├── main.ipynb
│   │   └── main_files
│   │       ├── figure-html 2
│   │       └── mediabag 2
│   ├── llm-usage-log.qmd
│   ├── progress-log.qmd
│   ├── supervised-learning
│   │   ├── instructions.qmd
│   │   └── main.ipynb
│   └── unsupervised-learning
│       ├── instructions.qmd
│       └── main.ipynb
└── xtra
    └── multiclass-portfolio-website
        ├── _quarto.yml
        ├── _site
        │   ├── images
        │   │   ├── 2024-10-14-16-56-34.png
        │   │   └── gu-logo.png
        │   ├── index.html
        │   ├── projects
        │   │   └── dsan-5000
        │   │       └── _site
        │   │           ├── about.html
        │   │           ├── index.html
        │   │           ├── search.json
        │   │           └── site_libs
        │   │               ├── bootstrap
        │   │               │   ├── bootstrap-icons.css
        │   │               │   ├── bootstrap-icons.woff
        │   │               │   ├── bootstrap.min.css
        │   │               │   └── bootstrap.min.js
        │   │               ├── clipboard
        │   │               │   └── clipboard.min.js
        │   │               ├── quarto-html
        │   │               │   ├── anchor.min.js
        │   │               │   ├── popper.min.js
        │   │               │   ├── quarto-syntax-highlighting.css
        │   │               │   ├── quarto.js
        │   │               │   ├── tippy.css
        │   │               │   └── tippy.umd.min.js
        │   │               ├── quarto-nav
        │   │               │   ├── headroom.min.js
        │   │               │   └── quarto-nav.js
        │   │               └── quarto-search
        │   │                   ├── autocomplete.umd.js
        │   │                   ├── fuse.min.js
        │   │                   └── quarto-search.js
        │   ├── search.json
        │   └── site_libs
        │       ├── bootstrap
        │       │   ├── bootstrap-icons.css
        │       │   ├── bootstrap-icons.woff
        │       │   ├── bootstrap.min.css
        │       │   └── bootstrap.min.js
        │       ├── clipboard
        │       │   └── clipboard.min.js
        │       ├── quarto-html
        │       │   ├── anchor.min.js
        │       │   ├── popper.min.js
        │       │   ├── quarto-syntax-highlighting.css
        │       │   ├── quarto.js
        │       │   ├── tippy.css
        │       │   └── tippy.umd.min.js
        │       ├── quarto-nav
        │       │   ├── headroom.min.js
        │       │   └── quarto-nav.js
        │       └── quarto-search
        │           ├── autocomplete.umd.js
        │           ├── fuse.min.js
        │           └── quarto-search.js
        ├── build.sh
        ├── images
        │   ├── 2024-10-14-16-56-34.png
        │   └── gu-logo.png
        ├── index.qmd
        └── projects
            └── dsan-5000
                └── _site
                    ├── assets
                    │   └── gu-logo.png
                    ├── collaborators.html
                    ├── index.html
                    ├── instructions
                    │   ├── expectations.html
                    │   ├── github-usage.html
                    │   ├── llm-usage.html
                    │   ├── overview.html
                    │   ├── quarto-tips.html
                    │   ├── topic-selection.html
                    │   └── website-structure.html
                    ├── report
                    │   └── report.html
                    ├── search.json
                    ├── site_libs
                    │   ├── bootstrap
                    │   │   ├── bootstrap-icons.css
                    │   │   ├── bootstrap-icons.woff
                    │   │   ├── bootstrap.min.css
                    │   │   └── bootstrap.min.js
                    │   ├── clipboard
                    │   │   └── clipboard.min.js
                    │   ├── quarto-html
                    │   │   ├── anchor.min.js
                    │   │   ├── popper.min.js
                    │   │   ├── quarto-syntax-highlighting.css
                    │   │   ├── quarto.js
                    │   │   ├── tippy.css
                    │   │   └── tippy.umd.min.js
                    │   ├── quarto-nav
                    │   │   ├── headroom.min.js
                    │   │   └── quarto-nav.js
                    │   └── quarto-search
                    │       ├── autocomplete.umd.js
                    │       ├── fuse.min.js
                    │       └── quarto-search.js
                    └── technical-details
                        └── data-collection
                            ├── instructions.html
                            ├── introduction.html
                            ├── main.html
                            └── methods.html

```
# Google Scholar Entry Collector

A Python script that collect publication information from a given google scholar
profile. It uses the [Python scholarly library](https://pypi.org/project/scholarly/).

## Use

To use it, replace the `scholar_url` in `collect_publications.py` with your
scholar URL, and run `collect_publications.py` with Python:

```bash
    python3 collect_publications.py
```

You should see something like that:

```bash
    User ID = Xix_ZHoAAAAJ
    User name = SungKu Heo


    2019 An insight into nanocellulo... Unknown Journal
    2019 A deep reinforcement learni... Energy and Buildings
    2020 Soft sensor validation for ... Control Engineering Practice
    2019 Hydrogen-based self-sustain... Energy Conversion and Management
    2021 Data-Driven Hybrid Model fo... IEEE Transactions on Industrial Informatics
    2021 A hybrid machine learning–b... Journal of Cleaner Production
    (...)
```

## Output

By default, publication information is written in a folder YEAR_NAME_JOURNAL,
located in `path = "./publications"`, to a file named `index.md` that can be read
with [Hugo](https://gohugo.io/) framework, just
like [my personal page](https://simongravelle.github.io). Feel free to clone and
adapt to your content.

Output looks like that:
```bash
---
title: "XRL-FlexSBR: Multi-agent reinforcement learning-driven flexible SBR control with explainable performance guarantee under diverse influent conditions"
date: 2024-01-01
publishDate: 2024-01-01
authors: ["SungKu Heo", "KiJeon Nam", "SangYoun Kim", "ChangKyoo Yoo"]
publication_types: ["2"]
abstract: "The sequencing batch reactor (SBR) process stands out for its small footprint and operational flexibility. However, the SBR process is highly nonlinear and subject to influent disturbances. In this study, we suggested an explainable multi-agent reinforcement learning (XRL) approach coupled with multi-agent reinforcement learning (MARL) and explainable AI (XAI); then, an XRL-driven flexible SBR control (XRL-FlexSBR) system was developed to conduct multivariate control the SBR process autonomously. Influent big datasets including biochemical oxygen demand (BOD) and total nitrogen (TN) were collected from the wastewater treatment plants (WWTPs) of South Korea. Then, the Gaussian mixture model was utilized to cluster the diverse influent conditions and the SBR mechanistic model was developed. A game abstraction method based on a two-stage attention network (G2ANET), one of MARL algorithms, was …"
featured: true
publication: "Journal of Water Process Engineering 2024 66 "
links:
  - icon_pack: fas
    icon: scroll
    name: Link
    url: 'https://www.sciencedirect.com/science/article/pii/S2214714424012236'
---
```
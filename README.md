# Overview

This repository contains the Python scripts used to download the raw
data underlying the analysis presented in:

Di Donato, F., Mannocci, A., Pecoraro, F., & Provost, L. (2026). *Mind
the Gap: From Policy to Practice at CNR. An Analysis of Career
Advancement Criteria in Light of the Agreement on Reforming Research
Assessment.* https://doi.org/10.5281/zenodo.18642800

The downloaded raw data were used to produce the supplementary material
accompanying the article, available at:

Di Donato, F., Mannocci, A., Pecoraro, F., & Provost, L. (2026).
*Supplemental material to the article "Mind the Gap: From Policy to
Practice at CNR. An Analysis of Career Advancement Criteria in Light of
the Agreement on Reforming Research Assessment"* (Version 1.0) \[Data
set\]. Zenodo. https://doi.org/10.5281/zenodo.18657087

------------------------------------------------------------------------

# Repository Structure

The repository includes two Jupyter notebooks that download official
public documents related to competitive selection procedures for career
progression of researchers and technologists at the Italian National
Research Council (CNR).

The notebooks are:

-   `download_2020.ipynb`
-   `download_2023.ipynb`

Each notebook:

1.  Fetches relevant web pages from `https://archivio.urp.cnr.it`
2.  Identifies linked PDF files associated with the relevant calls and
    evaluation criteria
3.  Downloads and stores the files in the `data/` directory

The scripts focus on two competitive selection procedures:

-   The 2020 procedure
-   The 2023 procedure (which is the object of the analysis presented in
    the aforementioned paper)

After execution of the notebooks, the fetched data is structured as follows:

```
    data/
    ├── 2020/
    │   ├── calls/
    │   └── criteria/
    └── 2023/
        ├── calls/
        │   ├── 315.62 RD/
        │   ├── 315.63 SR/
        │   ├── 315.64 TD/
        │   └── 315.65 ST/
        └── criteria/
            ├── 315.62 RD/
            ├── 315.63 SR/
            ├── 315.64 TD/
            ├── 315.65 ST/
```

-   `calls/` contains the official calls for applications.
-   `criteria/` contains the evaluation criteria documents for each
    selection procedure.

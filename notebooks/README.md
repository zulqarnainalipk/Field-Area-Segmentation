# Notebook guide

`main.ipynb` is the original end-to-end competition notebook. It is preserved under `notebooks/` so the project has a predictable structure without changing the experiment itself.

For future work, keep new analyses in this directory and separate data inspection from model experiments:

```text
notebooks/
├── main.ipynb
├── 01_data_inspection.ipynb
├── 02_mask_quality_review.ipynb
├── 03_polygon_error_analysis.ipynb
└── README.md
```

When comparing a new run with the competition result, record the image split, number of submissions, model configuration, and evaluation metrics. Field-boundary performance can look different across regions, so the data split is part of the result rather than an implementation detail.

## Author

Zulqarnain Ali — [zulqarnainali.com](https://zulqarnainali.com) · [zulqar445ali@gmail.com](mailto:zulqar445ali@gmail.com)

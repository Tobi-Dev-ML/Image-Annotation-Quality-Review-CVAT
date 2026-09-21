# Image Annotation & Quality Review using CVAT

An image annotation and quality-control project focused on bounding-box annotation for computer vision datasets using CVAT.

## Project Overview

This project involved annotating **16 images** containing people and everyday objects using the CVAT annotation platform.

A total of **92 bounding-box annotations** were created across four object classes:

* Person
* Vehicle
* Laptop
* Phone

The exported CVAT annotations were subsequently reviewed and validated using Python.

## Annotation Summary

| Metric                        |  Result |
| ----------------------------- | ------: |
| Images annotated              |      16 |
| Total bounding boxes          |      92 |
| Person                        |      67 |
| Vehicle                       |      18 |
| Laptop                        |       4 |
| Phone                         |       3 |
| Average annotations per image |    5.75 |
| Invalid boxes                 |       0 |
| Out-of-bounds boxes           |       0 |
| Images visually reviewed      | 16 / 16 |

## Annotation Workflow

1. Prepared the source image dataset
2. Created an annotation project in CVAT
3. Defined object classes
4. Applied bounding-box annotations
5. Exported the annotations in CVAT XML format
6. Parsed the exported annotations using Python
7. Checked bounding-box coordinates
8. Checked image-boundary compliance
9. Reviewed annotation distribution
10. Performed visual quality review
11. Prepared structured annotation summaries and QA documentation

## Quality Control

The exported annotations were checked programmatically for:

* Invalid bounding-box dimensions
* Negative coordinates
* Coordinates extending beyond image boundaries
* Label consistency
* Annotation distribution

All **92 bounding boxes passed the coordinate and boundary checks**.

A visual review of all **16 images** was also performed to check bounding-box placement and label consistency. No obvious annotation errors were identified during the review.

## Tools Used

* CVAT
* Python
* Pandas
* XML
* Google Colab

## Repository Structure

```text
image-annotation-quality-review-cvat/
│
├── README.md
├── annotations/
│   └── image_annotations_cvat.zip
│
├── data/
│   ├── annotation_summary.csv
│   └── annotation_quality_summary.csv
│
├── reports/
│   └── Annotation_Quality_Report.pdf
│
├── evidence/
│   ├── annotation_overview.png
│   ├── annotation_detail.png
│   └── annotation_QA_summary.png
│
└── notebook/
    └── Image_Annotation_Portfolio.ipynb
```

## Project Outcome

The project demonstrates practical experience with **image annotation, bounding-box annotation, object detection datasets, CVAT, data labeling, annotation quality assurance, dataset validation, CVAT XML processing, and visual annotation review**.

The final materials provide both the original annotation export and the supporting Python-based quality-control evidence.

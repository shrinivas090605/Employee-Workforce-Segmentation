# Employee-Workforce-Segmentation

Unsupervised learning project that segments the employees of the IBM HR Analytics dataset (1,470 employees) using PCA, K-Means and Hierarchical clustering, with a workforce analytics dashboard.

## Repository contents
| File | Description |
|---|---|
| `Workforce_Segmentation_Notebook.ipynb` | Full notebook (PCA, clustering, analysis) |
| `Employee_Segmentation_Report.docx` | Segment profiles, high-risk clusters, departments, performance and retention-risk groups |
| `PCA_Summary.docx` | Variance explained, component interpretation, PCA visualisation |
| `Workforce_Analytics_Dashboard.html` | Interactive dashboard (open in any browser) |

## Approach
- 20 standardised work-related features; attrition, department and performance kept out of clustering so they can validate the segments
- PCA to 12 components (about 83% of variance)
- K-Means with k chosen by elbow, silhouette and Davies-Bouldin (k = 3)
- Hierarchical clustering (Ward) compared with K-Means (Adjusted Rand Index 0.75)
- Analysis of high-risk clusters, department segments, performance groups and retention-risk groups

## Key findings
- Three segments: Early-Career Core, Established Mid-Career, Senior Experts
- Early-Career Core is high risk: 21.3% attrition vs 16.1% company average
- The High risk tier holds 75% of all leavers
- Employees rated 4 leave as often as those rated 3
- Segments overlap (low silhouette), so they are best read as career-stage bands

## How to run
1. Upload `Workforce_Segmentation_Notebook.ipynb` to Google Colab.
2. Click Runtime > Run all (the dataset downloads automatically).
3. Open `Workforce_Analytics_Dashboard.html` in a browser.


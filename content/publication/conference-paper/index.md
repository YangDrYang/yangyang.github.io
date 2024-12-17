<!-- ---
title: "An example conference paper"
authors:
  - admin
date: "2024-07-05T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2024-07-05T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: IEEE Transactions on Aerospace and Electronic Systems
publication_short: In *IEEE TAES*

abstract: Orbit determination (OD) is a fundamental problem in space surveillance and tracking, crucial for ensuring the safety of space assets. Real-world ground-based optical tracking scenarios often involve challenges such as limited measurement time, short visible arcs, and the presence of outliers, leading to sparse and non-Gaussian observational data. Additionally, the highly perturbative and nonlinear orbit dynamics of resident space objects (RSOs) in low Earth orbit (LEO) add further complexity to the OD problem. This article introduces a variant of the higher order unscented Kalman estimator (HOUSE) called w -HOUSE, which employs a square-root formulation and addresses the challenges posed by nonlinear and non-Gaussian OD problems. The effectiveness of w -HOUSE was demonstrated through synthetic and real-world measurements, specifically outlier-contaminated angle-only measurements collected for the Sentinel 6 A satellite flying in LEO. Comparative analyzes are conducted with the original HOUSE (referred to as δ -HOUSE), unscented Kalman filters (UKF), conjugate unscented transformation (CUT) filters, and precise OD solutions estimated via onboard global navigation satellite system measurements. The results reveal that the proposed w -HOUSE filter exhibits greater robustness when dealing with varying values of the dependent parameter compared to the original δ -HOUSE. Moreover, it surpasses all other filters in terms of positioning accuracy, achieving 3-D root-mean-square errors of less than 60 m in a three-day scenario. This research suggests that the w -HOUSE filter represents a viable alternative to UKF and CUT filters, offering improved positioning performance in handling the nonlinear and non-Gaussian OD problems associated with LEO RSOs.

# Summary. An optional shortened abstract.
summary: HOUSE based angle only orbit determination.

tags:
  - Source Themes
featured: true

links:
#- name: Custom Link
#  url: http://example.org
# url_pdf: http://eprints.soton.ac.uk/352095/1/Cushen-IMV2013.pdf
# url_code: '#'
# url_dataset: '#'
# url_poster: '#'
# url_project: ''
# url_slides: ''
# url_source: '#'
# url_video: '#'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
image:
  caption: "Image credit: [**Unsplash**](https://unsplash.com/photos/pLCdAaMFLTE)"
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects:
# - internal-project

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
# slides: example
---

{{% alert note %}}
Click the _Cite_ button above to demo the feature to enable visitors to import publication metadata into their reference management software.
{{% /alert %}}

{{% alert note %}}
Click the _Slides_ button above to demo academia's Markdown slides feature.
{{% /alert %}}

Supplementary notes can be added here, including [code and math](https://sourcethemes.com/academic/docs/writing-markdown-latex/). -->

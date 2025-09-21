---
title: "Hardware-Based Time Synchronization for a Multi-Sensor System"
authors:
  - admin
date: "2024-10-14T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2024-12-25T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: 2024 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS)
publication_short: In *IROS*

abstract: Accurate time synchronization is crucial for multisensor fusion, which is widely used in mobile robotics, autonomous driving, and virtual reality. Despite many advancements, precise multi-sensor synchronization is still challenging due to the sensors’ internal characteristics, data filtering, disjointed clock reference, and transmission delay caused by operation system scheduling. This paper proposes a novel hardware-based synchronization solution to achieve synchronization in microsecond-level precision. By introducing a Sensor Adaptor board that provides a unified clock reference, the proposed hardware architecture enables high-precision synchronization across multiple sensors. Furthermore, we develop a method for Visual-Inertial time synchronization that actively controls the exposure duration using an ambient light sensor. By managing the IMU clock signal and exposure trigger, we align the camera’s sampling moment with the authentic IMU sampling time and significantly reduce the time discrepancy in the Visual-Inertial system. Experiments are conducted to evaluate the efficiency of the proposed method and system, including comparisons with previous work. The results indicate that our method can achieve precise time synchronization and be successfully implemented in multi-sensor systems.

# Summary. An optional shortened abstract.
summary: Time Synchronization.

tags:
  - Source Themes
featured: false

draft: true

_build:
  list: never
  render: false

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

Supplementary notes can be added here, including [code and math](https://sourcethemes.com/academic/docs/writing-markdown-latex/).

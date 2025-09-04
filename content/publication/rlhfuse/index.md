---
title: 'Optimizing RLHF Training for Large Language Models with Stage Fusion'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - Yinmin Zhong
  - Zili Zhang
  - admin
  - Shengyu Liu
  - Yukun Chen
  - Changyi Wan
  - Hanpeng Hu
  - Lei Xia
  - Ranchen Ming
  - Yibo Zhu
  - Xin Jin

date: "2025-04-28T00:00:00Z"
# doi: '10.48550/arXiv.2305.05920'

# Schedule page publish date (NOT publication's date).
# publishDate: '2023'

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ['1']

publication_short: In *NSDI 2025*

abstract: 'We present RLHFuse, an efficient training system with stage fusion for Reinforcement Learning from Human Feedback (RLHF). Due to the intrinsic nature of RLHF training, i.e., the data skewness in the generation stage and the pipeline bubbles in the training stage, existing RLHF systems suffer from low GPU utilization. RLHFuse breaks the traditional view of RLHF workflow as a composition of individual tasks, splitting each task into finer-grained subtasks, and performing stage fusion to improve GPU utilization. RLHFuse contains two key ideas. First, for generation and inference tasks, RLHFuse splits them into sample-level subtasks, enabling efficient inter-stage fusion to overlap the execution of generation and inference stages, thus mitigating the original generation bottleneck dominated by long-tailed samples. Second, for training tasks, RLHFuse breaks them into subtasks of micro-batches and performs intra-stage fusion to concurrently execute these subtasks in the training stage with a fused pipeline schedule, effectively mitigating the pipeline bubbles. The experiments show that RLHFuse increases the training throughput by up to 3.7×, compared to existing systems.'

# Summary. An optional shortened abstract.
tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org
url_pdf: 'https://www.usenix.org/conference/nsdi25/presentation/zhong'
url_code: ''
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# image:
#   caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/pLCdAaMFLTE)'
#   focal_point: ''
#   preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
# projects:
#   - example

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
# slides: example
---
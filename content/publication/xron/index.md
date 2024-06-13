---
title: 'XRON: A Hybrid Elastic Cloud Overlay Network for Video Conferencing at Planetary Scale'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - Bingyang Wu
  - Kun Qian
  - Bo Li
  - Yunfei Ma
  - Qi Zhang
  - Zhigang Jiang
  - Jiayu Zhao
  - Dennis Cai
  - Ennan Zhai
  - Xuanzhe Liu
  - Xin Jin

# # Author notes (optional)
# author_notes:
#   - 'Equal contribution'
#   - 'Equal contribution'

date: '2023-09-10T00:00:00Z'
doi: 'https://dl.acm.org/doi/abs/10.1145/3603269.3604845'

# Schedule page publish date (NOT publication's date).
publishDate: '2017-01-01T00:00:00Z'

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ['1']

# Publication name and optional abbreviated publication name.
publication: In *ACM International Conference on Applications, Technologies, Architectures, and Protocols for Computer Communication*
publication_short: In *SIGCOMM 2023*

abstract: 'Quality and cost are two key considerations for video conferencing services. Service providers face a dilemma when selecting network tiers to build their infrastructure---relying on Internet links has poor quality, while using premium links brings excessive cost.We present XRON, a hybrid elastic cloud overlay network for our planetary-scale video conferencing service. XRON differs from prior overlays with two distinct features. First, XRON is hybrid, i.e., it leverages both Internet and premium links to simultaneously achieve high quality and low cost. Second, XRON is elastic, i.e., it exploits elastic cloud resources to adaptively scale its capacity based on realtime demand. The data plane of XRON combines active probing and passive tracking for scalable link state monitoring, uses asymmetric forwarding based on heterogeneous bidirectional link qualities, and quickly reacts to sudden link degradations without the control plane involvement. The control plane of XRON predicts video traffic based on application knowledge, and computes global forwarding paths and reaction plans with scalable algorithms. Large-scale deployment in DingTalk shows that XRON reduces video stall ratio and bad audio fluency by 77\% and 65.2\%, respectively, compared to using Internet links only, and reduces cost by 79\%, compared to using premium links only.'

# # Summary. An optional shortened abstract.
# summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum.

tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://dl.acm.org/doi/abs/10.1145/3603269.3604845'
url_code: ''
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: ''

# # Featured image
# # To use, add an image named `featured.jpg/png` to your page's folder.
# image:
#   caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/pLCdAaMFLTE)'
#   focal_point: ''
#   preview_only: false

# # Associated Projects (optional).
# #   Associate this publication with one or more of your projects.
# #   Simply enter your project's folder or file name without extension.
# #   E.g. `internal-project` references `content/project/internal-project/index.md`.
# #   Otherwise, set `projects: []`.
# projects:
#   - example

# # Slides (optional).
# #   Associate this publication with Markdown slides.
# #   Simply enter your slide deck's filename without extension.
# #   E.g. `slides: "example"` references `content/slides/example/index.md`.
# #   Otherwise, set `slides: ""`.
# slides: example
---
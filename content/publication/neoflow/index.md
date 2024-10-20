---
title: 'NeoFlow: A Flexible Framework for Enabling Efficient Compilation for High Performance DNN Training'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - Size Zheng
  - Renze Chen
  - Yicheng Jin
  - Anjiang Wei
  - admin
  - Xiuhong Li
  - Shengen Yan
  - Yun Liang

# # Author notes (optional)
# author_notes:
#   - 'Equal contribution'
#   - 'Equal contribution'

date: '2021-12-28T00:00:00Z'
doi: '10.1109/TPDS.2021.3138862'

# Schedule page publish date (NOT publication's date).
publishDate: '2017-01-01T00:00:00Z'

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ['2']

# Publication name and optional abbreviated publication name.
publication: In *IEEE Transactions on Parallel and Distributed Systems*
publication_short: In *TPDS 2021*

abstract: Deep neural networks (DNNs) are increasingly deployed in various image recognition and natural language processing applications. The continuous demand for accuracy and high performance has led to innovations in DNN design and a proliferation of new operators. However, existing DNN training frameworks such as PyTorch and TensorFlow only support a limited range of operators and rely on hand-optimized libraries to provide efficient implementations for these operators. To evaluate novel neural networks with new operators, the programmers have to either replace the holistic new operators with existing operators or provide low-level implementations manually. Therefore, a critical requirement for DNN training frameworks is to provide high-performance implementations for the neural networks containing new operators automatically in the absence of efficient library support. In this article, we introduce NeoFlow, which is a flexible framework for enabling efficient compilation for high-performance DNN training. NeoFlow allows the programmers to directly write customized expressions as new operators to be mapped to graph representation and low-level implementations automatically, providing both high programming productivity and high performance. First, NeoFlow provides expression-based automatic differentiation to support customized model definitions with new operators. Then, NeoFlow proposes an efficient compilation system that partitions the neural network graph into subgraphs, explores optimized schedules, and generates high-performance libraries for subgraphs automatically. Finally, NeoFlow develops an efficient runtime system to combine the compilation and training as a whole by overlapping their execution. In the experiments, we examine the numerical accuracy and performance of NeoFlow. The results show that NeoFlow can achieve similar or even better performance at the operator and whole graph level for DNNs compared to deep learning frameworks. Especially, for novel networks training, the geometric mean speedups of NeoFlow to PyTorch, TensorFlow, and CuDNN are 3.16X, 2.43X, and 1.92X, respectively.

# # Summary. An optional shortened abstract.
# summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum.

tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9664259'
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
---
permalink: /
title: "About Me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% include toc %}

I am an **M.Sc. in Artificial Intelligence** student at **Nanyang Technological University (NTU)** in Singapore. My expertise lies in bridging the gap between advanced AI research and production-scale engineering, with a focus on generative models, LLMs, and efficient machine learning systems.

I graduated **Cum Laude** with a B.Sc. in Computer Science from **Universitas Gadjah Mada (UGM)**.

Professional Experience
======

**Data Scientist @ JULO** *(May 2022 – July 2025)*

* **Credit Scoring & Risk:** Architected end-to-end credit scoring engines using XGBoost and LightGBM.
* **Low-Latency Systems:** Engineered a real-time risk system that increased Risk-Adjusted Returns (RAR) by 30% while maintaining sub-second inference speeds.
* **ML Infrastructure:** Led the migration of ML workflows from AWS to GCP, accelerating model training cycles from 5 days to 1 day.
* **Observability:** Built automated dashboards to monitor concept drift (PSI) and business metrics like ROI and CLV.
* **Leadership:** Mentored junior data scientists on ML best practices and internal domain logic.

Portofolio
======

* **Style Diffusion Reproduction (ICCV 2023):** 
  * Reproduced the complete DDPM architecture and attention mechanisms in PyTorch.
  * Implemented CLIP-based disentanglement to match official quality while adding novel multi-style blending capabilities.
  * [Github Link](https://github.com/ntu-ai-group-10/style_diffusion_reproduction)
  
  ![porto__style_diffusion__image_grid_output](/images/porto__style_diffusion__image_grid_output.png)

  ![porto__style_diffusion__image_grid_output_style_mix](/images/porto__style_diffusion__image_grid_output_style_mix.png)

* **Local RAG Document Q&A:** 
  * Developed a privacy-focused RAG pipeline for unstructured PDFs using LlamaIndex and ChromaDB.
  * Integrated a two-stage retrieval strategy (High-K + Reranking) powered by local LLMs via Ollama.
  * [Github Link](https://github.com/Ardacandra/rag_document_qna)

  ![porto__rag__sample_output](/images/porto__rag__sample_output.png)
  
* **Deepfake Audio Detection:** 
  * Created a Transformer-based classifier for AI-synthesized speech (TTS/VC) using Librosa for signal processing.
  * Achieved a 99.98% test accuracy, securing Runner-up at the DeepDetect Hackathon 2025.
  * [Github Link](https://github.com/Ardacandra/deepdetect_audio_deepfake_detection_challenge)

* **CapsNet COVID-19 Diagnostics:** 
  * Trained a Capsule Network on over 6,300 chest X-rays to classify COVID-19 and Pneumonia cases.
  * Utilized dynamic routing for viewpoint invariance, achieving 94.29% accuracy with fewer parameters than standard CNNs.
  * [Github Link](https://github.com/Yakuy/CapsNet-Covid19-X-Ray-Detection)

* **Intelligent Mask Detection:** 
  * Developed a Faster R-CNN model optimized for real-time inference on resource-constrained hardware like the GTX 960.
  * Recognized as the Winner of the Codig 3.0 Data Mining Competition.
  * [Github Link](https://github.com/Yakuy/proper-use-of-mask-detection)

    ![porto__mask_detection__sample_output](/images/porto__mask_detection__sample_output.png)

    ![porto__mask_detection__demo](/images/porto__mask_detection__demo.gif)

Publications
======

* **Human Face Detection and Tracking Using RetinaFace Network for Surveillance Systems**
    * **Venue:** 47th Annual Conference of the IEEE Industrial Electronics Society (IECON), 2021.
    * **Excerpt:** Engineered a CCTV face tracking pipeline using RetinaFace and detection-based tracking, improving face detection recall by 4.47% in low-illumination environments.
    * [Paper Link](https://ieeexplore.ieee.org/document/9589577)

* **Medical Subject Headings (MeSH) Indexing Using Unsupervised Learning**
    * **Venue:** 2021 International Conference on Computer, Control, Informatics and Its Applications (ICCCIA).
    * **Excerpt:** Implemented Latent Dirichlet Allocation (LDA) for unsupervised topic modeling to automate MeSH indexing, achieving a 74% topic similarity match against human-expert labels.
    * [Paper Link](https://dl.acm.org/doi/10.1145/3489088.3489096)

Technical Toolkit
======

* **Programming & Databases:** Python, SQL.
* **ML Frameworks:** PyTorch, TensorFlow, Scikit-Learn, Hugging Face, LlamaIndex, OpenCV.
* **Cloud & MLOps:** GCP (BigQuery, Compute Engine), AWS, Docker, Git/GitHub, CI/CD.
* **Domain Expertise:** Generative AI, LLMs, Financial Risk Modeling, Computer Vision, and Audio Signal Processing.

Let's Connect
======

I am currently based in **Singapore** and am open to collaborations in AI research or engineering.

* **Email:** [ardacandrasubiantoro@gmail.com](mailto:ardacandrasubiantoro@gmail.com)
* **LinkedIn:** [linkedin.com/in/ardacandra-subiantoro](https://linkedin.com/in/ardacandra-subiantoro)
* **GitHub:** [github.com/Ardacandra](https://github.com/Ardacandra)

<!-- This is the front page of a website that is powered by the [Academic Pages template](https://github.com/academicpages/academicpages.github.io) and hosted on GitHub pages. [GitHub pages](https://pages.github.com) is a free service in which websites are built and hosted from code and data stored in a GitHub repository, automatically updating when a new commit is made to the repository. This template was forked from the [Minimal Mistakes Jekyll Theme](https://mmistakes.github.io/minimal-mistakes/) created by Michael Rose, and then extended to support the kinds of content that academics have: publications, talks, teaching, a portfolio, blog posts, and a dynamically-generated CV. Incidentally, these same features make it a great template for anyone that needs to show off a professional template!

 You can fork [this template](https://github.com/academicpages/academicpages.github.io) right now, modify the configuration and Markdown files, add your own PDFs and other content, and have your own site for free, with no ads!

A data-driven personal website
======
Like many other Jekyll-based GitHub Pages templates, Academic Pages makes you separate the website's content from its form. The content & metadata of your website are in structured Markdown files, while various other files constitute the theme, specifying how to transform that content & metadata into HTML pages. You keep these various Markdown (.md), YAML (.yml), HTML, and CSS files in a public GitHub repository. Each time you commit and push an update to the repository, the [GitHub pages](https://pages.github.com/) service creates static HTML pages based on these files, which are hosted on GitHub's servers free of charge.

Many of the features of dynamic content management systems (like Wordpress) can be achieved in this fashion, using a fraction of the computational resources and with far less vulnerability to hacking and DDoSing. You can also modify the theme to your heart's content without touching the content of your site. If you get to a point where you've broken something in Jekyll/HTML/CSS beyond repair, your Markdown files describing your talks, publications, etc. are safe. You can rollback the changes or even delete the repository and start over - just be sure to save the Markdown files! You can also write scripts that process the structured data on the site, such as [this one](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb) that analyzes metadata in pages about talks to display [a map of every location you've given a talk](https://academicpages.github.io/talkmap.html).

For those users that need more advanced functionality, the template also supports the following popular tools:
- [MathJax](https://www.mathjax.org/) for mathematical equations
- [Mermaid](https://mermaid.js.org/) for diagraming
- [Plotly](https://plotly.com/javascript/) for plotting

Getting started
======
1. Register a GitHub account if you don't have one and confirm your e-mail (required!)
1. Fork [this template](https://github.com/academicpages/academicpages.github.io) by clicking the "Use this template" button in the top right. 
1. Go to the repository's settings (rightmost item in the tabs that start with "Code", should be below "Unwatch"). Rename the repository "[your GitHub username].github.io", which will also be your website's URL.
1. Set site-wide configuration and create content & metadata (see below -- also see [this set of diffs](https://archive.is/3TPas) showing what files were changed to set up [an example site](https://getorg-testacct.github.io) for a user with the username "getorg-testacct")
1. Upload any files (like PDFs, .zip files, etc.) to the files/ directory. They will appear at https://[your GitHub username].github.io/files/example.pdf.  
1. Check status by going to the repository settings, in the "GitHub pages" section

Site-wide configuration
------
The main configuration file for the site is in the base directory in [_config.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_config.yml), which defines the content in the sidebars and other site-wide features. You will need to replace the default variables with ones about yourself and your site's github repository. The configuration file for the top menu is in [_data/navigation.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_data/navigation.yml). For example, if you don't have a portfolio or blog posts, you can remove those items from that navigation.yml file to remove them from the header. 

Create content & metadata
------
For site content, there is one Markdown file for each type of content, which are stored in directories like _publications, _talks, _posts, _teaching, or _pages. For example, each talk is a Markdown file in the [_talks directory](https://github.com/academicpages/academicpages.github.io/tree/master/_talks). At the top of each Markdown file is structured data in YAML about the talk, which the theme will parse to do lots of cool stuff. The same structured data about a talk is used to generate the list of talks on the [Talks page](https://academicpages.github.io/talks), each [individual page](https://academicpages.github.io/talks/2012-03-01-talk-1) for specific talks, the talks section for the [CV page](https://academicpages.github.io/cv), and the [map of places you've given a talk](https://academicpages.github.io/talkmap.html) (if you run this [python file](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.py) or [Jupyter notebook](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb), which creates the HTML for the map based on the contents of the _talks directory).

**Markdown generator**

The repository includes [a set of Jupyter notebooks](https://github.com/academicpages/academicpages.github.io/tree/master/markdown_generator
) that converts a CSV containing structured data about talks or presentations into individual Markdown files that will be properly formatted for the Academic Pages template. The sample CSVs in that directory are the ones I used to create my own personal website at stuartgeiger.com. My usual workflow is that I keep a spreadsheet of my publications and talks, then run the code in these notebooks to generate the Markdown files, then commit and push them to the GitHub repository.

How to edit your site's GitHub repository
------
Many people use a git client to create files on their local computer and then push them to GitHub's servers. If you are not familiar with git, you can directly edit these configuration and Markdown files directly in the github.com interface. Navigate to a file (like [this one](https://github.com/academicpages/academicpages.github.io/blob/master/_talks/2012-03-01-talk-1.md) and click the pencil icon in the top right of the content preview (to the right of the "Raw | Blame | History" buttons). You can delete a file by clicking the trashcan icon to the right of the pencil icon. You can also create new files or upload files by navigating to a directory and clicking the "Create new file" or "Upload files" buttons. 

Example: editing a Markdown file for a talk
![Editing a Markdown file for a talk](/images/editing-talk.png)

For more info
------
More info about configuring Academic Pages can be found in [the guide](https://academicpages.github.io/markdown/), the [growing wiki](https://github.com/academicpages/academicpages.github.io/wiki), and you can always [ask a question on GitHub](https://github.com/academicpages/academicpages.github.io/discussions). The [guides for the Minimal Mistakes theme](https://mmistakes.github.io/minimal-mistakes/docs/configuration/) (which this theme was forked from) might also be helpful. -->

---
title: "Vtable hijacking: Object Type Integrity for run-time type information"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- "Marco Schröder"
- "Stefan Machmeier"
- "Vincent Heuveline"

# Author notes (optional)
author_notes:
- "Marco Schröder"
- "Stefan Machmeier"
- "Vincent Heuveline"

date: "2023-03-02T00:00:00Z"
doi: "10.11588/EMCLPP.2023.1.94354"

# Schedule page publish date (NOT publication's date).
publishDate: "2023-03-02T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["3"]

# Publication name and optional abbreviated publication name.
publication: In Preprint Series of the Engineering Mathematics and Computing Lab
publication_short: In Preprint Series of the EMCL

abstract: Attackers try to hijack the control-flow of a victim’s process by exploiting a run-time vulnerability. Vtable hijacking is a state-of-the-art technique adversaries use to conduct control-flow hijacking attacks. It abuses the reliance of language constructs related to polymorphism on dynamic type information. The Control Flow Integrity (CFI) security policy is a well-established solution designed to prevent attacks that corrupt the control-flow. Deployed defense mechanisms based on CFI are often generic, which means that they do not consider high-level programming language semantics. This makes them vulnerable to vtable hijacking attacks. Object Type Integrity (OTI) is an orthogonal security policy that specifically addresses vtable hijacking. CFIXX is a Clang compiler extension that enforces OTI in the context of dynamic dispatch, which prevents vtable hijacking in this setting. However, this extension does not enforce OTI in context of polymorphism. The contribution of this work is a practical implementation to enable OTI in the context of C++’s run-time type information for the dynamic_cast expressions and the typeid operator.

# Summary. An optional shortened abstract.
# summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum.

tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: ''
url_code: ''
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: 'CFIXX metadata rotation'
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
# projects:
# - example

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
# slides: example
---

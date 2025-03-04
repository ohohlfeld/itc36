---
title: Authors
menu: top-nav
menu-index: 5
---

# Author Information

## Submission guidelines

* Submitted papers must be original work, not under review at other journals/conferences, and may comprise of a maximum of 9 (full papers) or 5 (short papers) A4 in 2-column IEEE conference style with a minimum font size of 10 pt. Papers should be submitted electronically using HotCRP. All accepted papers must be presented at the conference by one of the authors.
* Submitted papers are single-blind reviewed. Please include author names and affiliations in your manuscript as in the provided template below.
* Link for Submissions: [here](https://itc2025.hotcrp.com/)
* Template for A4 (210 mm x 297 mm) pages in 2-column IEEE conference style with a minimum font size of 10 pt: LaTex and MS Word and is available for download [here](https://www.ieee.org/conferences/publishing/templates.html).

## Author registration

For your paper to be included in the final programme and to be published in the {{ site.conference-name }} Proceedings, at least 1 author needs to register before the deadline of March 31st at full rate. Papers not covered by any registration by that deadline will automatically be removed from the final programme.

## Open access

ITC follows an open access strategy. Accepted ITC conference and workshop papers can be downloaded from the open ITC digital library. In addition, ITC makes the effort to index accepted papers in public A&I databases. By getting sponsorship of technical communities like IEEE and ACM, as well as sticking to corresponding rules with respect to technical quality, papers of previous ITC editions were included in the corresponding databases IEEE Xplore and ACM DL.

Since ITC retains the copyrights, it is possible to make the papers accessible for free via the ITC digital library. This helps to increase the visibility and accessibility of accepted papers.

## Preparing the final manuscript

March 4th 2025: These instructions are not yet finalized and will be further updated.

### Auhor Final Paper Preparation and Submission Instructions

To submit the camera-ready copy, you need to complete the following steps by March 31st, 2025 at the latest.


* Revise your paper according to the reviewer comments and format it correctly.
* Include the copyright note in your paper.
* Include the conference header on the first page of your paper.
* Process the paper with PDF eXpress to obtain an IEEE Xplore-compatible pdf file.
* Upload the camera-ready version to via hotcrp.
* Sign the copyright form and sent it per email to [itc36_crv [at] iik [dot] ntnu [dot] no](mailto:itc36_crv@iik.ntnu.no). The subject of the email should include the submission number of the paper in hotcrp followed by "copyright form", e.g., " Paper 121 copyright form".

Details on the copyright notice, the conference header, and PDF eXpress can be found below.

In case of questions please contact us via [itc36_crv [at] iik [dot] ntnu [dot] no](mailto:itc36_crv@iik.ntnu.no).

### Conference Header

Each paper must include a header with the conference title on the first page. The text of the header has to be "2025 36th International Teletraffic Congress (ITC 36)" LaTeX users can insert the header by using the tikz package.
```
\usepackage{tikz}
\usetikzlibrary{positioning}
```
Additionally, the following commands need to be added after the IEEEkeywords environment.
```
\begin{tikzpicture}[overlay, remember picture]
\path (current page.north) node (anchor) {};
\node [below=of anchor] {%
2025 36th International Teletraffic Congress (ITC 36)};
\end{tikzpicture}```

### Copyright Notice

Each paper must include a copyright notice at the bottom of the first page. The copyright notice is: 978-3-948377-03-8/19/$31.00 ©2025 ITC. 
LaTeX users can insert the copyright notice by adding the following commands right before \maketitle.

\IEEEpubid{\makebox[\columnwidth]{978-3-948377-03-8/19/\$31.00 \copyright 2025 ITC \hfill} \hspace{\columnsep}\makebox[\columnwidth]{ }}```


### PDF eXpress

Make sure you added the correct copyright notice and proof-read your paper carefully so that no further changes are required. IEEE PDF eXpress can either be used to create an IEEE Xplore-compatible paper from source files or check an existing PDF document. However, any changes made to the PDF after IEEE PDF eXpress conversion or checking may invalidate the PDF. Papers not compatible with IEEE Xplore will not be included in the proceedings. To validate your paper, visit the IEEE PDF eXpress page and use either your existing account or create a new one. The conference ID is 65175X. After logging in, use ‘Create New Title’ for each of your papers and follow the instructions. Once the paper passed the validation upload the PDF eXpress-signed PDF in hotcrp.


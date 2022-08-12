# ES-LTR-Implicit-Explicit-Correlation
Correlation of Implicit feedback (click-through data) versus Explicit Human Relevance Judgements for Learning to Rank (LTR)

This script correlates the ranking performance of a ’real world’ Enterprise Search (ES) service of a large organisation using both relevance judgements and
click-through data. We generate and publish a small manually annotated LTR dataset (ENTRP-SRCH.txt) and calculate a Spearman correlation coefficient.


The attached dataset and code were used to perform correlation and ranking performance tests.

The LTR dataset is formatted as follows: -
![LETOR_format_diagram-with-clickThru](https://user-images.githubusercontent.com/51714656/179519935-eb7329c6-e9cb-4e69-b6a0-a71eef16ab03.png)

To reproduce, simply download the code (python ipynb file) and dataset (txt file).  It was compliled using python 3 and requires the installation (pip3) of datapane,jinja2 and scipy packages.

This research was usertaken by Colin Daly and Dr. Yvette Graham and has been partially funded by the ADAPT Centre and Trinity College Dublin

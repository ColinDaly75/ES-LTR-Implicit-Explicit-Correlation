# ES-LTR-Implicit-Explicit-Correlation
Correlation of Implicit feedback (click-through data) versus Explicit Human Relevance Judgements for Learning to Rank (LTR)

This script correlates the ranking performance of a ’real world’ Enterprise Search (ES) service of a large organisation using both relevance judgements and
click-through data (CTR). 


The click-through rate (CTR) is generally defined as the percentage of the number of clicks to the number of impressions~\cite{Chapelle2011}.  

For the purposes of this study, we calculate the CTR as a ratio showing how often people who see the document,d, in the returned listing actually generated by query,q, end up clicking it.
 
 <img src="https://render.githubusercontent.com/render/math?math=e^{i \pi} = -1">
  
 
 
 <img src="https://render.githubusercontent.com/render/math?math={\L = -\sum_{j}[T_{j}ln(O_{j})] + \frac{\lambda W_{ij}^{2}}{2} \rightarrow \text{one-hot} \rightarrow -ln(O_{c}) + \frac{\lambda W_{ij}^{2}}{2}}#gh-light-mode-only">
 
 <img src="https://render.githubusercontent.com/render/math?math={L = 1}">
 
<!-- %= \frac{clicks_{(q,d)}}{impressions_{(q,d)}}#gh-light-mode-only">  -->
 
 \[ CTR_{(q,d)} = \frac{ clicks_{(q,d)}}{impressions_{(q,d)}} \]
 
 where impressions is the sum of clicks for all documents returned for q.  A high CTR is a good indication that users find the document within the listings as helpful and relevant for the given query.


We generate and publish a small manually annotated LTR dataset (ENTRP-SRCH.txt) and calculate a Spearman correlation coefficient.


The attached dataset and code were used to perform correlation and ranking performance tests.

The LTR dataset is formatted as follows: -
![LETOR_format_diagram-with-clickThru](https://user-images.githubusercontent.com/51714656/179519935-eb7329c6-e9cb-4e69-b6a0-a71eef16ab03.png)

To reproduce, simply download the code (python ipynb file) and dataset (txt file).  It was compliled using python 3 and requires the installation (pip3) of datapane,jinja2 and scipy packages.

This research was usertaken by Colin Daly and Dr. Yvette Graham and has been partially funded by the ADAPT Centre and Trinity College Dublin

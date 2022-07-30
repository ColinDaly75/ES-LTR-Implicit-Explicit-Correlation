# ES-LTR-Implicit-Explicit-Correlation
Correlation of Implicit feedback (click-through data) versus Explicit Human Relevance Judgements for Learning to Rank (LTR)

This script correlates the ranking performance of a ’real world’ Enterprise Search (ES) service of a large organisation using both relevance judgements and
click-through data. We generate and publish a small manually annotated LTR dataset (ENTRP-SRCH.txt) and calculate a correlation coefficient of ρ = 0.765. Additionally, the nDCG@10 ranking performance using relevance judgements is just 2.47% higher than when click-though data is used. 

The attached dataset and code were used to generate the following correlation plot.
![Fig-strip-correlation](https://user-images.githubusercontent.com/51714656/179519401-a5c039c3-2979-4ceb-9684-7b875858defc.PNG)

The LTR dataset is formatted as follows: -
![LETOR_format_diagram-with-clickThru](https://user-images.githubusercontent.com/51714656/179519935-eb7329c6-e9cb-4e69-b6a0-a71eef16ab03.png)

